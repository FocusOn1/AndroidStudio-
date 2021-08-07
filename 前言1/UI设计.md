一、UI相关概念

## 1.view

![image-20210729105431939](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729105431939.png)

> ps:
>
> View类位于android.view包中；
>
> View类的子类一般都位于android.widget包中。

## 2.view类常用属性

| 属性           | 代码格式                                                     |
| -------------- | ------------------------------------------------------------ |
| id属性         | `android:id="@+id/user"`                                                                                                  ![image-20210729111514939](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729111514939.png) |
| background属性 | 【图片】`android:background="@mipmap/bg"`                                 ![image-20210729111555315](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729111555315.png)                                                                                                            【颜色背景】`android:background="#FF6600"`                                   ![image-20210729111610381](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729111610381.png) |
| padding属性    | ![image-20210729111932519](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729111932519.png)![image-20210729111707739](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729111707739.png)![image-20210729111436703](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729111436703.png)![image-20210729111337219](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729111337219.png) |

## 3.View Group

![image-20210729112139435](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729112139435.png)

> ViewGroup控制其子组件分布时依赖的内部类
>
> | 类                           |                                                              | 功能                     |
> | ---------------------------- | ------------------------------------------------------------ | ------------------------ |
> | ViewGroup.LayoutParams       | ![image-20210729112725070](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729112725070.png) | 控制组件的位置，宽度高度 |
> | ViewGroup.MarginLayoutParams | ![image-20210729113237930](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729113237930.png) | 控制子组件的外边距       |

## 4.Android UI组件的层次结构

![image-20210729113447075](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729113447075.png)

# 二、控制UI界面

## 1.控制UI界面的4种方法

| 方法                    |                                                              | 效果                                                         |
| ----------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 使用XML布局文件【推荐】 | ![image-20210729114052261](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729114052261.png) | ![image-20210729154725424](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729154725424.png) |
| 在Java代码中            | ![image-20210729155652796](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729155652796.png)![image-20210729155353308](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729155353308.png) | ![image-20210729162957673](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729162957673.png) |
| 使用XML和Java代码混合   | ![image-20210729163645534](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210729163645534.png) | ![image-20210730152400107](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730152400107.png) |
| 开发自定义的View        | ![image-20210730152325017](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730152325017.png) | <video src="C:\Users\59501\Desktop\琪亚娜诱捕器.wmv"></video> |



# 三、布局管理器

## 1.什么是布局管理器

![image-20210730161736062](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730161736062.png)

## 2.常用的布局管理器

| 类型                      | 形态                                                         | 相关组件                                                     |
| ------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| RelativeLayout  相对——    | ![image-20210730162454162](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730162454162.png) | ![image-20210730163050798](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730163050798.png) |
| LinearLayout      线性——  | ![image-20210730163839169](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730163839169.png) | ![image-20210730164517802](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730164517802.png)【<LinearLayout>标记】![image-20210730164240081](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730164240081.png) |
| FrameLayout      帧——     | ![image-20210730200301306](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730200301306.png) | ![image-20210730200429425](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730200429425.png) |
| TableLayout        表格—— | ![image-20210731132059859](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210731132059859.png)![image-20210730201304239](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210730201304239.png) |                                                              |
| AbsoluteLayout   网格——   |                                                              |                                                              |
| GridLayout                | ![image-20210731211909517](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210731211909517.png)![image-20210731132025054](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210731132025054.png) | ![image-20210731132549689](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210731132549689.png)![image-20210731132219730](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210731132219730.png) |

## 3.布局管理器嵌套

![image-20210801163125045](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210801163125045.png)

### 1.布局管理器的嵌套原则

![image-20210801163752875](C:\Users\59501\AppData\Roaming\Typora\typora-user-images\image-20210801163752875.png)

