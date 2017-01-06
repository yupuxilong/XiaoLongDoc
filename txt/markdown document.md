#Mardown
![](http://i.imgur.com/CPSlHqI.jpg "Angry me")

[**## reference ##**](https://www.zybuluo.com/AntLog/note/63228#题记)
##正文
###1.Markdown是什么

- **Markdown**是一种轻量级标记语言，它以纯文本形式(易读、易写、易更改)编写文档，并最终以HTML格式发布。你可以导出 HTML 格式的文件用来网站发布，也可以十分方便的导出 PDF 格式.
- **Markdown**也可以理解为将以MARKDOWN语言编写的语言转换成HTML内容的工具，最初是一个perl脚本Markdown.pl.
###2.语法
Markdown语法主要分为如下几大部分： 标题，段落，区块引用，代码区块，强调，列表，分割线，链接，图片，反斜杠 \，符号'`'。
####2.1 标题
使用#，可表示1-6级标题。
>\# 一级标题  
>\## 二级标题  
>\### 三级标题  
>\#### 四级标题  
>\##### 五级标题  
>\####### 六级标题（依次类推）

效果如下
># 一级标题
>## 二级标题
>### 三级标题
>#### 四级标题
>##### 五级标题
>###### 六级标题（依次类推）

####2.2 段落
段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用两个以上空格加上回车（引用中换行省略回车）。
####2.3 区块引用
在段落的每行或者只在第一行使用符号>,还可使用多个嵌套引用，如：
> \> 区块引用  
> \>> 二级嵌套引用  
> \>>> 三级嵌套引用（依次类推）

效果如下：
> 区块引用  
>> 二级嵌套引用  
>>> 三级嵌套引用（依次类推）
####2.4 代码区块
代码区块的建立是在每行加上4个空格或者一个制表符（如同写代码一样）；或者快捷键Ctrl+k；
如普通段落：  
void main(){  
   printf("Hello, Markdown.");  
} 
 
代码区块：
  
    void main(){
        printf("Hello, Markdown.");
    }

```
var canvas = document.getElementById("canvas");  
var context = canvas.getContext("2d"); 
```

**注意:需要和普通段落之间存在空行。**

#### 2.5 强调

在强调内容两侧分别加上*或者_，如：

>\*斜体\*，\_斜体\_  
>\*\*粗体\*\*，\_\_粗体\_\_   

效果：

>*斜体*， _斜体_  
>**粗体**， __粗体__


#### 2.6 列表

使用·、+、或-标记无序列表，如：

>\- 第一项  
>\- 第二项

__注意：标记后面最少有一个空格或制表符。若不在引用区块中，必须和前方段落之间存在空行。__

效果：

>- 第一项
>- 第二项

有序列表的标记方式是将上述的符号换成数字,并辅以.，如：

>1. 第一项  
>2. 第二项  
>3. 第三项  
2016/6/16 星期四 18:19:22 2016/6/16 星期四 18:19:23 2016/6/16 星期四 18:19:25 
效果：

>1 .第一项  
>1 .第二项  
>1 .第三项  

#### 2.7 分割线

分割线最常使用就是三个或以上*，还可以使用-和_。如：  
\****  
\---  
\___   
\* \* \*  
效果：  
***  
---  
___
* * *  
#### 2.8 链接

链接可以由两种形式生成：行内式和参考式。
行内式：

>\[younghz的Markdown库](https:://github.com/younghz/Markdown "Markdown")

效果：  
[younghz的Markdown库](https:://github.com/younghz/Markdown "Markdown")  
参考式：
>\[younghz的Markdown库1]\[1]  
>\[younghz的Markdown库2]\[2]  
>\[1]:https:://github.com/younghz/Markdown "Markdown"  
>\[2]:https:://github.com/younghz/Markdown "Markdown"  

效果：
>[younghz的Markdown库1][1]  
>[younghz的Markdown库2][2]  
>[1]:https:://github.com/younghz/Markdown "Markdown"  
>[2]:https:://github.com/younghz/Markdown "Markdown"  

**注意：上述的[1]:https:://github.com/younghz/Markdown "Markdown"不出现在区块中。**

#### 2.9 图片
- 添加网络图片的形式和链接相似，只需在链接的基础上前方加一个！。
- 添加本地图片则需通过菜单栏-->插入-->浏览并上传，默认生成形式：
\!\[](http://i.imgur.com/CPSlHqI.jpg)


#### 2.10 反斜杠\

**相当于反转义作用。使符号成为普通符号。**

#### 2.11 符号'`'

起到标记作用。如：

\`ctrl+a\`

效果：

`ctrl+a`

#### 2.12 注脚 ####
使用 [^footer] 表示注脚。

如:  
这是一个注脚测试\[^footer1]。  
效果：  
这是一个注脚测试[^footer1]
[^footer1]: 这是一个测试，用来阐释注脚。

#### 2.xx 常用字符（更新中...）
- 版权&copy;（&+copy+;） 

### 3.扩展

Markdown的已写扩展功能

#### 3.1 表格
表格扩展的激活方法：tool-->options-->Markdown-->Mrakdown处理器-->markdown（扩展）

表格的使用，如：  

\|Name|Gender|Age|  
\|-|--|-|  
\|a|b|c|  
\|a|b|  
\|a|b|c|d|  

效果：

|Name|Gender|Age|
|-|--|-|
|a|b|c|
|a|b|
|a|b|c|d|

**注意：第二行是表示默认的列数，实际列数不受其约束。**

#### 3.2 公式 ####


#### 3.3 生成目录 ####

* [1.语法示例](#1)

* [1.1图片](#1.1)

* [1.2换行](#1.2)

* [1.3强调](#1.3)

#### 3.4 html tags ####
[http://www.w3school.com.cn/tags/att_standard_id.asp](http://www.w3school.com.cn/tags/att_standard_id.asp)



*By Justice* 2016/6/16 星期四 18:20:01 



