# DatePicker
项目中抽离的日期选择器

每当我们在做日期选择器的时候通常是用原生的日期选择器，但是远远满足不了项目需求，那么当我们自己去写的时候困难还是有的，今天为大家分享一下自定义的日期选择器，分享交流开心你我他！

## 项目效果图
<img src = "https://github.com/jinhuizxc/DatePicker/blob/master/screenshots/img1.jpg">
## GIF
<img src = "https://github.com/jinhuizxc/DatePicker/blob/master/screenshots/2.gif">

##  项目目录结构
<img src = "https://github.com/jinhuizxc/DatePicker/blob/master/screenshots/img2.jpg">

## 代码块-简要分析
主界面布局很简单，主要介绍选择日期的点击事件。

* 1.选择日期的点击事件：
```
 ll_selectedtime.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                final String[] str = new String[10];
                final ChangeDatePopwindow mChangeBirthDialog = new ChangeDatePopwindow(MainActivity.this);
//                mChangeBirthDialog.setDate("2017", "6", "20");
                mChangeBirthDialog.showAtLocation(frameLayout, Gravity.TOP, 0, 400);
                mChangeBirthDialog.setBirthdayListener(new ChangeDatePopwindow.OnBirthListener() {

                    @Override
                    public void onClick(String year, String month, String day) {

                        selectDate(Integer.parseInt(year), Integer.parseInt(month) - 1, Integer.parseInt(day));
                    }
                });
            }
        });
```
* 2.自定义的popwindow：
```
dsfsdf
```


- 如果你觉得以上对你有帮助，欢迎给个star!

## 关于我

## [简书](http://www.jianshu.com/u/e0d050a2120f)|[csdn](http://blog.csdn.net/jinhui157)




