***
11月30日
***
# 1. 核心技术
- HTML5
- CSS3
- JavaScript

### Web是什么?
- Web标准是由W3C组织和其他标准化组织制定的一些列标准的集合
- Web标准的构成:主要包括结构(structure)、表现(performance)、和行为(behavior)三个方面

### 常用的网站
- [W3Schools](https://www.w3schools.com/)
- [MDN Web Docs](https://developer.mozilla.org/zh-CN/)

## 1.1 HTML
Hyper Text Markup Language(超文本标记语言)

```html
  <!DOCTYPE html>
```
- 文档类声明,告诉浏览器用的是哪个版本的HTML
- 必须在第一行
- 这不是一个标签!

```html
  <html lang="en"> </html>
```
- HTML的语言是应为, en为英文, zh-CN是中文

```html
  <meta charset="UTF-8" />
```
- 储存各种文字
- UTF-8 万国码
— GB2312 简体中文
- GIG5 繁体中文
- GBK 包含了简体中文和繁体中文

```html
  <meta name="" content="" />
```
- `name`可以为keyword,也可以为内容描述
- `content`可以为测试关键字,也可以为测试描述

```html
  <body> </body>
```
- 用来组成HTML的骨架

```html
  <title> </title>
```
- 页面名称的标签

## 1.2 HTML编辑工具
- 记事本
- Sublime
- VS Code
- Atom
- WebStorm
- Dreamweaver

## 1.3 HTML基本标签
```html
  <h1> </h1>
  <h2> </h2>
  <h3> </h3>
  <h4> </h4>
  <h5> </h5>
  <h6> </h6>
```
- 标题标签
- 字体变粗, 字号变大
- 一个标题占一整行
- 一共6级

```html
  <p> </p>
```
- P标签
- 段落标签
- 段落之间有空行
- 会根据浏览器窗口自动换行

```html
  <br />
```
- 换行标签
- 遇到该标签会换行

```html
  <hr />
```
- 分割线标签

```html
  <strong> </strong>
```
- 强调文本
- 文字加粗
- 推荐使用

```html
  <b> </b>
```
- 文字加粗

```html
  <em> </em>
```
- 强调文本
- 文字斜体
- 推荐使用

```html
  <i> </i>
```
- 文字斜体

```html
  <ins> </ins>
```
- 强调文本
- 下滑线标签
- 推荐使用

```html
  <u></u>
```
- 文字添加下划线

```html
  <del> </del>
```
- 删除标签
- 推荐使用

```html
  <div> </div>
```
- 没有语义
- 独占一行
- 块元素
- 用来布局

```html
  <span> </span>
```
- 没有语义
- 一行多个
- 行内元素/內联元素
- 用来布局

```html
  <img src="" alt="" title="" height="" width="">
```
- 图像标签
- `src` 用来放图片的路径
- `alt` 在图像不显示时显示的替代文字
- `title` 当鼠标悬停在图片上时会显示的提示文本
- `width` 设置图像的宽度, `height` 设置图像高度; 通常只需要设置一个,另外一个会根据图像大小自动调整,否则会失真
- img属性以key-value形式呈现

```html
  <a href="" target=""> </a>
```
- 链接标签
- `href` 用来添加链接路径
- `target`用来指明链接在哪个窗口打开
- 页面间链接, 不同页面之间的跳转
- 锚链接, 同一页面快速定位, `href` 添加 `# + 目标标签的id`
- 功能性链接, 如:电子邮件、QQ、MSN、Facebook
Ins等

### 1.3.1 常见图像格式
- JPG
- GIF
- PNG
- BMP

### 1.3.2 注释以及特殊符号

```html
  &nbsp; 空格符 ` `
  &lt; 左尖括号 `<`
  &gt; 右尖括号 `<`
  &copy; 版权符号 `@`
  &quot; 引号 `"`
```

## 1.4 列表
```html
  <ul>
    <li> </li>
    <li> </li>
    <li> </li>
  </ul>
```
- 无序列表(最常用)
- `ul`标签下必须是`li`标签
- 没有顺序
- 每个`li`标签独占一行
- 一般用于无序类型的列表,如导航、侧边栏、有规律的图文组合模块

```html
  <ol>
    <li> </li>
    <li> </li>
    <li> </li>
  </ol>
```
- 有序列表
- 默认`li`标签项前面有顺序标记
- `ol`标签下必须是`li`标签
- 每个`li`标签独占一行
- 一般用于排序类型的列表

```html
  <dl>
    <dt>
      <dd> </dd>
    </dt>
    <dt>
      <dd> </dd>
      <dd> </dd>
    </dt>
    <dt>
      <dd> </dd>
      <dd> </dd>
      <dd> </dd>
    </dt>
  </dl>
```
- 定义列表
- `dl`标签下必须是`dt`标签和`dd`标签
- `dt`标签和`dd`标签独占一行

## 1.5 表格
```html
  <table cellpadding="" cellspacing="">
    <tr>
      <th>name</th>
      <th>age</th>
      <th>gender</th>
    </tr>
    <tr>
      <td>Albert</td>
      <td>25</td>
      <td>Male</td>
    </tr>
    <tr>
      <td>Marry</td>
      <td>24</td>
      <td>Female</td>
    </tr>
  </table>
```
- 第一个`tr`标签中通常为`th`标签
- `th`标签为表格的标题,字体会加粗且居中
- `tr`标签为表格行标签
- `td`标签为表格列标签
- `cellpadding`
- `cellspacing`

## 1.6 Form
- 块元素, 用于采集和提交信息
```html
  <form action="" method=""> </form>
```
- `action`将指示form提交的位置
- `method`将指示form是提交还是获取, `get`为获取, `post`提交
- 在实际网页开发中通常采用`post`的方式提交表单数据

## 1.7 Input
```html
  <input type="text" name="" value="">
```
- input属性

| 属性 | 说明 |
| - | - |
|`type`|制定元素的类型.常见的为: `text`、`password`、`checkbox`、`radio`、`submit`、`reset`、`file`、`hidden`、`image`、和`button`, 默认为`text`|
|`name`|制定表单元的名称|
|`value`|元素的初始直. `type`为`radio`的时候必须指定一个值|
|`size`|指定表单元的初始宽度.当`type`为`text`或`password`时,表单元的大小以字符为单位.对于其他类型,宽度以像素为单位|
|`maxlength`|`type`为`text`或`password`时,可以输入的最大字符数|
|`checked`|`type`为`radio`或`checkbox`时,指定按钮是否被选中|
|`placeholder`|输入框中的提示字符|
|`readonly`|只读|
|`disable`|禁用|
|`autocomplete`|自动补全, `on` 表示开启, `off` 表示关闭|
|`required`|表示内容不能为空,否则将无法提交表格|

## 1.8 列表框
```html
  <select name="" size="">
    <option value="" selected=""></option>
    <option value=""></option>
  </select>
```
- 下拉菜单
- `name`为列表框名称
- `size`列表框显示的选项数,默认为1
- `<option> </option>`选项标签,下拉菜单中的选项
- `selected`表示下拉菜单中的默认被选中的选项

## 1.9 HTML元素及分类
### 1.9.1 块元素
```html
<address> <article> <aside> <blockquote> <canvas> <dd> <div>  <dl> <dt> <fieldset> <figcaption> <figure> <footer> <form> <h1> <h2> <h3> <h4> <h5> <h6> <header> <hr> <li> <main> <nav> <noscript> <ol> <p> <pre> <section> <table> <tfoot> <ul> <video>
```

### 1.9.2 行内元素
```html
<a> <abbr> <acronym> <b> <bdo> <big> <br> <button> <cite> <code> <dfn> <em> <i> <img> <input> <kbd> <label> <map> <object> <output> <q> <samp> <script> <select> <small> <span> <strong> <sub> <textarea> <time> <tt>
```

### 1.9.3 HTML常用结构元素
```html
<header> <footer> <section> <article> <aside> <nav> <details> <figcaption> <figure> <mark> <main> <summary> <time>
```
#### PS.编写HTML5文档注意遵守W3C相关标准,W3C提倡内容和结构分离,HTML结构具有语义化

#### semantic HTML
- HTML结构清晰, 易读性和维护性更好
- 无障碍阅读更友好, 对于读屏器等设备,能够播报的更流畅且准确
- 搜索引擎可根据标签的语言确定上下文和权重问题.更利于SEO优化, 语义化标签能够提升页面质量
