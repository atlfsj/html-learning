* <font color="red"> VS Code里打开超链接：</font>
1. 用http-server打开，终端安装server，打开链接路径后接/文件名再打开
```
yarn global add http-server
http-server -c-1 (hs -c-1)
```
2. 用parcel打开，终端安装，打开
```
yarn global add parcel
parcel a-href.html (文件名)
```
* a标签的href取值：
1. 网址：
   1. https://google.com
   2. http://google.com（不安全）
   3. //google.com(无协议)浏览器打开页面后，打开检查，点击Network，选中Preserve log，再点链接在name会发现http在跳转（写网址就用这个）
2. 路径：
   1. /a/b/c.html (当加了http时文件将不是文件，http显示不安全，此时根目录“/”不是硬盘的而是打开位置。如果用双击打开html前缀将变成文件，再点c.html将从D盘根目录，找不到文件。)
   2. （./）a/b/c.html(相对路径)
3. 伪协议：
   1. javascript:代码(空的用来执行"无操作,不刷新"的链接)
```
<a href="javascript:alert(1);">JavaScript</a>
<a href="javascript:;">空的JavaScript</a>
<a href="#;">JavaScript</a> 
```
   2. #id 跳转到指定标签
```
<p id="xxx">123</p>
<a href="#xxx">查看xxx</a>

```
   3. mailto:邮箱
```
<a href="mailto:aaaaaaaaaaaaaaaaaa">发邮件给xxx</a>
```
   4. tel：手机号
```
<a href="tel:111111111111111111111">打电话给xxx</a>
```
* a标签的target取值：
  1. _blank 在新页面打开
  2. _top 在当前页面的最上面的窗口打开
  3. _parent 在当前页面所在的上一层窗口打开
  4. _self(默认) 在当前页面（窗口）打开
  5. window的name：在同一页面显示
```
    <a href="https://google.com" target="xxx">google</a>
    <a href="https://baidu.com" target="xxx">baidu</a>
```
  6. iframe的name：在指定窗口显示(goodbai网页)
```
<a href="//google.com" target="xxx">google</a>
<a href="//baidu.com" target="yyy">baidu</a>
<iframe src="" name="xxx"></iframe>
<iframe src="" name="yyy"></iframe>
```
* <font color="red">table的正确用法:</font>(可没有head，foot，顺序可调)
```
    <table>
        <thead>
            <tr>
                <th></ht>
                <th>英语</th>
                <th>翻译</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>2</td>
                <td>typer</td>
                <td>超级</td>
            </tr>
            <tr>
                <td>3</td>
                <td>target</td>
                <td>目标</td>
            </tr>
            <tr>
                <td>4</td>
                <td>reference</td>
                <td>引用</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>空</td>
                <td>空</td>
                <td>空</td>
            </tr>
        </tfoot>
    </table>
    ```
    table的样式：
```
    <style>
        table{
            width: 600px;
            table-layout: auto;
            border-spacing: 20px;
            border-collapse: collapse;
        }
        td,
        th{
            border: 1px solid blue;
        }
    </style>
```
