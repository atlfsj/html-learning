# html重点标签
* style写在head里不显示，写在body里有效果且显示
* 不到万不得已不要使用id，因为他不唯一不报错且有忌讳（控制台中window所有的属性不能用），故一般用class
* js优先级>style>css
* 头部和页尾header footer
* div用来划分内容，如：header，div，footer
* 段落和章节都用section
* dua
* 旁支
```
<aside></aside>
```
* 使用户可直接编辑
```
<style contenteditable>
```
* 隐藏内容
```
<header hidden>顶部广告</header>
```
* 省略文字
```
text-overflow: ellipsis;
```
* 鼠标悬浮时显示省略的文字
```
<header id="xxx" style="border: 10px solid green;" title="完整内容">
 ```
* 网页无鼠标操作, "0"是最后一个访问，"-1"不访问，其余顺序访问
```  
<h1 tabindex="1">文章标题</h1>
```
* 版权标志
```
<footer tabindex="0">&copy; 饥人谷版权所有</footer>
```
***
***
***
* 默认样式：css未出现时html有自己的样式，在浏览器中打开检查，在elements中选中要改的代码，在element.style可更改样式

* 清除并修改默认样式
```
<style>
      *{margin: 0;padding: 0;box-sizing: border-box;}
      *::after, *::before{box-sizing: border-box;}
      h1,h2,h3,h4,h5,h6{font-weight: normal;}

      a{color: inherit; text-decoration: none;}
      ul, ol {list-style: none;}
      table{border-collapse: collapse; border-spacing: 0}
      pre{font: inherit;}
  </style>
  <style>
      h1{font-size: 48px;}
      h2{font-size: 36px;}
  </style>
```
常见的CSS reset
1. [方老师常用](https://gist.github.com/FrankFang/df5e57a0799823ed89a960a642b3a1e2)
2. 找大厂首页，打开浏览器开发者工具，复制粘贴到自己的项目，命名为reset.css

* 自定义格式和代码
```
    <pre>
    <code>
var a = 1
console.log(a)    
    </code>
    </pre>
```
* 网站连接,taget=blank表示新窗口打开，不加会在当前页面打开
```
<a href="http://qq.com" target="_blank_">qq</a>
```
* 引用（加block表示换行）
```
欧阳修说过：<blockquote>三上：马上，厕上，枕上</blockquote>
```
