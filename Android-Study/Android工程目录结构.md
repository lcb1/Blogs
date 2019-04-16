Android 项目目录结构  
=
* **总目录结构**  
![](https://upload-images.jianshu.io/upload_images/11025854-3ac5b335d6d98ea9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/363/format/webp)  
工程目录视图  
---
* .gradle 文件夹包含gradle工具的各个版本  
![](https://upload-images.jianshu.io/upload_images/11025854-29a2814ace16be46.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/249/format/webp)
>Gradle是一个基于Apache Ant和Apache Maven概念的项目自动化构建工具。它使用一种基于Groovy的特定领域语言(DSL)来声明项目设置，抛弃了基于XML的各种繁琐配置。——来自“百度百  
---
* .idea 文件夹包含了开发所需的各种环境  
![](https://upload-images.jianshu.io/upload_images/11025854-7fac5dcc0c402f96.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/352/format/webp)  
>IDEA 全称IntelliJ IDEA，是java语言开发的集成环境，IntelliJ在业界被公认为最好的java开发工具之一，尤其在智能代码助手、代码自动提示、重构、J2EE支持、Ant、JUnit、CVS整合、代码审查、 创新的GUI设计等方面的功能可以说是超常的。IDEA是JetBrains公司的产品，这家公司总部位于捷克共和国的首都布拉格，开发人员以严谨著称的东欧程序员为主。——来自“百度百科”
---
* app 文件夹存放build工具，项目依赖的库，项目源码  
![](https://upload-images.jianshu.io/upload_images/11025854-3c4414994ea257c7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/296/format/webp)  
*在这个 app 文件夹目录下同样有一个 build.gradle 文件，这个文件的设置只对本 app 有效，而上一层目录下的 build.gradle 对本项目有效。平时我们需要引用别人的开源库，就是在这里面添加的。*
![](https://upload-images.jianshu.io/upload_images/11025854-53f95588e6067f3d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1000/format/webp)  
