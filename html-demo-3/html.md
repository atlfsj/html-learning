* img标签
  1. 属性：
     1. alt：在图片加载失败时显示的文字
     2. width/height只写其中一个另一个会自适() 
  2. 事件(id只在测试时用)：查看图片是否加载成功（console），404图片(要将展示的图片放入VS code) 
     1. onload:图片加载成功(script必须在下)
     2. onerror:图片加载失败
     ```
    <img id="xxx" width="400" src="dog.png" alt="一只狗">
    <script>    
        xxx.onload = function() {
            console.log("图片加载成功")
        }
        xxx.onerror = function() {
            console.log("图片加载失败")
        };
        xxx.src = "/404.png";
    </script>
     ```
  3. 响应式：:铺满页面(适应手机)
    ```
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }   
        img {
            max-width: 100%;
        }
    </style>
    ```
* form标签：
    1. method:控制get/post请求，
    2. autocomplete:自动完成填充
    3. target:与a标签的相同 
    ```
    <form action="/xxx" method="post" autocomplete="on" target="a">
    ```
    4. action:打开位置（后端）  <font color="red">   
    5. value：设置文字(button与input区别在于input不能加效果,button连图片也行)        </font>
    ```
    <input type="submit" value="搞起">
    ```
    6. button：按钮。不写type默认为submit
    ```
    <button type="submit"><strong>搞起</strong></button>
    ```
* input标签：让用户输入内容
    1. 属性:类型type:button/checkbox/email/file(multiple选择多文件)/hidden/number/password/radio/search/submit/tel/text
       其他:name(用于分组)/autofocus/checked/disabled/maxlength/pattern/value/placeholder
     ```
        <form action="/xxx" method="post" autocomplete="on" target="a">
        <input name="username" type="text">
        <input type="submit" value="搞起">
        <button type="submit"><strong>搞起</strong></button>
        <hr>
        <input type="color">
        <hr>
        <input type="password">
        <hr>
        <input name="gender" type="radio">男
        <input name="gender" type="radio">女
        <hr>
        <input type="checkbox" name="hobby">唱
        <input type="checkbox" name="hobby">跳
        <input type="checkbox" name="hobby">rap
        <input type="checkbox" name="hobby">篮球
        <hr>
        <input type="file">
        <input type="file" multiple>
        <hr>
        </form>  
    ``` 
    2. textarea文本框(无resize则框的大小可随意调)
    ```
    <textarea style="resize: none; width: 50%; height: 300px;"></textarea>
    ```
    3. option选项框
    ```
    <select>
    <option value="">-请选择-</option>
    <option value="1">星期一</option>
    <option value="2">星期二</option>
    </select>
    ```
    4. 事件：onchange/onfocus/onblur
    ```
    <input name="username" type="text" required>
    ```
    5. 验证器：HTML5新增功能
    6. 注意事项：
 * 一般不监听input的click事件
 * form里面的input要有name
 * form里面要放一个type=submit才能触发submit事件

