**ViewPager和Fragment使用过程中会遇到哪些问题**

### 1. 适配器的选择

使用ViewPager加载多个Fragment时，我一般选择FragmentPagerAdapter。
需要大家注意：
FragmentPagerAdapter：该类内的每一个生成的 Fragment 都将保存在内存之中，因此适用于那些相对静态的页，数量也比较少的场景
但是，如果需要处理有很多页，并且数据动态性较大、占用内存较多的情况，这时候，我们选择怎么是的适配器呢？

应该使用FragmentStatePagerAdapter

FragmentStatePagerAdapter：会把已经创建的Fragment进行保存。会保持Fragment的状态
通过源码分析发现：
FragmentStatePagerAdapter这个类抽象出了一个getItem()方法，用于创建对应的Fragment
而FragmentStatePagerAdapter的.instantiateItem()方法实现中，调用了getIitem()方法。
调用该instantiateItem()方法时，判断一下要生成的 Fragment 是否已经生成过了，如果生成过了，就使用旧的，旧的将被 Fragment.attach()；
如果没有，就调用 getItem() 生成一个新的，新的对象将被 FragmentTransation.add()。
FragmentStatePagerAdapter会将所有生成的 Fragment 对象通过 FragmentManager 保存起来备用，以后需要该 Fragment 时，都会从 FragmentManager 读取，而不会再次调用 getItem() 方法。

### 2. Fragment数据的缓存

Fragment在初始化View对象，把该对象作为一个成员变量进行保存。
再一次初始化Fragment对应的View对象时，判断当前成员变量View对象是否为空。
如果为空，创建新的View对象，否则，不在创建。这样就可以做到对Fragemnt进行数据缓存

这样做的好处：避免了每次加载Fragment都要重新创建View，加载数据了。提高了性能，以及减少了内存的开销。

### 3. ViewPager预加载

我们知道，系统的ViewPager默认提供预加载机制。但是，根据业务需要，取消掉对应的预加载机制。
可以这样做：替换掉系统原生的Viewpager类。将该类中的一个变量mOffscreenPageLimit 设置为0,不进行预加载

### 4. Fragment嵌套Fragment

在Fragment中嵌套Fragment时，一定要使用getChildFragmentManager();

否则，会在ViewPager中出现fragment不会加载的情况，即fragment出现空白页的情况。