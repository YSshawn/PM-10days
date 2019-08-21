# 如何转行产品经理（五）原型设计工具Axure
Axure是产品经理最常用的原型设计工具。最新的Axure RP 9 新增了对手机端原型的设计支持。好了废话不多说，下面介绍Axure的使用方法。
<br/>

### Axure功能区简介
![功能区](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/2980541-c1aacb4a97333690.jpg)
<br/>

Axure功能区主要分四大块：

1）位于最上面的是导航菜单和工具区。有点类似于word。

2）位于最左边的是页面和元件库。主要展示原型中用到的全部页面，和设计原型时使用的元件。

3）中间一大片空白区域为设计原型时的工作区。所有的原型展示和交互都在这里完成。

4）位于最右边的是样式与交互设计区。主要负责原型的样式和交互动作。
<br/>

PS：左右两边的功能区是可以拖拽摆放的。可以根据自己的喜好进行摆放。
<br/>

![拖动演示](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/1.webp)
<br/>

### 原型设计实战·百度首页
![百度首页](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/2.webp)
<br/>

接下来，我们用Axure制作百度首页的原型，我们只制作右上方的导航和中间的搜索框区域，下面的二维码和页面footer不做（因为思路和上面两个一样，只是一个体力工作）。
<br/>

**文末附实战案例的RP文件下载地址**
<br/>

### [页面展示与布局]

###### 1、页面设置

1）鼠标停留在Axure功能键时，都会有功能提示，默认已经有一个页面了，我们将他的名字改为“百度”（如果需要新增页面时，点击上面的加号）。
<br/>

2）选择样式，将设备栏Auto选择到Web，宽度调到1920（现在大部分电脑是1920*1080的分辨率），页面排列选择居中，Axure默认是居中的，这里就不用管了。

![样式设置](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/3.webp)
<br/>
<br/>

###### 2、添加导航按钮

1）导航是由8个带下划线的文字按钮和1个蓝底白字的按钮组成的。我们先拖拽文字元件到工作区。双击修改文字，并添加下划线。为了方便后续工作，我们将文字区域设置为70*35并上下左右居中。
![样式设置](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/4.webp)
<br/>

2）按住CTRL拖拽元件可实现元件的快速复制，如下图。我们迅速设置好其他7个文字按钮（Axure9带有智能标尺功能，元件离着较近时会显示原件之间的距离，我们让2个按钮紧靠即可）。

![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/5.webp)
<br/>
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/6.webp)
<br/>

3）最后拖入一个带有背景的按钮，依然设置为70*35并紧靠前一个文字按钮，设置好文字和背景的颜色。

![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/7.webp)
<br/>

4）摆放导航栏。全选导航按钮，将导航按钮置于页面右上角合适位置。

![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/8.webp)
<br/>
<br/>

###### 3、添加搜索区

1）添加百度logo，拖动logo到页面中部，软件会自动识别居中，调整高度放置。
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/9.webp)
<br/>

2）拖入输入框元件和按钮元件（这里用的矩形）。调整尺寸和颜色。
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/10.webp)
<br/>

想要改变输入框线条颜色，需要先选中输入框，然后点击切换颜色。如下图
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/11.webp)
<br/>
<br/>
<br/>

### 【交互设计】

###### 1、相机（基础动态面板交互）

1）添加已经下载好的相机icon（下载地址为阿里巴巴矢量图标库）并调整好大小，右键转为动态面板，并添加面板状态2（动态面板每一个状态都是一个独立的展示页面，可以通过交互事件控制动态面板要展示哪个内容）。如下图。
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/12.webp)
<br/>

2）为动态面板添加交互。鼠标移入显示面板2，鼠标移除显示面板1。下图2为预览效果。
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/13.webp)
<br/>
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/14.webp)
<br/>

###### 2、文字按钮（基础页面跳转交互）

1）选中新闻按钮，添加点击事件，在新窗口打开链接http://news.baidu.com/
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/15.webp)
<br/>

2）其他几个按钮，操作基本相同，这里不再重复演示。
<br/>

###### 3、百度一下（高级参数，前期可不必掌握）

1）实现点击百度一下时，根据输入的内容跳到百度并查询

2）依然是配置跳转链接，但是要点击fx设置参数
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/16.webp)
<br/>

3）参数前面是百度的搜索链接格式，后面是我们自定义的局部变量，而变量内容为输入框输入的内容。
![图片](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/17.webp)
<br/>
<br/>

演示地址（请用PC打开）：http://www.wulihub.com.cn/go/Jm5oYJ/start.html#id=a8gjac&p=%E7%99%BE%E5%BA%A6
<br/>
<br/>

**原型下载：公众号回复“百度”**

**Axure下载：**
公众号里回复“Axure”，获取Axure安装程序及汉化程序等。


**[关于Axure的几点学习建议]**

1）勤加练习，多找一些web或APP进行临摹，由浅入深

2）每个元件都拖出来看一下，看看有何不同

3）每个元件都添加一下事件，看看有何不同

4）每个事件都使用一下，看看有何不同

5）上面的原型文档中，附送了一份正版的金乌Axure7的视频教程。虽然Axure7和Axure9有一些不同，但是A7掌握的话，A9完全不在话下。



<br/>
<br/>
<br/>
<br/>
<br/>

转自公众号：岩杉Shawn

![二维码](https://raw.githubusercontent.com/YSshawn/PM-10days/master/pic/2980541-065cc3b5b0ab390b.jpg)
