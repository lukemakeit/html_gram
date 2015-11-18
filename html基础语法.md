##元信息标记meta
meta元素提供的信息**不显示在页面中**，一般用来**定义页面信息的说明、关键字、刷新等**。在 HTML 中，**meta标记不需要设置结束标记，在一个尖括号内就是一个 meta 内容**。在一个HTML页面中可以有多个meta元素。 meta 元素的属性有name和http-equiv ，其中 name属性主要用于秒数网页，以便于搜索引擎的查找、分类。   

- 设置页面关键字——在搜索引擎中，检索信息都是通过输入关键字来实现的。关键字在浏览时候看不到，但是可以提供搜索引擎使用。当搜素引擎搜索网站时，如果网页中包含了关键字，就可以在搜索出来。  
语法：**< meta name="keywords" cotent="输入具体的关键字">**   
- 页面说明信息 ——也是为了便于搜索引擎的查找，用来说明网页的内容，页面说明在网页中也不显示:**< meta name="description" content="设置页面说明">**  
- 定义编辑器：**< meta name="genertator" content="编辑软件的名称">**
- 设置作者信息：**< meta name="author" content="作者姓名">**
- 设置网页文字以及语言：**< meta http-equiv="content-type" content="text/html;charset=字符集类型">**  
在该语法中，http-equiv用于传送HTTP通信协议的标头，而在content中才是具体的属性
值。charset用于设置网页的内码语系，也就是字符集的类型，国内常用的是GB码，charset往往设置为gb2312，即简体中文
- 设置网页的定时跳转——使用<meta/>标记可以使网页在经过一定时间后自动刷新，这可通过将http-equiv属性值设置为refresh来实现。content属性值可以设置为更新时间。（在浏览网页时经常会看到一些欢迎信息的页面，在经过一段时间后，这些页面会自动转
到其他页面，这就是网页的跳转。）   
语法：**< meta http-equiv="refresh" content="跳转时间；url=跳转到的地址">**  
**亲自测试了一下，他是跳转到指定的html上面去**   
![meta_refresh](meta_refresh.png)  
##网页的主体标记body
所有body中的标签放置在一起，表明它对网页中所有未单独设置的元素起作用。 
 
-  网页背景颜色bgcolor——在该语法中的body就是页面的主体标记，bgcolor的值可以是一个已命名的颜色，也可以是十六进制的颜色值。  
语法：**< body bgcolor="背景颜色">**
-  设置网页背景图片background  
语法：**< body backgroud="图片地址">**  
-  文字颜色text  
语法：**< body text="文字颜色" >**
-  链接文字属性link——在默认情况下，浏览器以蓝色作为超链接文字的颜色，访问过的文字则颜色变为暗红色。可以通过link参数修改链接文字的颜色。  
语法：**< body link="颜色">——设置默认的链接颜色**  
	 **< body alink="颜色">——设置访问时的链接颜色**  
	 **< body vlink="corlor">——设置访问后的链接颜色**  
-  边距margin——单位：**像素**  包括上边距(topmargin)和左边距(leftmargin)  
语法：<body topmargin="400" leftmargin="500">   
-  页面注释标记：< ! --注释内容-->
##文字与段落标记
-  标题
	-  标题字：< h1> < h2> < h3> < h4> < h5> < h6>级别依次减少
	-  标题字对其属性align  
	语法：**<align=对齐方式> 包括：left center right**  
	例如：< h2 align="left">2 级标题左对齐</h2>  
-  正文内容  
	-  字体属性face——默认字体是宋体
	语法：**< font face="字体样式">...</font>**  
	-  字号属性 size，还可以使用"+3" "-4"等语法
	-  颜色属性 color 
	-  粗体标记  
	语法：< b> < /b> or < strong> < /strong>
	- 斜体标记：< i>< /i> or < em> < /em> or < cite> < /cite>
	- 上标标记 sup——< sup>< /sup>   
	例如：a< sup>2</sup>+b< sup>2< /sup>
	- 下标标记 sub——< sub>< /sub>
	- 大号字小号字< big> < small>
	- 下划线标记——< u>< /u>
	- 段落标记< p> < p>
	- 换行标记 < br>
	-  不换行标记 < nobr>
	-  水平线 < hr>
	-  水平线宽度 < hr width="500">
	-  水平线高度 < hr size="高度">
	-  水平线去掉阴影< hr noshade>
	-  水平线颜色< hr color="#CC6600">
	-  对齐方式< hr align="left/right">
	-  插入空格 & nbsp;
	-  特殊符号:  
	![special](special.png)   

## 图像格式  	
- img元素属性  
![img](img.png)  
提示：alt——当**鼠标放在图片上时给出提示**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;图像的宽度和高度**width、height是用来限制图像大小**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**图像的边框border就是加边框咯**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**垂直边距vspace——用来调整图像和文字的垂直边距**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**水平边距hspace——用来调整图像和文字的水平边距**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**图像的排列align——bottom、top、middle、left、center、right不懂！！！！**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**图片的超链接——和文字的超链接方法类似，使用< a>标签完成,只需要将标签放在< a>< /a>之间就可以,如:< a href="链接地址">< img src="图像的地址">< /a>**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**图像热区链接——多个热点区域使用usemap  不懂！！！**  
## 使用列表
- 有序列表：  
	< ol type="a" start="2">  
	< li>星期一< /li>  
	< li>星期二< /li>  
	< /ol>  
type的值：  
![liebiao_type](liebiao_type.png)  

-   无序列表类型type：  
< ul type="符号类型">  
< li>列表项< /li>  
< li>列表项< /li>  
< /ul>  
type的值：  
![ul_type](ul_type.png)  
-  定义列表标记  
< dl>  
< dt>定义条件< /dt>  
< dd>定义描述< /dd>  
< /dl>
## 表格  
< table width="表格宽度"  &nbsp;&nbsp;height="表格高度" &nbsp;&nbsp;align="left/center/right" &nbsp;&nbsp;border="" &nbsp;&nbsp;bordercolor="">  
< caption>表格标题< caption>    
< th> 表头也就是列名< /th>  
< tr>  
< td>< /td>  
< /tr>  
< tr>    
< td>  < /td>  
< td>  < /td>  
< /td>  
< /table>  

-  table——cellspacing:内框宽度（单元格之间的间距）
-  table——cellpadding:文字与边框间距
-  table——bgcolor表格背景颜色（当然是全部表格，不是单元格）
-  table——background表格背景图像（值是图像地址）
-  tr（行）属性——height bordercolor bgcolor background align(水平对齐：left center right ) valigh(垂直：top middle bottom)  
-  td(单元格)属性——width height **colspan（水平跨度） rowspan(垂直跨度)**  align valign bgcolor bordercolor bordercolorlight(亮边框)  bordercolordark（暗边框）background  
-  表格的结构(一个一个单元格去修改表的属性或者一行一行修改太麻烦了，所以需要表格的结构)：
	-  表首标记< thread bgcolor="" align="">< /thread>
	-  表格主体< tbody bgcolor="" align="">< /tbody>
	-  表尾标记< tfoot>< /tfoot>
## 超链接

-  简单的内部链接< a href="链接地址"> ...< /a>(真不知道这用来干嘛)
-  target——目标窗口的打开方式：  
![href_target](href_target.png)  
尝试了一下，真不知道\_sef、\_top、\_parent有啥区别!!!  
-  锚点链接< a name='锚点名称'>< /a>  **< a href="#锚点名称"> < /a>** 例如:
><pre><code> < p>
    < a href="#hello">打招呼< /a>
  < /p>
  < p>
    < a name="hello">大家好，我叫luke。还请大家多多关照！< /a>
</code></pre>
链接到其他页面的锚点：   
**< a href="链接的文件地址#锚点名称">...< /a>**   

-  外部链接——**< a href="http://....">......< /a>**
-  链接到e-maill——**< a href="mailto:邮件地址">...< /a>**
-  链接到FTP(文件传输协议):大部分的FTP网站需要一个用户名和密码来进入网站。在FTP网站的链接内如果包含用户名和密码，这些信息对任何浏览源代码的人都是公开的。  
**< a href="ftp://ftp地址">...< /a>**
-  链接到telnet:telnet常常用来登录一些BBS网站，也是一种远程登录方式。  
**< a href="telnet://地址">...< /a>**  
-  下载文件——**< a href="文件路径">...< /a>**  
如果是.doc文件等，那么会产生预览功能。如果是.tar、.zip则会下载。
##多媒体
-  设置滚动效果——< marquee>....< /marquee>
	-  滚动方向——dirction:up/down/left/right
	-  滚动方式——behavior
![marquee_behavior](marquee_behavior.png)  
alternate:就是那种左右左、上下上的意思。碰到边界就返回...
-  滚动的速度scrollamount(以像素为单位)
-  滚动延迟scrolldelay：时间间隔的单位是毫秒。如果时间设置过长的的话会出现走走停停的效果！
-  循环次数loop，默认是无限循环，loop可以控制次数；
-  滚动范围width和height，以像素为单位；
-  滚动的背景颜色bgcolor;
-  空白空间hspace、vspace——使用hspace和vspace可以设置它们之间的空白空间；
-  插入flash/音频/视频——**< embed src="文件地址" width="" height="">...</embed>**
-  背景音乐bgsound（文件可以是avi、mp3等格式）——**< bgsound src="文件地址">**
	-  loop——循环次数
-java Applet  