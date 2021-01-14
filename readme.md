- 2021.01.13
pink老师
html50%
css3 50%
h5c3提高10%
项目品优购电商网站20%


- goal目标


- 网页
1. 网页概念
    网站有多个网页组成
    网页构成网页
        网页包含图片，文字，链接等元素
        htm和html俗称HTML文件
        html语言
        html：超文本标记语言
        所谓超文本 1. 图片等 2. 超级链接文本 
    由网页元素组成


- 常用浏览器
1. 常用浏览器   ie和edge 火狐 谷歌chrome(blink) safari(webkit) opera等五大浏览器
2. 浏览器内核   负责拂去内容,整理讯息，计算网页的显示方式
3. web标准 w3c(万维网联盟)
    3.1 为什么需要web标准
    3.2 web标准的构成(面试)
        结构    网页元素html
        样式    css
        行为    javascript
    结构样式行为相分离


- html
1. 语法结构
2. 基本结构标签也叫骨架标签
3. 工具vscode
4. vscode插件安装
5. ! + tab 


- html常用标签
    4.1 语义标签
    4.2 标题标签    <h1> -> <h6> 依次变小   独占一行
    4.3 段落标签和换行标签
        <p>段落</p>
        <br />强制换行
    4.4 文本格式化标签
        粗体<strong></strong>
        斜体<em>建议</em>   <i></i>
        删除线<del>建议</del>   <s></s>
        下划线<ins>建议</ins>   <u></u>
    4.5 <div> division 和 <span>  没有语义就是盒子
        <div>独占一行   理解为大盒子
        <span>一行可以放多个span 理解为小盒子
    4.6 图像标签<img>
        标签属性src
        <img src = "图像url"/>
        img属性：
        alt：文字替换图片
        title: 提示文本
        width:高度
        height:宽度，改一个另一个等比例缩放
        border: 边框
    4.7 超链接标签
        1. 外部链接
        <a href="跳转地址" target=“目标打开方式” >跳转</a> 
        target   _self当前窗口的方式(默认)    _blank新窗口打开
        2. 内部链接    同一级直接文件名    使用路径即可
        3. 空连接<a href="#" /></a>
        4. 下载链接<a href="放要下载文件的地址" />下载文件</a>
        5. 网页元素的链接<a href="#" />图片文字等均可 <img src = "图像url"/></a>
        6. 锚点链接<a href="#maodian" />跳向目标id</a>  <h1 id="maodian"></h1>
    4.8 路径
        1. 目录文件和根目录
        2.  相对路径：相对html文件  相对路径用/    ../上一级    /下一级 
            绝对路径:              绝对路径用\     也可以用网络地址



- 注释
    <!-- 注释 -->  ctrl + /
    特殊字符
    空&nbsp;格
    <  &lt;
    >  &gt;
    其他的查就好


- html标签下
1. 表格标签 不是用来布局页面的，  而是 显示，展示数据
两行三列
<table  align="center" border="1"  cellpadding="20px" cellspacing="0" width="300px" height="250px">
    <thead>
        <tr>
             <!-- 表头会加粗居中 -->
            <th>表头1</th>
            <th>表头2</th>
            <th>表头3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="2">1.1</td>
            <td colspan="2">1.2</td>
            <td>1.3</td>
        </tr>
          <tr>
            <td>2.1</td>
            <td>2.2</td>
            <td>2.3</td>
        </tr>
    </tbody>
</table>
表格的属性在实际开发中不常用，后面会通过css设置
合并单元格
跨行合并rowspan="合并数量"
跨列合并colspan="合并数量"
记得删除多余单元格

2. 列表 整齐有序可以用来布局
    1. 无序列表
    <ul>
        <li>榴莲</li>
        <li>臭豆腐</li>
        <li>鲱鱼罐头</li>
    </ul>
    2. 有序列表
    <ol>
        <li>刘德华</li>
        <li>刘若英</li>
        <li>pink老师</li>
    </ol>
    3. 自定义列表
    <dl>
        <dt>关注我们</dt>
        <dd>新浪微博</dd>
        <dd>官方微信</dd>
        <dd>联系我们</dd>
    </dl>


3. 表单 ---为了收集用户信息
表单域--包含表单元素的区域
<form>定义表单域
</form>
表单控件--
提示信息
 <form action="demo.php" method="POST" name="name1">
        <!-- text 文本框 用户可以用来输入任何文字 -->
        <!-- maxlength最长字符 -->
        用户名：<input type="text" name="username" value="请输入用户名" maxlength="20"><br>
        密码：<input type="password" name="pwd"><br>
        <!-- radio 单选框 单选  必须有name属性才能设置单选 -->
        <!-- name 是表单元素名字 性别单选必须设置相同的那么才能实现单选 -->
        <!-- 单选按钮和复选框可以设置checked属性，即默认选中 -->
        性别：男<input type="radio" value="男" name="sex" checked="checked">
        女<input type="radio" value="女" name="sex" value="保密">
        保密<input type="radio" name="sex"><br>
        <!-- checkbox 复选框 多选 -->
        爱好：吃饭<input type="checkbox" value="吃饭" name="hobby"> 
        睡觉<input type="checkbox" value="睡觉" name="hobby">
        打豆豆<input type="checkbox" value="打豆豆" name="hobby"><br>
        <!-- 提交按钮提交表单的值 -->
        <input type="submit" value="免费注册">
        <!-- 重置按钮还原表单的初始状态 -->
        <input type="reset" value="重新填写"><br>
        <!-- 普通按钮 button 后期跟javascript一起用 -->
        <input type="button" value="获取短信验证码"><br>
        <!-- 文件域 使用场景 上传文件使用的 -->
        上传头像：<input type="file">
</form>

<lable>标签
<!-- 通过绑定id让可选择范围变大，增加用户体验 -->
<label for="user">username:</label><input type="text" name="" id="user">

<select>下拉标签
   籍贯:<select name="" id="">
            option 至少有一个
            <option value="">北京</option>
            <option value="">上海</option>
            <option value="">深圳</option>
            <option value="" selected="selected">火星</option>
        </select><br>

文本域<br>
<textarea name="" id="" cols="30" rows="10">pink 老师</textarea>




- CSS
