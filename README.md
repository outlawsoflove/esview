# 此项目已暂停开发

#Esview是一款拖拽组件生成vue代码的工具。
#包含拖拽生成页面、页面管理、组件管理等功能。
#前端采用vue和iview，生成的代码必须安装vue和iview才能使用，
#后台采用java（springboot）作为持久层，保存生成的页面、创建的组件。

#编译报错 [参考连接](https://blog.csdn.net/phlr5/article/details/83780628)

<p align="right">
  <a href="https://github.com/furioussoul/soul-esview/blob/master/ui/README-ch.md">中文</a>
</p>
<p align="center"><a href="#">Esview</p>



<p align="center">
  <a href="https://www.npmjs.com/package/esview"><img src="https://img.shields.io/npm/l/esview.svg" alt="License"></a>
   <br>
</p>
  

# Introduction
Esview is a vue page code generator based on iview-ui.  

You can get .vue file code by dnd components on esview.

Also you can customize your own draggable components.

![QQ图片20171027113639.png](http://chuantu.biz/t6/121/1509463255x2890191685.gif)

# Online Demo

http://47.97.220.227:9090/#/

# <a href="https://github.com/furioussoul/esview/blob/master/ui/doc/SUMMARY.md">Doc</a>

1 generate code:

You can assemble page by dragging components on the left side and drop them into the middle section.

Click 'code' on the action bar to see generated code and click copy to get code.

2 customize own draggable components:

You should know how to register components on vue,so this is the first step,

second step is to go to page 'Develop->ManageControl',copy code of 'Div',

and modify exports.* according to your own components,click save and you will see it on assemble page.


# Install
frontend: Esview uses vue and iview，so the code generated must rely on vue and iview.

backend: Java（springboot）,so you must install jdk firstly.

database:mysql,the sql file is on directory 'server',named 'soul-esview.sql'.

# Theory
How to implement dnd：I use html api，the code is in dnd.js .

How to generate code：The data structure behind assembled page is a syntax tree,

I use recursive downward parsing to get the final .vue code.  

# License
[MIT](https://opensource.org/licenses/MIT)

Copyright (c) 2017-present,  SunZhengJie(Furioussoulk)
