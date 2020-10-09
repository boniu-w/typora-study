









# 区域元素

## YAML FONT Matters

在文章最上方输入---，按换行键产生，输入内容即可

## 菜单

输入+换行键，产生标题，自动更新

```
[toc]
```

[TOC]

## 快捷键

无序列表：输入-之后输入空格
有序列表：输入数字+“.”之后输入空格
任务列表：-[空格]空格 文字
标题：ctrl+数字
表格：ctrl+t
生成目录：[TOC]按回车
选中一整行：ctrl+l
选中单词：ctrl+d
选中相同格式的文字：ctrl+e
跳转到文章开头：ctrl+home
跳转到文章结尾：ctrl+end
搜索：ctrl+f
替换：ctrl+h
引用：输入>之后输入空格
代码块：ctrl+alt+f
加粗：ctrl+b
倾斜：ctrl+i
下划线：ctrl+u
删除线：alt+shift+5
插入图片：直接拖动到指定位置即可或者ctrl+shift+i
插入链接：ctrl+k



## 段落

按换行键建立新的一行
可在行尾插入打断线，禁止向后插入

```
按换行键建立新的一行<br/>
```

## 标题

开头#的个数表示，空格+文字。标题有1~6个级别，#表示开始，按换行键结束

```
# H1
## H2
###### H6
```

## 引注

开头>表示，空格+文字，按换行键换行，双按换行跳出

```
> ni
>
> ni hao
```

> ni
>
> nini

## 序列

开头*/+/-，空格+文字，可以创建无序序列，换行键换行，删除键+shift+tab跳出

开头1.，空格+后接文字，可以创建有序序列

```
*   Red
+   Green
-   Blue

1.  Red
2.  Green
3.  Blue
```

- 无序序列

1. 你

## 可选序列

开头序列+空格+[ ]+空格+文字，换行键换行，删除键+shift+tab跳出

```
- [ ] a
+ [ ] b
* [ ] c
- [x] completed
```

- [ ] a
- [ ] b
- [ ] c
- [x] d

## 代码块

开头```+语言名，开启代码块，换行键换行，光标下移键跳出

```
​```python
​```
```

## 数学块

使用MtathJax建立数学公式

开头$$+换行键，产生输入区域，输入Tex/LaTex格式的数学公式

```
$$

$$
```

$$
\mathbf{V}_1 \times \mathbf{V}_2 = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \
\frac{\partial X}{\partial u} & \frac{\partial Y}{\partial u} & 0 \
\frac{\partial X}{\partial v} & \frac{\partial Y}{\partial v} & 0 \
\end{vmatrix}
$$

## 表格

开头|+列名+|+列名+|+换行键，创建一个2*2表格

将鼠标放置其上，弹出编辑尺寸，个数，文字等

```
|first|second|
```

| first | second |
| ----- | ------ |
|       |        |

## 脚注

在需要添加脚注的文字后面+[+^+序列+]，注释的产生可以鼠标放置其上单击自动产生，添加信息

或人工添加+[+^+序列+]+:

```
脚注产生的方法[^footnote].
[^footnote]:这个就是*脚注*
```

脚注产生的方法[1](http://www.cnblogs.com/fhkankan/p/8082351.html#fn1).

## 水平线

输入***/---，换行键换行

```
***
---
```

------

------

# 特征元素

## 链接

单击链接，展开后可编辑

ctr+单击，打开链接

### 超链接

用[]括住要超链接的内容，紧接着用()括住超链接源+名字，超链接源后面+超链接命名

```
This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.
```

This is [an example](http://example.com/) inline link.

[This link](http://example.net/) has no title attribute.

### 内链接

### 相关链

使用[+超链接文字+]+[+标签+]，创建可定义链接

```
This is [an example][id] reference-style link.

Then, anywhere in the document, you define your link label like this, on a line by itself:

[id]: http://example.com/  "Optional Title Here"
```

[Baidu](http://baidu.com/)
And then define the link:

[Google](http://google.com/)
And then define the link:

## URLs

用<>括住url，可手动设置url

对于标准URLs，可自动识别

```
<i@163.com>
www.baidu.com
```

[i@163.com](mailto:i@163.com)

www.baidu.com

## 图片

1. 手动添加：类似链接，前面需加！
2. 用鼠标拖图片进入，然后鼠标放置其上修改

```
![Alt text](/path/to/img.jpg)

![Alt text](/path/to/img.jpg "Optional title")
```

![Alt text](http://www.cnblogs.com/path/to/img.jpg)

![Alt text](http://www.cnblogs.com/path/to/img.jpg)

## 斜体

以**或__括住，建议双*

```
*single asterisks*

_single underscores_
```

*single asterisks*

*single underscores*

## 加粗

开头双*或双_，结尾双*或双_，建议双*

```
**double asterisks**

__double underscores__
```

**double asterisks**

**double underscores**

## 删除线

用两个~开头，两个~结尾

```
~~Mistaken text.~~
```

~~错误文字.~~

## 下划线

使用HTML标签

```
<u>Underline</u>
```

Underline

## 代码

用两个`在正常段落总表示代码

```
Use the `printf()` function.
```

Use the `printf()` function.

## 数学式

需 `Preference` Panel -> `Markdown` Tab启动，

输入$，然后按ESC键，之后输入Tex命令，可预览

```
$\lim_{x\to\infty}\exp(-x)=0$
```

$\lim_{x\to\infty}\exp(-x)=0$

## 下标

需 `Preference` Panel -> `Markdown` Tab启动，

使用双~括住内容

```
H~2~O, X~long\ text~/
```

H~2~O`,`X~long text~

## 上标

需 `Preference` Panel -> `Markdown` Tab启动，

使用双^括住内容

```
X^2^
```

X^2^

## 高亮

需 `Preference` Panel -> `Markdown` Tab启动，

使用双==括住内容

```
==highlight==
```

==highlight==

## 改变表格的宽度

```javascript
<span style="white-space: nowrap;">表格的其中一列&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;</span> 
```



```javascript
&emsp; 是全角空格
&nbsp; 半角空格
```



## 快捷键

### 文件

| 功能                 | 热键（Windows / Linux） | 热键（macOS）        |
| :------------------- | :---------------------- | -------------------- |
| 新                   | Ctrl + N.               | Command + N.         |
| 新窗户               | Ctrl + Shift + N.       | Command + Shift + N. |
| 新标签               | *（不支持）*            | Command + T.         |
| 打开                 | Ctrl + O.               | Command + O.         |
| 快速打开             | Ctrl + P.               | Command + Shift + O. |
| 重新打开已关闭的文件 | Ctrl + Shift + T.       | Command + Shift + T. |
| 保存                 | Ctrl + S.               | Command + S.         |
| 另存为/重复          | Ctrl + Shift + S.       | Command + Shift + S. |
| 偏爱                 | Ctrl +，                | Command +，          |
| 关                   | Ctrl + W                | Command + W          |





### 编辑

| 功能                                | 热键（Windows / Linux）    | 热键（macOS）                       |
| :---------------------------------- | :------------------------- | ----------------------------------- |
| 新段落                              | 输入                       | 输入                                |
| 新队                                | Shift + Enter              | Shift + Enter                       |
| 切                                  | Ctrl + X.                  | Command + X.                        |
| 复制                                | Ctrl + C.                  | Command + C.                        |
| 糊                                  | Ctrl + V.                  | Command + V.                        |
| 复制为Markdown                      | Ctrl + Shift + C.          | Command + Shift + C.                |
| 粘贴为纯文本                        | Ctrl + Shift + V.          | Command + Shift + V.                |
| 全选                                | Ctrl + A.                  | Command + A.                        |
| 选择行/句子 选择行（在表格中）      | Ctrl + L.                  | Command + L.                        |
| 删除行（在表中）                    | Ctrl + Shift + Backspace   | Command + Shift + Backspace         |
| 选择样式范围 选择单元格（在表格中） | Ctrl + E.                  | Command + E.                        |
| 选择Word                            | Ctrl + D.                  | Command + D.                        |
| 删除Word                            | Ctrl + Shift + D.          | Command + Shift + D.                |
| 跳到顶部                            | Ctrl + Home                | Command +↑                          |
| 跳转到选择                          | Ctrl + J                   | Command + J                         |
| 跳到Buttom                          | Ctrl + End                 | Command +↓                          |
| 找                                  | Ctrl + F.                  | Command + F.                        |
| 找下一个                            | F3 /回车                   | Command + G / Enter                 |
| 找到上一个                          | Shift + F3 / Shift + Enter | Command + Shift + G / Shift + Enter |
| 更换                                | Ctrl + H.                  | Command + H.                        |





### 段

| 功能         | 热键（Windows / Linux） | 热键（macOS）            |
| :----------- | :---------------------- | ------------------------ |
| 标题1到6     | Ctrl + 1/2/3/4/5/6      | Command + 1/2/3/4/5/6    |
| 段           | Ctrl + 0                | 命令+ 0                  |
| 提高标题级别 | Ctrl + =                | 命令+ =                  |
| 降低标题级别 | Ctrl + -                | 命令+ -                  |
| 表           | Ctrl + T.               | Command + Option + T.    |
| 代码围栏     | Ctrl + Shift + K.       | Command + Option + C.    |
| 数学块       | Ctrl + Shift + M.       | Command + Option + B.    |
| 引用         | Ctrl + Shift + Q.       | Command + Option + Q.    |
| 订购清单     | Ctrl + Shift + [        | Command + Option + O.    |
| 无序列表     | Ctrl + Shift +]         | Command + Option + U.    |
| 缩进         | Ctrl + [/ Tab           | Command + [/ Tab         |
| 减少缩进     | Ctrl +] / Shift + Tab   | Command +] / Shift + Tab |



### 格式

| 功能     | 热键（Windows / Linux）             | 热键（macOS）         |
| :------- | :---------------------------------- | --------------------- |
| 强大     | Ctrl + B.                           | Command + B.          |
| 重点     | Ctrl + I                            | 命令+我               |
| 强调     | Ctrl + U.                           | Command + U.          |
| 码       | Ctrl + Shift +`| Command + Shift +` |                       |
| 罢工     | Alt + Shift + 5                     | Control + Shift +`    |
| 超链接   | Ctrl + K.                           | Command + K.          |
| 图片     | Ctrl + Shift + I                    | Command + Control + I |
| 清除格式 | Ctrl + \                            | 命令+                 |



### 视图

| 功能                      | 热键（Windows / Linux） | 热键（macOS）         |
| :------------------------ | :---------------------- | --------------------- |
| 切换补充工具栏            | Ctrl + Shift + L.       | Command + Shift + L.  |
| 大纲                      | Ctrl + Shift + 1        | Command + Control + 1 |
| 用品                      | Ctrl + Shift + 2        | Command + Control + 2 |
| 文件树                    | Ctrl + Shift + 3        | Command + Control + 3 |
| 源代码模式                | Ctrl + /                | 命令+ /               |
| Fouus模式                 | F8                      | F8                    |
| 打字机模式                | F9                      | F9                    |
| Toggler全屏               | F11                     | Command + Option + F. |
| 真实大小                  | Ctrl + Shift + 0        | *（不支持）*          |
| 放大                      | Ctrl + Shift + =        | *（不支持）*          |
| 缩小                      | Ctrl + Shift + -        | *（不支持）*          |
| 在打开的Documnets之间切换 | Ctrl + Tab              | 命令+`                |
| 切换DevTools              | Ctrl + Shift + I        | -                     |