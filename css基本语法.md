##CSS
###创建和插入
-  外部样式表
<pre><code>< head>  
< link rel="stylesheet" type="text/css" href="mystyle.css" />  
< /head></code></pre>
注意：  
**< link>是放在< head>中**；  

-  内部样式表   
<pre><code>< head>
< style type="text/css">
	hr {color: red;}
	p {margin-left: 20px;}
	body {color: red; }
< /style>
< /head></code></pre>

-  内联样式（谨慎使用）  
<pre><code>< p style="color: sienna; margin-left: 20px">
	This is a paragraph
< /p></code></pre>
###选择器
