## Markdown标记语言入门

[TOC]

### 一、什么是 Markdown：

$\qquad\!\!$Markdown 是一种轻量级标记语言，由约翰·格鲁伯（John Gruber）于 $2004$ 年创立。$2017$ 年，GitHub 发布了基于 CommonMark 的 Github Flavored Markdown（[GFM](https://github.github.com/gfm/)）的正式规范。

$\qquad\!\!$约翰·格鲁伯对于 Markdown 的定义是：

> [Markdown is a text-to-HTML conversion tool for web writers. Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML).](https://daringfireball.net/projects/markdown/) 
>
> Markdown 是面向 Web作家 的文本到 HTML 转换工具。Markdown 允许您使用易于阅读，易于编写的纯文本格式进行编写，然后将其转换为结构上有效的 XHTML（或HTML）。

$\qquad\!\!$Markdown 的目标是实现「易读易写」，能够通过简单的标记语法，使普通的文本内容具有一定的格式。**标记语法**即通过一系列的控制字符，使得**写作本身**与**排版的细节**相分离。因此 Markdown 能够让你双手不离开键盘的情况下（只是使用键盘，而不用鼠标或触屏），实现给文本**加粗**，区别各级标题，引用格式，插入图片、链接、表格、数学公式等等功能。例如：**加粗**、_倾斜_、~~删除线~~

$\qquad\!\!$分离写作和排版还会带来一个意想不到的好处：你可以轻松地、迅速地把文档转换成另一个主题，或者_另一个样式_。

### 二、Markdown 能干什么：

$\qquad\!\!$作为一种为写作而生的语言，它在日常写作方面几乎可以代替 MS Word。你可以用 Markdown：

- 写文章
- 记笔记
- 写 Blog
- 写书
- 甚至……写论文

$\qquad\!\!$由于 Markdown 也是一种适用于网络的书写语言，很多知名的网站都支持用 Markdown 写作：

- 简书
- 洛谷，国内著名 OJ
- 马克飞象，印象笔记的一款工具
- GitHub，全球最大的~~同性~~程序员交友网站
- Reddit，知名的娱乐、社交及新闻网站
- Gitbook，写作网站

$\qquad\!\!$同时，本文就用 Markown 写作。

### 三、Markdown 的优缺点：

$\qquad\!\!$任何事物都具有两面性，虽然 Markdown 的优点不少，但是它还是具有一定的缺陷。

#### （一）、优点：

1. **标准化**：我们都有这种体验，一份 Word 文档，在自己电脑上看还好好的，但是发给他人就乱码了，这多半是由于两个软件平台编码格式不一致导致的。而 Markdown 不存在这样的问题，使用正式规范的编码对文本进行的格式化，在任何支持 Markdown 的平台，都能正常显示。

    > 由于平台显示形态可能不一样，比如标题的颜色、引用线粗细等会不太一样，因此要忠实重现文本，最好用 PDF 版本进行文件的传阅。

2. **轻量化**：纯文本的 Markdown 文档像记事本一样的快速，简洁，不用因为想写一个小文档，打开了笨重达 $2GB$ 的 MS Word。并且易于学习，新手学习没有门槛，入门简单、熟练快速。

3. **易于排版**：可以快速实现文字的排版。只通过键盘输入即可实现排版，不要另外操作排版，可以让作者摆脱排版的困扰，专心写作。不用像用 MS Word 一样一边写一边（凭感觉）排版, 甚至打乱了你写作的节奏。

4. **一次编辑多次多平台使用**：因为是纯文本，只要支持 Markdown 的地方都能获得相同的排版效果，不需要重复排版。同时它可在多种平台上获得支持，不像在很多地方并不支持 doc 和 docx 格式， 或者支持较弱。 比如 Linux、Mac OS、 笔记应用,、以及绝大部分网站。并且很多MarkDown编辑器都支持直接将文本转换为 pdf、docx、html 等格式。

#### （二）、缺点：

1. **需要记一些语法**。
2. **难以进行高级排版**：由于很多复杂的排版无法实现，只适用于普通排版要求的文档。
3. **可能令人分心**：由于严格的标准化，在书写 Markdown 文件的时候通常会非常注意格式排版，比如：中英文标点符号，空格，列表的插入与退出等。

### 四、Markdown 的语法：

$\qquad\!\!$看完前面的介绍，大家有没有跃跃欲试的感觉呢？那么接下来我们就来学习一下 Markdown 的基本语法！

#### （一）、段落与换行：

$\qquad\!\!$一个 Markdown 段落是由一个或多个连续的文本行组成，它的前后要有一个以上的**空行**。普通的 Markdown 段落不可以用空格或制表符来缩进。（所以这个段落前的空白怎么做到的呢？那就是 $\LaTeX$ 的妙用喽！详细请参照下面**内联公式**部分。）

> 空行：一行之内只包含回车换行、空格、制表符。

#### （二）、标题：

$\qquad\!\!$Markdown 的标题是在行首插入 $1$ 到 $6$ 个 #，# 和标题文字之间使用一个或多个空格，对应到标题 $1$ 到 $6$ 级。第一级和第二级的标题后自带分割线。

**例如**：

```
# 这是 H1
## 这是 H2
### 这是 H3
#### 这是 H4
##### 这是 H5
###### 这是 H6
```

**效果**：

[![ye1QL8.png](https://s3.ax1x.com/2021/02/01/ye1QL8.png)](https://imgchr.com/i/ye1QL8)

#### （三）、文字的修饰：

$\qquad\!\!$Markdown 使用星号（ * ）和底线（ _ ）作为修饰字词的符号，被 * 或 _ 包围的字词会被转成用 `<em>` 标签包围（即*斜体*），用两个 * 或 _ 包起来的话，则会被转成 `<strong>`（即**粗体**）。

**例如**：

```
*单引号斜体*

_单下划线斜体_

**双引号加粗**

__双下划线加粗__

~~删除线~~
```

**效果**：

*单引号斜体*

_单下划线斜体_

**双引号加粗**

__双下划线加粗__

~~删除线~~

$\qquad\!\!$但是如果你的 * 和 _ 两边都有空白的话，它们就只会被当成普通的符号。如果要在文字前后直接插入普通的星号或底线，你可以用反斜线（\）（参见下面的**反斜杠**部分）。

**例如**：

```
\*使用反斜线开头的\*被当做是普通的字符\*
```

**效果**：

\*使用反斜线开头的\*被当做是普通的字符\*

#### （四）、代码块：

1. ##### 小块代码：

    $\qquad\!\!$需要引用代码时，如果引用的语句只有一段，不分行，可以用 \` 将语句包起来。

    > 如果你真的要打这个字符的话，可以仿照和 \* 这个字符一样的处理方式，在 \` 前加一个反斜杠。

    **例如**：

    ```
    `#include<iostream>`
    ```

    **效果**：

    `#include<iostream>`

2. ##### 大块代码：

    $\qquad\!\!$Markdown 建立代码块的方法：将 ``` 置于这段代码的首行和末行，独立成一行。 

    $\qquad\!\!$第一行的 ``` 后面可以加上语言名称，例如 cpp、java、c、pascal 等（不要写成 c++ ）。

    **例如**：

    ```
    ​```cpp
    #include<iostream>
    int a,b;
    int main()
    {
    	std::cin>>a>>b;
    	std::cout<<a+b<<"\n";
    	return 0;
    }
    ​```
    ```

    **效果**：

    ```cpp
    #include<iostream>
    int a,b;
    int main()
    {
    	std::cin>>a>>b;
    	std::cout<<a+b<<"\n";
    	return 0;
    }
    ```

#### （五）、区块引用：

$\qquad\!\!$Markdown 标记区块引用的方法是在行的最前面加 \> ，也可以只在整个段落的第一行最前面加上 \>，区块引用内部可以嵌套，只要根据层次加上不同数量的 \> 即可，引用的区块内也可以使用其他的 Markdown 语法，包括标题、列表、代码区块等。

**例如**：

```
>Markdown 标记区块引用的方法是在行的最前面加>
>
>也可以只在整个段落的第一行最前面加上 >
>>区块引用内部可以嵌套，只要根据层次加上不同数量的 >即可.
>>
>>*我是内部嵌套区块，我可以使用其他 Markdown 语法哦*
>>
>>### 我是引用区块内使用标题3语法
>>```java
>>      //在引用区块内可以加入代码块
>>      import java.net.URL;
>>      import java.util.Arrays;
>>      import java.util.Date;
>>      import java.util.Set;
>>```
```

**效果**：

>Markdown 标记区块引用的方法是在行的最前面加 >
>
>也可以只在整个段落的第一行最前面加上 >
>>区块引用内部可以嵌套，只要根据层次加上不同数量的 > 即可.
>
>>*我是内部嵌套区块，我可以使用其他 Markdown 语法哦*
>
>>### 我是引用区块内使用标题3语法
>>```java
>> //在引用区块内可以加入代码块
>> import java.net.URL;
>> import java.util.Arrays;
>> import java.util.Date;
>> import java.util.Set;
>>```

#### （六）、列表：

$\qquad\!\!$Markdown 支持有序列表和无序列表，无序列表使用星号、加号或是减号作为列表标记，有序列表则使用数字接着一个英文句点。两种列表方式格式都是：列表标记+空格+列表项，即列表项目标记通常是放在最左边，也可以缩进最多 $3$ 个空格，项目标记后面则一定要接着至少一个空格或制表符。

$\qquad\!\!$列表能够支持通过换行自动延续、列表内嵌套列表、列表内使用其它 Markdown 语法等功能。

1. ##### 无序列表：

    $\qquad\!\!$星号、加号或是减号三种列表方式效果等同。

    **例如**：

    ```
    *   Red
    *   Green
    *   Blue
    
    +   Red
    +   Green
    +   Blue
    
    -   Red
    -   Green
    -   Blue
    ```

    **效果均为**：

    *   Red
    *   Green
    *   Blue

2. ##### 有序列表：（其实现在就在一个有序列表当中……）

    $\qquad\!\!$有序列表则使用数字接着一个英文句点。

    **例如**：

    ```
    1.  Red
    2.  Green
    3.  Blue
    ```

    **效果**：

    1.  Red
    2.  Green
    3.  Blue

#### （七）、行内链接：

$\qquad\!\!$在方块括号后面紧接着圆括号并插入网址链接即可，如果你还想要加上链接的 title 文字，只要在网址后面，用双引号把 title 文字包起来即可。

**形如**：`[an example](http://example.com/ "title")`

- `an example` 是想显示出的文字

- `http://example.com/` 是网站链接, 也可以是本机路径

- `"title"` 是把鼠标放在这个链接上时显示的文本
    - 相信你也发现了这个东西似乎没什么用。所以, 这部分是可选的
    - 对于印刷品，这并没有什么用

**例如**：

```
这是 [百度](http://www.baidu.com/“百度”) 内联方式。
```

**效果**：

这是 [百度](http://www.baidu.com/"百度") 内联方式。

#### （八）、图片：

$\qquad\!\!$Markdown 使用一种和链接很相似的语法来标记图片，一个惊叹号 \!，接着一个方括号，里面放上图片的替代文字（这些文字将在图片加载失败的时候显示），接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 title 文字。

**形如**：`![lable](picture path "title")`

**例如**：

```
![YuYl5V.jpg](https://s1.ax1x.com/2020/05/08/YuYl5V.jpg)
```

**效果**：

![YuYl5V.jpg](https://s1.ax1x.com/2020/05/08/YuYl5V.jpg)

<center> 我的电脑桌面啦 </center> 

#### （九）、自动链接：

$\qquad\!\!$Markdown 支持以比较简短的自动链接形式来处理网址和电子邮件信箱，只要是用尖括号包起来， Markdown 就会自动把它转成链接。一般网址的链接文字就和链接地址一样。

**例如**：

```
<https://www.baidu.com>
```

**效果**：

<https://www.baidu.com>

#### （十）、表格：

$\qquad\!\!$表格是 GFM 对 Markdown 原规范的扩展，但几乎所有的编辑器都支持这一语法。表格由两部分组成：表头和内容。

**例如**：

```
| Items          | Price      | Description               |
| -              | :--:       | -:                        |
| T-Shirt        | £9.15      | Suggested in the NCEE     |
| Uniform in H3Z | about ¥100 | design beyond description |
| left aligned   | centered   | right aligned             |
```

**效果**：

| Items          |   Price    |               Description |
| -------------- | :--------: | ------------------------: |
| T-Shirt        |   £9.15    |     Suggested in the NCEE |
| Uniform in H3Z | about ¥100 | design beyond description |
| left aligned   |  centered  |             right aligned |

$\qquad\!\!$上面的分隔符是 \|， 也就是 Backspace 和 Enter 中间的键。

- 表头（也就是第一行）是必选的
- 第二行声明了表格。每格中 \-  至少一个， 不过也可以是连续的多个， 没有影响
    - 每格中两边的 : 代表对齐方式
        1. :\- 或者 \- 左对齐
        2. :\-: 居中对齐
        3. \-: 右对齐
- 之后的每一行就是表格的具体内容

$\qquad\!\!$美观起见，你可以在每一格的文字两边加入若干空格，但没有影响。每一格的文字都可以为空（包括表头），只需有两边的 \| 即可，这时表格中的这一格也会为空。

#### （十一）、分隔线：

$\qquad\!\!$可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他内容。也可以在星号或是减号中间插入空格。

**例如**：

```
* * *

***

*****

- - -

---------------------------------------
```

**效果**：

* * *

***

*****

- - -

---------------------------------------

#### （十二）、反斜杠：

$\qquad\!\!$Markdown 可以利用反斜杠来插入一些在语法中有其它意义的符号，例如：如果你想要用星号加在文字旁边的方式来做出强调效果（但不用`<em>`标签倾斜），你可以在星号的前面加上反斜杠。

$\qquad\!\!$Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号。加上反斜杠后，这些符号都会以原来的方式显示：

```
\   反斜线
`   反引号
*   星号
_   底线
{}  花括号
[]  方括号
()  括弧
#   井字号
+   加号
-   减号
.   英文句点
!   惊叹号
```

#### （十三）、嵌入 HTML：

$\qquad\!\!$根据 Markdown 的定义或者说原理可知：Markdown 渲染就是把它翻译成 HTML。

$\qquad\!\!$那么, 我们可不可以在 Markdown 中直接使用 HTML 呢? 答案是肯定的。有能力的同学, 可以在写的 Markdown 文档中加入 HTML 代码，来实现一些 Markdown 本身无法实现的功能。

**例如**：上文图片下面的那句居中的话：

```
<center> 我的电脑桌面啦 </center> 
```

**效果**：

<center> 我的电脑桌面啦 </center> 



> 不过，必须用 HTML 的地方其实很少。而且很多都可以用内联的 $\LaTeX$ 代替。

$\qquad\!\!$比如，在表格中实现换行：

**例如**：

```
//HTML 实现换行：
| Header1 | Header2                          |
|---------|----------------------------------|
| item 1  | 1. one<br />2. two<br />3. three |
```

**效果**：

| Header1 | Header2                          |
| ------- | -------------------------------- |
| item 1  | 1. one<br />2. two<br />3. three |

**例如**：

```
//LaTeX 实现换行：
| Header1 | Header2                          |
|---------|----------------------------------|
| item 1  | $ 1. one \\ 2. two \\ 3. three $ |
```

**效果**：（大家有没有觉得用 $\LaTeX$ 不仅仅能够换行，而且渲染出来的数字和英文更美观了呢？）

| Header1 | Header2                          |
| ------- | -------------------------------- |
| item 1  | $ 1. one \\ 2. two \\ 3. three $ |

### 五、$\LaTeX$ 公式：

$\qquad\!\!$前文中多次提到了一个词：$\LaTeX$，相信大家一定很好奇它究竟是个什么东西，那么它究竟是个啥？

#### （一）、$\LaTeX$ 简介：

$\qquad\!\!\TeX$ 是一个由美国计算机教授高德纳编写的功能强大的排版软件，而为了让使用者可以更为方便的使用 $\TeX$的强大功能，美国计算机科学家莱斯利·兰伯特在 $20$ 世纪 $80$ 年代初期开发了一种基于 $\TeX$ 的排版系统—— $\LaTeX$。

$\qquad\!\!$ $\LaTeX$ 是当今世界上最流行和使用最为广泛的 $\TeX$ 宏集。使用 $\LaTeX$ 基本上不需要使用者自己设计命令和宏等，因为 $\LaTeX$ 已经替你做好了。因此，即使使用者并不是很了解 $\TeX$，也可以在短短的时间内生成高质量的文档。**而对于生成复杂的数学公式，$\LaTeX$ 表现的更为出色**。

$\qquad\!\LaTeX$作为一门能**生成媲美书籍的质量的文章**的语言，和 Markdown 一样可以用来写作，但是这里和这篇文章无关，就不再过多介绍了。不过有兴趣的同学可以参考 Reference 中的 ${}^5$ 自行学习。

#### （二）、内联公式：

$\qquad\!\!$虽然 $\LaTeX$ 作为一门独立的排版系统，但是它的行内数学公式却可以在 Markdown 中作为内联公式所存在。就我个人而言，如此喜欢使用 Markdown，与能够生成复杂、漂亮的数学公式的内联公式密不可分。

$\qquad\!\!$在 Markdown 文档中，将数学公式写在两个 \$ 之间，便代表插入了行内数学公式。

#### （三）、部分语法：

$\qquad\!\!$由于 $\LaTeX$ 的功能十分强大，支持的公式类型也极其之多，在这里仅仅介绍一部分我个人认为比较常用的语法，其它更多可参考 Reference 中的 ${}^6$ 自行学习。

1. 上标下标：

    ```
    $a^2 a_2 a^{2+2} a_{i,j} a^2_2 {}^2_1\!X^3_4$
    // \!的作用在下面空格一栏有讲述。
    ```

    $a^2 \ \ a_2 \ \ a^{2+2} \ \ a_{i,j} \ \ a^2_2 \ \ {}^2_1\!X^3_4$

2. 根号：

    ```
    $\surd \sqrt{2} \sqrt[n]{} \sqrt[n]{x}$
    ```

    $\surd \ \ \sqrt{2} \ \ \sqrt[n]{} \ \ \sqrt[n]{x}$

3. 运算符、巨运算符：

    ```
    $+ - \pm \mp \times \div$
    ```

    $+ \ \ - \ \ \pm \ \ \mp \ \ \times \ \ \div$

    ```
    $\sum_{i=1}^na_i \sum\limits_{i=1}^na_i$
    // 求 a_1+……+a_n
    $\prod_{i=1}^na_i \prod\limits_{i=1}^na_i$
    // 求 a_1*……*a_n
    ```

     $\sum_{i=1}^na_i \ \ \sum\limits_{i=1}^na_i \ \ \prod_{i=1}^na_i \ \ \prod\limits_{i=1}^na_i$

4. 分数、百分数：

    ```
    $\frac{1}{2}=0.5 \tfrac{1}{2}=0.5 \dfrac{1}{2}=0.5$
    $\dfrac{1}{x+\dfrac{3}{y+\dfrac{1}{5}}}$
    // 从美观的角度来看，我通常使用 \dfrac{}{} 作为分数
    ```

    $\frac{1}{2}=0.5 \ \ \tfrac{1}{2}=0.5 \ \ \dfrac{1}{2}=0.5 \ \ \dfrac{1}{x+\dfrac{3}{y+\dfrac{1}{5}}}$

5. 标准函数：

    ```
    $\sin a \cos b \tan c \left\vert a \right\vert$
    $\min(x,y) \max(x,y) \gcd(m,n) \operatorname{lcm}(m,n)$
     //未预先定义的标准函数，均可用 \operatorname{}() 的格式定义
    ```

     $\sin a \ \ \cos b \ \ \tan c \ \ \left\vert a \right\vert \ \ \min(x,y) \ \ \max(x,y) \ \ \gcd(m,n) \ \ \operatorname{lcm}(m,n)$

6. 集合符号：

    ```
    $\{ \} \emptyset \varnothing $
    ```

    $\{ \} \ \ \emptyset \ \ \varnothing $

    ```
    $\in \notin \not\in \ni \not\ni$
    // \not 是在下一个字符上画斜杠。
    ```

    $\in \ \ \notin \ \ \not\in \ \ \ni \ \ \not\ni$

    ```
    $\cap \cup \complement_U A$
    ```

    $\cap \ \ \cup \ \ \complement_U A$

    ```
    $\subset \supset \subseteqq \subsetneqq \supseteqq \supsetneqq$
    ```

    $\subset \ \ \supset \ \ \subseteqq \ \ \subsetneqq \ \ \supseteqq \ \ \supsetneqq$

7. 关系符号：

    ```
    $= \ne \neq \equiv \not\equiv \approx$
    ```

    $= \ \ \ne \ \ \neq \ \ \equiv \ \ \not\equiv \ \ \approx$

    ```
    $< > \leqslant \geqslant$
    ```

    $< \ \ > \ \ \leqslant \ \ \geqslant$

8. 几何符号：

    ```
    $\parallel \perp \angle \sphericalangle \measuredangle 45^\circ$
    ```

    $\parallel \ \ \perp \ \ \angle \ \ \sphericalangle \ \ \measuredangle \ \ 45^\circ$

9. 逻辑符号：

    ```
    $\forall \exists \nexists \therefore \because \And \&$
    ```

    $\forall \ \ \exists \ \ \nexists \ \ \therefore \ \ \because \ \ \And \ \ \&$

10. 希腊字母：

    ```
    $\alpha \beta \gamma \eta \theta \mu \pi \rho \omega \phi$
    ```

    $\alpha \beta \gamma \eta \theta \mu \pi \rho \omega \phi$

11. 空格和换行：

    ```
    $x\!y \\ xy \\ x\,y \\ x\;y \\ x\ y \\ x\quad y \\ x\qquad y$
    ```

    $x\!y 宽度为-\dfrac{m}{6}\\ xy 宽度为0\\ x\,y 宽度为\dfrac{m}{6}\\ x\;y 宽度为\dfrac{2m}{7}\\ x\ y 宽度为\dfrac{m}{3}\\ x\quad y 宽度为m\\ x\qquad y宽度为2m$

    > 在文档中，段落前空两格大概是 $\dfrac{5m}{3}$ 的宽度，所以在段首键入 `$\qquad\!\!$` 即可做到。

12. 其它：

    ```
    $\TeX \LaTeX$
    ```

    $\TeX \ \ \LaTeX$

    ```
    // 二项式系数
    $\dbinom{n}{m}=\dbinom{n}{n-m}=C_n^m=C_n^{n-m}$
    ```

    $\dbinom{n}{m}=\dbinom{n}{n-m}=C_n^m=C_n^{n-m}$

    ```
    // 方程组
    $\begin{cases}2x+9y-5z=10\\4x+20y+z=24\\x-\dfrac{1}{2}y+3z=8\end{cases}$
    ```

    $\begin{cases}2x+9y-5z=10\\4x+20y+z=24\\x-\dfrac{1}{2}y+3z=8\end{cases}$

$\qquad\!\!$虽然看起来挺多，但是其实还有颜色、字体更多的公式和符号的语法没有介绍，更多可参考 Reference 中的 ${}^6$ 自行学习。

### 六、Markdown 编辑器 Typora：

$\qquad\!\!$学会了 Markdown 的语法后，大家就可以在很多网站上进行相应的编辑。但是如果想在本地进行利用 Markdown 书写，并且输出为各种格式的文档，就需要一款 Markdown 编辑器。在众多的 Markdown 编辑器中，在这里推荐给大家一款相当好用的 Markdown 编辑器：Typora.

#### （一）、什么是 Typora?

$\qquad\!\!$Typora 是一款轻便、简洁、**免费**、轻量级的 Markdown 编辑器，它是一款跨平台的 Markdown 写作软件，具备写作 Markdown 的绝大部分功能，你可以在 Windows,Mac OS，甚至各大 Linux 发行版上使用它。

$\qquad\!\!$作为一款 **富文本的编辑模式 +** **Markdown 源格式** 的编辑器，Typora 支持**即时渲染**技术，即**“所见即所得”**。我们可以像编辑 word 文档一样流畅地编辑 Markdown 文档。这是 Typora 与其它各种 Markdown 编辑器最大的区别，不用像其它编辑器一样拥有繁重的工具栏以及必须分为左右两列：++ 源码 ++|++ 显示 ++，十分便捷。

#### （二）、外观：

$\qquad\!\!$图标样式：

[<img src="https://s3.ax1x.com/2021/02/02/yu4Oat.png" alt="yu4Oat.png" style="zoom:50%;" />](https://imgchr.com/i/yu4Oat)

$\qquad\!\!$光是图标是不是就已经感觉非常简洁了呢？还有更加简洁的就是，其它的 Markdown 编辑器一般都有一个工具栏并且一半是编辑窗口，一半是预览窗口：[![yu50eA.png](https://s3.ax1x.com/2021/02/02/yu50eA.png)](https://imgchr.com/i/yu50eA)

$\qquad\!\!$但是 Typora 的窗口：[![yu5jm9.png](https://s3.ax1x.com/2021/02/02/yu5jm9.png)](https://imgchr.com/i/yu5jm9)

既不存在工具栏也仅仅为单独一个界面。

#### （三）、主题：

$\qquad\!\!$细心的同学们一定能注意到上面 Typora 页面顶部有一个**主题**菜单，选择后发现其中有五个不同的主题选项：Github,Newsprint,Night,Pixyll,Whitey.

[![yuIJ7n.png](https://s3.ax1x.com/2021/02/02/yuIJ7n.png)](https://imgchr.com/i/yuIJ7n)

$\qquad\!\!$这里放一张来自 Typora 官网的图片，从左到右依次为 Github,Newsprint,Night,Whitey 主题的页面。

$\qquad\!\!$看到了这么几个主题，有没有想都体验一遍的冲动？不用着急，Typora 不仅仅支持这五个自带的主题，更支持定制化主题，开发者可以开发主题。如果你对 CSS 有所涉及，便能做出专属于自己的主题。

#### （四）、对于 Markdown 的支持：

$\qquad\!\!$除了仅仅支持普通的 Markdown 语法外，Typora 还有更加便捷的 Markdown 使用方式。

$\qquad\!\!$首先是一些有关的设置：

> 文件 $\rightarrow$ 偏好设置 $\rightarrow$ Markdown

[![yuor28.png](https://s3.ax1x.com/2021/02/02/yuor28.png)](https://imgchr.com/i/yuor28)

$\qquad\!\!$这些设置还是蛮重要的，否则内联公式 $\LaTeX$、==高亮== 等扩展性的语法均无法使用。

$\qquad\!\!$再者，以 Typora 较为突出的 表格、代码块、公式块 三个方面进行一下简单的介绍：

1. 表格：

    >ctrl+t / 鼠标右键 $\rightarrow$ insert / 段落 $\rightarrow$ 表格

    然后它会出现让我们选择**行列数**的窗口，这样的话就不用十分麻烦地去敲 Markdown 中表格的语法了。

    [![yuTSxO.png](https://s3.ax1x.com/2021/02/02/yuTSxO.png)](https://imgchr.com/i/yuTSxO)

    $4\times4$ 的表格：

    [![yuozRK.png](https://s3.ax1x.com/2021/02/02/yuozRK.png)](https://imgchr.com/i/yuozRK)

    但是这样就无法去编辑其格式无法控制对齐了啊？没事的，通过左上角的**调整表格**，轻松可以做到。

2. 代码块：

    > ctrl+shift+k / 鼠标右键 $\rightarrow$ insert / 段落 $\rightarrow$ 代码块

    Typora 可以通过你指定的语言来高亮代码，并且支持上百种语言，足够一般的用途。

    [![yuT5TA.png](https://s3.ax1x.com/2021/02/02/yuT5TA.png)](https://imgchr.com/i/yuT5TA)

3. 公式块：

    >ctrl+shift+m / 鼠标右键 $\rightarrow$ insert / 段落 $\rightarrow$ 公式块

    Typora 不仅仅支持行内式，也支持行外的公式块。由于相当于处于 \$\$ 与 \$\$ 之间，所以会被强制居中。这种十分大气的行外式特别适合巨运算符的书写：

    [![yuHCEd.png](https://s3.ax1x.com/2021/02/02/yuHCEd.png)](https://imgchr.com/i/yuHCEd)

    

> 这三点不仅仅可以利用 Typora 自身的属性操作，别忘了也可以直接用 Markdown 的语法进行操作哦！

#### （五）、专注模式与打字机模式：

$\qquad\!\!$Typora 同时支持两种写作模式：专注模式与打字机模式。

1. 专注模式（Focus Mode）：

    > F8 / 视图 $\rightarrow$ 专注模式

    在这个模式下，当你在编辑某一行文字的时候其他行会变成灰色。

    [![yuvkdO.png](https://s3.ax1x.com/2021/02/03/yuvkdO.png)](https://imgchr.com/i/yuvkdO)

    专注模式比较适合与全屏同时开启，连工具栏都不存在，自然简洁到超级舒服。

2. 打字机模式：

    > F9 / 视图 $\rightarrow$ 打字机模式

    在这个模式下，你的光标会始终处于屏幕中间，我们的眼光就能始终正对屏幕中央。就我个人来讲非常喜欢使用这个模式，不仅仅是因为不用动眼睛，更因为光标的自动换行能够更加便于仅键盘进行操作。

    [![yuvskF.png](https://s3.ax1x.com/2021/02/03/yuvskF.png)](https://imgchr.com/i/yuvskF)

    相信大家能够捕捉到光标的位置。

> 这两种模式并不相斥，更是能够同时使用的哦！

#### （六）、字数统计、拼写检查与源代码模式：

$\qquad\!\!$相信大家一定对前面图片上页面底部的几个图标产生了好奇，下面就来简单地介绍一下：

1. 字数统计：

    和 Word 文档一样，Typora 也支持实时统计文档的字数，位于页面的右下角：

    [![yuxEn0.png](https://s3.ax1x.com/2021/02/03/yuxEn0.png)](https://imgchr.com/i/yuxEn0)

    *哇！这篇文章也已经六千多词了欸！*

2. 拼写检查：

    和 Word 文档一样，Typora 也支持实时的拼写检查，位于字数统计旁边：

    [<img src="https://s3.ax1x.com/2021/02/03/yuxM9J.png" alt="yuxM9J.png" style="zoom:50%;" />](https://imgchr.com/i/yuxM9J)

    *虽然在打中文的时候从来没见过它报错……*

3. 源代码模式：

    即显示文档的 Markdown 源码的一种模式，开关位于页面左下角旁：[![yuxNND.png](https://s3.ax1x.com/2021/02/03/yuxNND.png)](https://imgchr.com/i/yuxNND)

    开启后就能够以纯文本的格式显示文档的 Markdown 源码：

    [![yuxw3d.png](https://s3.ax1x.com/2021/02/03/yuxw3d.png)](https://imgchr.com/i/yuxw3d)

    *说实话我还真没开着源代码模式打过文档。*

#### （七）、侧边栏与自生成目录：

$\qquad\!\!$还差页面最右下角的一个图标没有介绍了。没错！你没猜错！就是**侧边栏**。

1. 侧边栏：

    在显示侧边栏后，会发现上面有两个子目录：文件与大纲。

    文件就是显示该文档所在的目录结构以及该文档所在的目录里其它可被导入 Typora 的文档：

    [<img src="https://s3.ax1x.com/2021/02/03/yuzkPe.png" alt="yuzkPe.png" style="zoom:50%;" />](https://imgchr.com/i/yuzkPe)

    大纲即由现在编辑的文档的标题组成的目录结构：

    [<img src="https://s3.ax1x.com/2021/02/03/yuz3GQ.png" alt="yuz3GQ.png" style="zoom:50%;" />](https://imgchr.com/i/yuz3GQ)

2. 自生成目录：

    在文章开始写入 `[TOC]` 将自动在文章生成目录：

    [![yuztrq.md.png](https://s3.ax1x.com/2021/02/03/yuztrq.md.png)](https://imgchr.com/i/yuztrq)

    *并且能够支持文档内部的超链接哦！*

#### （八）、文本导出：

$\qquad\!\!$文本导出也能够算是 Typora 非常方便的一大特性，Typora 本身能够支持导出 PDF 文档、两种样式的 HTML 文档以及图像！

$\qquad\!\!$同时也可以导出 Word,Epub,LaTeX 等其它多种文件格式，不过需要安装 pandoc 进行辅助。不过无须多虑的是，在并未安装 pandoc 时，点击 Word 文档等即可进入 Typora 对于 pandoc 的安装引导，十分方便地安装完甚至不用学 pandoc 的各种文件转换命令即可在 Typora 中直接使用。

#### （九）、下载方式：

$\qquad\!\!$讲了这么多，相信大家已经对用 Typora 编写 Markdown 跃跃欲试了！那么在哪里能够下载呢？

$\qquad\!\!$进入 Typora 官网 <https://www.typora.io/> 即可！

[![yKSkwV.png](https://s3.ax1x.com/2021/02/03/yKSkwV.png)](https://imgchr.com/i/yKSkwV)

$\qquad\!\!$下滑到底部后，即可选择下载哪种 Typora ，下载完安装后即可使用！

### 七、结语：

$\qquad\!\!$完稿于 2021/2/3 凌晨。

$\qquad\!\!$写了一段时间的班刊终于完美收官了！相信大家看完之后一定会有所收获。

$\qquad\!\!$文章的内容和标题**相照应**，仅仅是一篇~~自我感觉良好的~~ Markdown 入门教程。无论是 Markdown 的扩展，还是 $\LaTeX$ 五花八门的公式，还是 Typora 的部分功能，我都有没介绍到的地方。而且我接触 Markdown 的时间也不算长，文章如有疏漏不当之处，请各位读者海涵。

$\qquad\!\!$如果你看完这篇文章后不想尝试 Markdown 的写作，那就权当是增加了知识；如果你看完这篇文章后对用 Markdown 写作充满了期待，那就现在就用 Markdown 写一篇文章吧！相信你也会体验到这个有数百万人使用的语言的优美之处！

$\qquad\!\!$最后，由衷地感谢班主任老师及同学门组织的这次班刊编写活动，给了我写这篇文章的一个机会；感谢我参考的文章的作者，让我有了这篇文章的素材；也要感谢帮助我审稿校验的朋友们，是你们给予了我投稿的支持；更要感谢每一位读完这篇文章的读者，衷心地希望这篇文章能够使大家有所受益！

----------

Reference:

1. [Markdown 标记语言指北](https://www.cnblogs.com/ubospica/p/11065405.html) *学长的文章哦！*
2. [Markdown标记语法，从入门到熟练](https://zhuanlan.zhihu.com/p/112327926)
3. [洛谷 Markdown 格式手册](https://www.luogu.com.cn/blog/luogu/how-to-use-markdown)
4. [也许 Markdown 并不是一个好选择](https://zhuanlan.zhihu.com/p/68293222)
5. [LaTeX入门](https://www.luogu.com.cn/blog/IowaBattleship/latex-ru-men)
6. [LaTeX数学公式大全](https://www.luogu.com.cn/blog/IowaBattleship/latex-gong-shi-tai-quan)
7. [Typora ---一款简洁的Markdown编辑器](https://www.cnblogs.com/-guz/p/10258557.html)
8. [Typora - 不要太棒的Markdown编辑器](https://zhuanlan.zhihu.com/p/44998516)

