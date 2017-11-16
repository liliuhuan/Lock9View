# Lock9View
九宫格手势密码
使用方式很简单，直接在xml中引用就可以

<com.example.customer.myapplication.weight.Lock9View
        android:layout_width="300dp"
        android:layout_height="300dp"
        app:nodeLineColor="@color/colorPrimary"
        app:nodeLineWidth="5dp"
        app:nodePadding="20dp"
        app:errorNum="3"
        app:minPoint="4"
        app:normalDrawable="@drawable/chushi"
        app:hightDrawable="@drawable/huizhi"
        >

    </com.example.customer.myapplication.weight.Lock9View>
    Lock9View中有这么一个方法
    /**
     * 设置已有密码
     *
     * @param lock
     */
    public void setLock(String lock) {
        this.lock = lock;
        this.isSetLock = false;
    }
    是用来设置已经保存的密码的，如果设置了这个密码，那么接下来的就是解锁操作
    当然，默认是设置密码的操作
    具体的实现过程大家有兴趣的可以去里面看一下源码
    
    
    首次提交到GitHub上，有什么不足或不对的地方欢迎大家指正！
