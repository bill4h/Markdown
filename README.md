# Markdown
## 一、啥是Markdown
Markdown是一种轻量级标记语言，创始人是约翰·格鲁伯。它允许人们使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML(或者HTML)文档。这种语言吸收了很多再电子邮件中已有的纯文本标记的特性。(如果你认真读完了，那么恭喜你，这段来自百度百科，你可以百度一下，再读一遍)。
  
按我的理解，就是使用一些特定的符号，诸如：# = - ...等符号来修饰你的文本内容，使其能够在一些平台上被转换成XHTML或HTML的格式，更好地做内容输出。
   
Markdown具体的产生和历史，感兴趣的小伙伴可以自行了解。详情可参见：[younghz/Markdown](https://github.com/younghz/Markdown.git)   

本文主要是记录Markdown的常见用法，以防作者“提前进入老年期”，忘东忘西，便于日后自己查找使用。

*PS：接下来在文中将使用**MD**来代指Markdown。*

## 二、文本格式篇

### 1 文本标题

#### 1.1 MD写法1：

> 1级标题 使用 =  
> 2级标题 使用 -   
> **使用特点**：需在文本中占据两行，第1行是标题内容，第2行是**至少三个连续相同**的 = 或 - <br>具体格式如下：
>
> 1级标题   
>`=======`
>
> 2级标题   
>`-------`
    
#### 1.2 写法1效果：

> # 1级标题
> ## 2级标题

#### 1.3 MD写法2：

> 使用 **#** 表示1-6级标题。   
> `#`  1级标题   
> `##`  2级标题   
> `###`  3级标题   
> `####`  4级标题   
> `#####`  5级标题   
> `######`  6级标题   

#### 1.4 写法2效果：

> #  1级标题
> ##  2级标题
> ###  3级标题
> ####  4级标题
> #####  5级标题
> ######  6级标题
>
> 综上所述，我选择写法2... 毕竟它更好记。

### 2 段落

#### 2.1 MD写法

> 前1行和后1行都是**空行**的文本内容，就是段落。  
> 所以段落就是被**两空行夹击**的。       
>
> ~~(段落前空行，这行不能有东西，谢谢配合)~~
>  
> 我是段落内容，巴拉巴拉巴拉...   
> 我是段落内容，巴拉巴拉巴拉...   
> 我是段落内容，巴拉巴拉巴拉...   
>
> ~~(段落后空行，这行不能有东西，谢谢配合)~~

#### 2.2 段落效果-没换行：

我是段落内容，巴拉巴拉巴拉...
我是段落内容，巴拉巴拉巴拉...
我是段落内容，巴拉巴拉巴拉...

> 哦吼？？？为啥这里的展示，与我在MD中写的格式不一样？  
> 我明明就有在每行后面添加**回车键(Enter)**,为啥到了你这就变成都显示在一行了呢？  
>
> ~~拿出小本本：这里要画起来。虽然它不考...~~  
>
> 在段落文本中，若要进行换行，仅使用一个回车键(Enter)是达不到换行效果的。  
> 要使用 **2个空格(space) + 1个回车键(Enter)** 或者 **`<br>`标签** 来实现段落内换行的操作。
> 
> 我是段落内容，巴拉巴拉巴拉... ~~(2个space + 1个Enter)~~  
> 我是段落内容，巴拉巴拉巴拉... `<br>`<br>
> 我是段落内容，巴拉巴拉巴拉...
>

#### 2.3 段落效果-换行：

我是段落内容，巴拉巴拉巴拉...  
我是段落内容，巴拉巴拉巴拉...  
我是段落内容，巴拉巴拉巴拉...

### 3.区块引用

> 在行的开头使用 > 可以进行区块引用，啥意思呢？  
> 与上面的**段落效果-换行**相比较，当前行的开头是有一个竖条的，表示说我当前行是一个区块。<br>
> 区块可以让我们将内容进行分块展示，使得整体的文章结构更清晰明了。<br>
> 区块可以是单个，也可以是多个(嵌套引用)。<br>
>
#### 3.1 MD写法：

> `>` 区块引用<br>
> `>>` 嵌套引用<br>
> `>>>` 嵌套引用+1<br>

#### 3.2 区块(嵌套)引用效果：

> 区块引用
>> 嵌套引用
>>> 嵌套引用+1


### 4.代码区块
> 当需要在文中show出你的代码时，可以使用代码区块来进行展示。<br>
> 代码区块是在代码的每行开头使用 **制表符(Tab)** 或者 **4个空格(space)** 来表示。<br>
#### 4.1 MD写法：

>~~(Tab)~~     public class HandsomeBoy{<br>
>~~(4个space)~~     private final String name = "bill4h";<br>
>~~(Tab)~~     }<br>

#### 4.2 代码区块效果：

    public class HandsomeBoy{
        private final String name = "bill4h";
    }

