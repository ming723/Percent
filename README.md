# Android完美适配之百分比适配
#### 开发中少不了各种机型的适配，市面上也有各种各样的适配，什么权重适配，dimens适配……，进行计算，写各种分辨率的文件，总之并不是太理想，为此Google终于开始支持百分比的方式布局了.
    具体使用，大家可以下载上面的四个类，复制到自己的项目中
      
        <com.abner.ming.myappli.PercentRelativeLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content">
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="hello"
            android:textColor="#000"
            app:layout_marginLeftPercent="10%"
            />
    </com.abner.ming.myappli.PercentRelativeLayout>
    具体属性有：
    layout_widthPercent
    layout_heightPercent
    layout_marginPercent
    layout_marginLeftPercent
    layout_marginTopPercent
    layout_marginRightPercent
    layout_marginBottomPercent
    layout_marginStartPercent
    layout_marginEndPercent
    layout_aspectRatio
    
#### 需要注意的是，style.xml文件里写入下面的代码
    <resources>
        <declare-styleable name="PercentLayout_Layout">
            <attr format="fraction" name="layout_widthPercent"/>
            <attr format="fraction" name="layout_heightPercent"/>
            <attr format="fraction" name="layout_marginPercent"/>
            <attr format="fraction" name="layout_marginLeftPercent"/>
            <attr format="fraction" name="layout_marginTopPercent"/>
            <attr format="fraction" name="layout_marginRightPercent"/>
            <attr format="fraction" name="layout_marginBottomPercent"/>
            <attr format="fraction" name="layout_marginStartPercent"/>
            <attr format="fraction" name="layout_marginEndPercent"/>
            <attr format="fraction" name="layout_aspectRatio"/>
        </declare-styleable>
    </resources>
    
