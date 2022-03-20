* 将各段格式化并放入li中：选中文字；shift+ctrl+p 输入wrap自动换行；输入emmet wrap缩写包围个别行（按需要选择包围）；输入ul>li*（或者ol）
* 使用正则表达式：选中编辑-替换，选中"*"(使用正则表达式)，输入\[\d+\] ，点击全部替换，再次点击 " *"清空。
* <font color="red">不知道怎样使用插件克在ctrl+shift+p中打开查找</font>
* <font color="red">插件设置：ctrl+shift+p，输入setting(ui)，输入插件名(format on save)</font>
*  多选的快捷编辑：alt选中
*  引用本地图片：将图片放入vs code的imges文件夹，img加路径
```
<img src="imges/1.jpg" alt="图一">
```
* 目录：导航nav
```
<nav>
    <ol>
        <li><a href="#events">主要事件</a></li>
    </ol>
</nav>
<h2 id="events">
```
* 兼容手机<meta name="viewport">完整代码
```
  content="width=device-width, 是手机显示宽度
  initial-scale=1.0", 是画面缩放比例
  minimum-scale=1.0, 最小缩放比例
  maximum-scale=1.0, 最大缩放比例
  user-scalable="no", 用户不准缩放
  <style>
    img {
        max-width: 100%;
        }
   </style>
```
* 用WIFI调试手机：
    1. 让手机和电脑处于同一wifi
    2. 手机可以直接用IP和端口访问电脑
    3. 用哪个IP？hs -c-1给出的IP全试一遍
    4. 用border调试法调试css
    5. cConsole.js调试js
* 用Chrome远程调试
    1. 搜索Chrome远程调试（-csdn）
    2. 按教程做 

* 部署到github page里(复习VScode提交代码到github)
    1. github新建库，分别复制or push an...的代码
    2. 终端
    ```
    git status
    gst
    ga .
    gc (写明提交原因并保存)
    分别粘贴or push an...的代码
    ```
    3. github点settings，选中github pages，选中source中的master branch，再点击所给出的地址加路径
    4. 预览地址（放在醒目位置）：在库中找到about设置按钮，description写预览地址：，website复制自制的网站的地址，点save
