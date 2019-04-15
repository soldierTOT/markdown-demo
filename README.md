__Markdown基本语法__
====================
*注：本文档参考<https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet>编写*

----------------------
* [一、标头](##一、标头)  
* [二、强调重点](##二、强调重点)  
* [三、列表](##三、列表) 
* [四、链接](##四、链接) 
* [五、图片](##五、图片) 
* [六、代码及语法高亮](##六、代码及语法高亮) 
* [七、表格](##七、表格) 
* [八、块引用](##八、块引用) 
* [九、内联HTML](##九、内联HTML) 
* [十、水平分割线](##十、水平分割线) 
* [十一、换行符](##十一、换行符) 
* [十二、音频文件](##十二、音频文件) 
* [十三、TeX数学公式](##十三、TeX数学公式) 
----------------------

## 一、标头
  ```html
  <!-- 其中只有H1&H2含有下划线 -->
  # H1
  ## H2
  ### H3
  #### H4
  ##### H5
  ###### H6

  <!-- H1&H2的另一种表示方法(下划线表示风格) -->
  H1要包含的内容
  =============

  H1要包含的内容
  -------------
  ```
## 二、强调重点
  ```html
  斜体, 应用 *星号*  or _下划线_.

  加粗, 应用 **双星号** or __双下划线__.

  斜体+加粗, 应用 **双星号 and _下划线_**.

  删除线, 应用 ~~双波浪符号~~.
  ```
  斜体, 应用 *星号* or _下划线_.

  加粗, 应用 **双星号** or __双下划线__.

  斜体+加粗, 应用 **双星号 and _下划线_**.

  删除线, 应用 ~~双波浪符号~~.

## 三、列表
  ```html
  1. 第一有序列表项
  2. 另一个列表项
    * 无序子列表. 
  1. 实际的数字并不重要,它只是一个数字
     <!-- 此处子列表项若未与父列表项为对齐,则认为非子列表项 -->
    1. 有序子列表项
  4. 另个一列表项.  

     某些文本应该与父列表项对齐.

  * 无序列表可以使用星号
  - 或者 减号
  + 或者 加号
  ```
  1. 第一有序列表项
  2. 另一个列表项
    * 无序子列表. 
  1. 实际的数字并不重要,它只是一个数字
    1. 有序子列表项
  4. 另个一列表项.  

     某些文本应该与上面的项目对齐.

  * 无序列表可以使用星号
  - 或者 减号
  + 或者 加号

## 四、链接
  有两种方法可以创建链接.
  ```html
  [这是一个内联样式的链接](https://www.baidu.com)

  [这是一个引用样式的链接][大小写不敏感的指向]

  [您可以使用数字来定义的引用样式的链接][1]

  或者直接使用链接 [链接地址]

  url地址和包含尖括号的url地址将自动转换为链接. 
  http://www.example.com or <http://www.singletoworld.com> and sometimes 
  example.com (but not on Github, for example).

  为保障引用链接可跳转需追加链接地址.

  [大小写不敏感的指向]: https://www.mozilla.org
  [1]: http://www.singletoworld.com
  [链接地址]: http://www.singletoworld.com
  ```
  [这是一个内联样式的链接](https://www.baidu.com)

  [这是一个引用样式的链接][大小写不敏感的指向]

  [您可以使用数字来定义的引用样式的链接][1]

  或者直接使用链接 [链接地址]

  url地址和包含尖括号的url地址将自动转换为链接. 
  http://www.example.com or <http://www.singletoworld.com> and sometimes 
  example.com (but not on Github, for example).

  为保障引用链接可跳转需追加链接地址.

  [大小写不敏感的指向]: https://www.mozilla.org
  [1]: http://www.singletoworld.com
  [链接地址]: http://www.singletoworld.com

## 五、图片
  ```html
  这是Markdown的logo (鼠标悬停时可查看标题文本):

  内联样式: 
  ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "这是标志文本 1")

  引用样式: 
  ![alt text][图标]

  [图标]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "这是标志文本 2"
  ```
  这是Markdown的logo (鼠标悬停时可查看标题文本):

  内联样式: 
  ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "这是标志文本 1")

  引用样式: 
  ![alt text][图标]

  [图标]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "这是标志文本 2"

## 六、代码及语法高亮
  *注：Markdown自身支持代码高亮；若要支持语法高亮，具体支持语言请参考<http://softwaremaniacs.org/media/soft/highlight/test.html>*
  ```html
  内嵌的 `代码` 使用 `反单引号`.
  ```
  内嵌的`代码` 使用 `反单引号`.

  代码块要么用带有三个单反引号隔开，要么用四个空格缩进.建议只使用包含反引号的代码块——它们更简单，并且只有反单引号支持语法高亮。
  ```javascript
  var s = "JavaScript语法高亮";
  alert(s);
  ```

  ```python
  s = "Python语法高亮"
  print s
  ```

  ```
  若三个反引号后无任何语言提示,则无法显示语法高亮. 
  But let's throw in a <b>tag</b>.
  ```	

## 七、表格
  表格不是Markdown主要规范的一部分，但是它们是[GFM](https://help.github.com/en/categories/writing-on-github)的一部分，并且Markdown在这里支持它们。
  它们是向电子邮件添加表的一种简单方法——否则，这项任务将需要从另一个应用程序复制粘贴.
  ```html
  冒号可以用来对齐列.

  | Tables        | Are           | Cool  |
  | ------------- |:-------------:| -----:|
  | col 3 is      | 右对齐         | $1600 |
  | col 2 is      | 中央对齐       |   $12 |
  | zebra stripes | are neat      |    $1 |

  The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown.

  Markdown | Less | Pretty
  --- | --- | ---
  *Still* | `renders` | **nicely**
  1 | 2 | 3
  ```
  | Tables        | Are           | Cool  |
  | ------------- |:-------------:| -----:|
  | col 3 is      | 右对齐         | $1600 |
  | col 2 is      | 中央对齐       |   $12 |
  | zebra stripes | are neat      |    $1 |

  最外侧的 (|) 是可选的, 如果不需要让原本的表格看起来漂亮些,可只使用表格内部标记符号即可.

  Markdown | Less | Pretty
  --- | --- | ---
  *Still* | `renders` | **nicely**
  1 | 2 | 3

## 八、块引用
  ```html
  > 块引用在电子邮件中用于模拟回复文本非常方便.
  > This line is part of the same quote.

  Quote break.

  > This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this 
  is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 
  ```
  > 块引用在电子邮件中用于模拟回复文本非常方便.
  > This line is part of the same quote.

  Quote break.

  > This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this 
  is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 

## 九、内联HTML
  你也可以使用原始的HTML,其会同样生效.
  ```html
  <dl>
    <dt>Definition list</dt>
    <dd>Is something people use sometimes.</dd>

    <dt>Markdown in HTML</dt>
    <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
  </dl>
  ```
  <dl>
    <dt>Definition list</dt>
    <dd>Is something people use sometimes.</dd>
    <!-- 此处包含空行时下方无法生效 -->	
    <dt>Markdown in HTML</dt>
    <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
  </dl>

## 十、水平分割线
  ```html
  以下符号需要三个及以上

  ---

  连字号

  ***

  星号

  ___

  下划线
  ```
  以下符号需要三个及以上

  ---

  连字号

  ***

  星号

  ___

  下划线

## 十一、换行符
  对于学习换行如何工作，建议是进行实验并发现——点击<Enter>一次(即，插入新行)，然后按两次(即，插入两行新代码)，看看会发生什么。
  ```html
  Here's a line for us to start with.

  This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

  This line is also a separate paragraph, but...
  This line is only separated by a single newline, so it's a separate line in the *same paragraph*.  
  ```  
    Here's a line for us to start with.

  This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

  This line is also a separate paragraph, but...
  This line is only separated by a single newline, so it's a separate line in the *same paragraph*. 
  
## 十二、音频文件
  音频文件不能直接添加，但你可以添加一个图像并附加视频链接:
  ```html
  <a href="#" target="_blank"><img src="https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png" 
	alt="这是个图片" width="240" height="180" border="10" /></a>
  ```
  <a href="#" target="_blank"><img src="https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png" 
	alt="这是个图片" width="" height="" border="" /></a>
  
  或者，直接使用Markdown，但会失去图像原本的大小和边框:
  ```html
  [![这是个图片](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)](音频地址)
  ```
  [![这是个图片](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)](音频地址)
  
## 十三、TeX数学公式
  此部分对于程序狗一般超出范围，具体请参考原文档<https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet>.	
