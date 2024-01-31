# [HTML](https://www.runoob.com/html/html-quicklist.html)
## Emphasis
1) \<meta charset="UTF-8">防止中文变乱码
2) 浏览器在显示 HTML 时，会省略源代码中多余的空白字符（空格或回车等）。
3) [缩写](https://www.runoob.com/try/try.php?filename=tryhtml_abbr)
4) 锚点链接：在同一页面内创建内部链接。要创建锚点链接，需要在目标位置使用 <a> 元素定义一个标记，并使用#符号引用该标记。例如：
```html
<a href="#section2">跳转到第二部分</a>
<!-- 在页面中的某个位置 -->
<a name="section2"></a>
```
4') 从另一个页面创建一个链接到"有用的提示部分(id="tips"）"：  
```html
<a href="https://www.runoob.com/html/html-links.html#tips">
访问有用的提示部分</a>
```

## Summary  

1）\<head> 元素包含了所有的头部标签元素。在\ <head>元素中你可以插入脚本（scripts）, 样式文件（CSS），及各种meta信息。  
可以添加在头部区域的元素标签为: \<title>, \<style>,\ <meta>, \<link>, \<script>, \<noscript> 和 \<base>。
META 元素通常用于指定网页的描述，关键词，文件的最后修改时间，作者，和其他元数据。  
元数据可以使用于浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他Web服务。  
eg:
为搜索引擎定义关键词:
> \<meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript">

为网页定义描述内容:
> \<meta name="description" content="免费 Web & 编程 教程">

定义网页作者:
> \<meta name="author" content="Runoob">

每30秒钟刷新当前页面:
> \<meta http-equiv="refresh" content="30">
