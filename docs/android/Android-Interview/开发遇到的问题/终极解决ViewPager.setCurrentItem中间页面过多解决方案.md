### 源码分析相关面试题

- [Volley源码分析](http://www.jianshu.com/p/ec3dc92df581)
- [注解框架实现原理](http://www.jianshu.com/p/20da6d6389e1)
- [okhttp3.0源码分析](http://www.jianshu.com/p/9ed2c2f2a52c)
- [onSaveInstanceState源码分析](http://www.jianshu.com/p/cbf9c3557d64)
- [静默安装和源码编译](http://www.jianshu.com/p/2211a5b3c37f)

### Activity相关面试题

- [保存Activity的状态](http://www.jianshu.com/p/cbf9c3557d64)

### 与XMPP相关面试题

- [XMPP协议优缺点](http://www.jianshu.com/p/2c04ac3c526a)
- [极光消息推送原理](http://www.jianshu.com/p/d88dc66908cf)

### 与性能优化相关面试题

- [内存泄漏和内存溢出区别](http://www.jianshu.com/p/5dd645b05c76)
- [UI优化和线程池实现原理](http://www.jianshu.com/p/c22398f8587f)
- [代码优化](http://www.jianshu.com/p/ebd41eab90df)
- [内存性能分析](http://www.jianshu.com/p/2665c31b9c2f)
- [内存泄漏检测](http://www.jianshu.com/p/1514c7804a06)
- [App启动优化](http://www.jianshu.com/p/f0f73fefdd43)
- [与IPC机制相关面试题](http://www.jianshu.com/p/de4793a4c2d0)

### 与登录相关面试题

- [oauth认证协议原理](http://www.jianshu.com/p/2a6ecbf8d49d)
- [token产生的意义](http://www.jianshu.com/p/9b7ce2d6c195)
- [微信扫一扫实现原理](http://www.jianshu.com/p/a9d1f21bd5e0)

### 与开发相关面试题

- [迭代开发的时候如何向前兼容新旧接口](http://www.jianshu.com/p/cbecadec98de)
- [手把手教你如何解决as jar包冲突](http://www.jianshu.com/p/30fdc391289c)
- [context的原理分析](http://www.jianshu.com/p/2706c13a1769)
- [解决ViewPager.setCurrentItem中间很多页面切换方案](http://www.jianshu.com/p/38ab6d856b56)

### 与人事相关面试题

- [人事面试宝典](http://www.jianshu.com/p/d61b553ff8c9)

### 本文配套视频

- [ViewPager.setCurrentItem的bug演示一](https://v.qq.com/x/page/n0501ylwqx1.html)
- [ViewPager.setCurrentItem解决方案二](https://v.qq.com/x/page/g05012qi6hs.html)

今天做项目用ViewPager.setCurrentItem 方法，如果两个页面相聚比较远，就会闪瞎我的钛合金双眼，中间切换大概20个页面，如下所示：

![img](http://upload-images.jianshu.io/upload_images/4037105-bab7127dbfb0d444?imageMogr2/auto-orient/strip)

setCurrentItem第二个参数设置false，四不四很简单，直接使用如下代码：

```
ViewPager.setCurrentItem(position,false);
```

很不幸的是，使用上面的代码会出现如下效果，扎心了老铁：

![img](http://upload-images.jianshu.io/upload_images/4037105-5dc7bf8e931596ce?imageMogr2/auto-orient/strip)

从第一题点击切换到第十八题，你会发现页面显示空白，如果从第十个页面切换到第十五个页面没事，平时大家估计没有发现这个bug，一般我们使用ViewPager都是底下5个tab页面，从第一个切换到第五个没事，之前我也以为把第二个参数设置false就行，今天才发现，原来如果当页面比较少的时候，大概十个以内，一般没有问题，如果超过十个页面切换就会出现空白，加载不了数据，扎心了，提出解决方案吧，ViewPager滑动使用的是Scroll，咱们把Scroll的滑动时间duration 设置为0就行。

### **自定义一个Scroll类，用于控制ViewPager滑动速度：**

```java
public  class MScroller extends Scroller {

   private static final Interpolator sInterpolator = new Interpolator() {
   public float getInterpolation(float t) {
            t -= 1.0f;
            return t * t * t * t * t + 1.0f;
        }
    };


  public boolean noDuration;

  public void setNoDuration(boolean noDuration) {
        this.noDuration = noDuration;
    }

  public MScroller(Context context) {
        this(context,sInterpolator);
  }

  public MScroller(Context context, Interpolator interpolator) {
        super(context, interpolator);
  }

    @Override
  public void startScroll(int startX, int startY, int dx, int dy, int duration) {
        if(noDuration)
            //界面滑动不需要时间间隔
            super.startScroll(startX, startY, dx, dy, 0);
        else
            super.startScroll(startX, startY, dx, dy,duration);
    }
}
```

#### **上面代码可知：**

1）动态判断页面是否需要滑动，如果不需要滑动，设置滑动时间为0；

### **为方便使用，定义一个辅助类**

```java
public class ViewPageHelper {
    ViewPager viewPager;

    MScroller scroller;

    public ViewPageHelper(ViewPager viewPager) {
        this.viewPager = viewPager;
        init();
    }

    public void setCurrentItem(int item){
        setCurrentItem(item,true);
    }

    public MScroller getScroller() {
        return scroller;
    }


    public void setCurrentItem(int item, boolean somoth){
        int current=viewPager.getCurrentItem();
        //如果页面相隔大于1,就设置页面切换的动画的时间为0
        if(Math.abs(current-item)>1){
            scroller.setNoDuration(true);
            viewPager.setCurrentItem(item,somoth);
            scroller.setNoDuration(false);
        }else{
            scroller.setNoDuration(false);
            viewPager.setCurrentItem(item,somoth);
        }
    }

    private void init(){
        scroller=new MScroller(viewPager.getContext());
        Class<ViewPager>cl=ViewPager.class;
        try {
            Field field=cl.getDeclaredField("mScroller");
            field.setAccessible(true);
            //利用反射设置mScroller域为自己定义的MScroller
            field.set(viewPager,scroller);
        } catch (NoSuchFieldException e) {
            e.printStackTrace();
        }catch (IllegalAccessException e){
            e.printStackTrace();
        }
    }

}
```

#### **由上面代码可知：**

1）Math.abs(current-item)>1 ，通过数学函数判断页面相隔大于1,就设置页面切换的动画的时间为0。

2）这样每次设置页面的时候，通过 helper 就可以自动选择是否有时间间隔了。

3）但是这样有点麻烦，每次还要手动改，而且使用TabLayout或者ViewPagerIndicator的话，它会自动调用ViewPager的方法，无法使用Helper，所以可以采用自定一个ViewPager,代码如下：

```java
public class SuperViewPager extends ViewPager {


    private ViewPageHelper helper;

    public SuperViewPager(Context context) {
        this(context,null);
    }

    public SuperViewPager(Context context, AttributeSet attrs) {
        super(context, attrs);
        helper=new ViewPageHelper(this);

   }

    @Override
    public void setCurrentItem(int item) {
        setCurrentItem(item,true);
    }

    @Override
    public void setCurrentItem(int item, boolean smoothScroll) {
        MScroller scroller=helper.getScroller();
        if(Math.abs(getCurrentItem()-item)>1){
            scroller.setNoDuration(true);
            super.setCurrentItem(item, smoothScroll);
            scroller.setNoDuration(false);
        }else{
            scroller.setNoDuration(false);
            super.setCurrentItem(item, smoothScroll);
        }
    }
}
```

至此完美解决了，ViewPager.setCurrentItem切换页面，效果如下：

![img](http://upload-images.jianshu.io/upload_images/4037105-b2f5486c91c65eae?imageMogr2/auto-orient/strip)

- 欢迎关注微信公众号,长期推荐技术文章和技术视频
- 微信公众号名称：Android干货程序员

![img](http://upload-images.jianshu.io/upload_images/4037105-8f737b5104dd0b5d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)