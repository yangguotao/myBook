# myBook
#坚持每天使用琉璃說APP练习英语     ———坚持
##安装篇
###安装ubuntu 16.04系统
1.在ubuntu官网下载ubuntu 16.04ISO
2.利用u盘安装ubuntu 16.04系统
3.安装路径
4.空间分配
5.源更新方法
##安装vscoed
1.在vscoed官网下载vscoed对应的版本安装
##在VScode上安装Markdown插件 
##安装git
1.安装git==》sudo apt-get install git-core
2.一些全局变量的初始化
    在本地建立一个文件夹，然后做一些全局变量的初始化
    git config --global user.name 用户名或者用户ID
    git config --global user.email 你邮箱
    这两个选项会在以后你提交代码至本地仓库时自动填写到你的提交记录中去.

##复习篇
###1.在w3cshool复习H5的知识
1.1开始学习HTML标签 
1.2HTML 学习h2标签
1.3HTML 学习p标签
1.4删除HTML的注释
1.5HTML注释语句学习
1.6HTML用占位符文本填补空白
1.7删除HTML标签
1.8HTML 更换文本的颜色
1.9使用CSS选择器定义标签
1.10使用一个CSS Class去给标签定义Style
<style>
.red-text{
color: red;
}
</style>
1.11HTML 为多个元素使用CSS类定义样式

<style>
.red-text {
color: red;
}
</style>

<p2 class="red-text">html编程入门教程</p2>

<p class="red-text">在大家心目中，也许编程是一件非常困难的事情，其实也是一件非常有乐趣的事情，只要掌握好编程入门的方法，就能慢慢进入一个全新的创造世界。</p>

1.12HTML HTML 设置标签的字体大小
<style>
  .red-text {
    color: red;
  }
  p{
  font-size:16px;
  }
</style>

1.13HTML 设置标签的字体样式
1.14引入Google字体
<style>
.red-text {
color: red;
font-family:Lobster;
}
p {
font-size: 16px;
font-family: Monospace;
}
</style>
1.15HTML 处理多个字体降级
1.16HTML 给页面添加图片
1.17HTML 调整网页里图片大小
1.18HTML 给标签增加边框
1.19HTML 给标签增加圆角边框
1.20HTML 给图像设置圆角边框
1.21HTML 设置链接锚元素外部页面
1.22HTML 在p标签内设置锚链接
1.23HTML 使用#符合设置固定链接

<p>Click here for <a href=#>cat photos</a>.</p>

1.24HTML 为图片设置超链接
1.25HTML 为图片添加alt描述

1.26HTML 创建项目符号无序列表
1.27HTML 创建有序列表
1.28HTML 创建文本输入框
1.29HTML 为文本输入框设定预定值
1.30HTML 添加表单
1.31HTML 为表单添加提交按钮
1.32HTML 使用HTML5技术把表单设置为必填
1.33HTML 添加单选框
1.34HTML 添加复选框
1.35HTML 使用checked属性设置复选框和单选框默认被选中

<label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>

1.36HTML 在div元素中嵌套多个元素
1.37HTML 为div元素设置背景颜色
1.38HTML 为标签添加ID属性
1.39HTML 使用ID属性设置标签样式
1.40HTML 使用padding布局页面标签
1.41HTML 使用margin布局页面标签
1.42 HTML 使用负值设置页面元素的margin属性
1.43 HTML 为不同方向padding设置不同的值
1.44 HTML 为不同方向margin设置不同的值
1.45 HTML CSS中padding简写
1.46 HTML CSS中margin简写
1.47 CSS 样式的继承
1.48 CSS 继承Body元素样式
1.49 CSS 样式的覆盖
1.50 CSS 多个class处理样式覆盖
1.51 CSS 通过ID的样式属性覆盖class类的声明
1.52 CSS 通过内联样式覆盖class类的声明
1.53 CSS 通过使用Important覆盖所有其他样式
1.54 CSS 通过使用十六进制代码设置特定的颜色
1.55 CSS 十六进制白色表达方式
1.56 CSS 十六进制RGB红色表达方式
1.56 CSS 十六进制RGB绿色表达方式
1.56 CSS 十六进制RGB蓝色表达方式
1.57 CSS 十六进制RGB混合颜色
1.58 CSS 灰色度设置
1.59 CSS 不同等级的灰度设置
1.60 CSS 十六进制RGB表达式缩写
1.61 CSS 使用rgb属性设定颜色
1.62 CSS 使用rgb属性设定白色
1.63 CSS 使用rgb属性设定红色
1.64 CSS 使用rgb属性设定绿色
1.65 CSS 使用rgb属性设定蓝色
1.66 CSS 使用rgb属性设定混合颜色
###2.在w3cshool复习JavaScript的知识
2.1理解JavaScript未定义变量

var a=5;
var b=10;
var c="I am a";

a = a + 1;
b = b + 5;
c = c + " String!";

2.2理解JavaScript变量的大小写敏感性
使用 驼峰命名法 来设置一个 Javascript 变量，在 驼峰命名法 中，变量名的第一个单词的首写字母小写，后面的单词的第一个字母均为大写。
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
2.3JavaScript 转义字符串中的引号
当你定义一个字符串时，你必须以单引号或双引号作为开头和结尾。那么当你需要在字符串中使用一个: " 或者 ' 时该怎么办呢?
在 JavaScript 中，你可以通过在引号前面使用 反斜杠 (\) 来转义引号。
var sampleStr = "Alan said, \"Peter is learning JavaScript\".";
2.4JavaScript 队列
在计算机科学中 队列（queue）是一个抽象的数据结构，队列中的数据条目都是有秩序的。新的条目会被加到 队列 的末尾，旧的条目会从 队列 的头部被移出。
写一个函数 queue ，用一个数组arr和一个数字item作为参数。数字item添加到数组的结尾，然后移出数组的第一个元素，最后队列函数应该返回被删除的元素。
function queue(arr, item) {
// Your code here
        arr.push(item);
        item=arr.shift();
return item;// Change this line
}
// Test Setup
var testArr = [5,6,7,8,9];
// Display Code
console.log("Before: " + JSON.stringify(testArr));
console.log(queue(testArr, 10)); // Modify this line to test
console.log("After: " + JSON.stringify(testArr));

2.5JavaScript 使用中括号索引查找字符串中的第N个字符

你也可以使用 [索引]来获得一个字符串中的某个位置的字符。
请记住，计算机是从 0 开始计数，所以获取第一个字符的索引实际上是[0]。
var firstName = "Ada";
var secondLetterOfFirstName = firstName[1];

// Setup
var lastName = "Lovelace";
// Only change code below this line.
var thirdLetterOfLastName = lastName[2];

2.6Javascript 字符串操作综合训练

现在我们将结合之前学习的字符串相关知识，来玩一个填字风格的文字游戏。
通过使用提供的变量：名词myNoun、形容词myAdjective、动词myVerb、副词myAdverb，来创建一个新的字符串并赋值到 result。
此外，除了所提供的词之外，你还需要添加额外的连接字符串。
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
var result = "";
// Your code below this line
result=myNoun+','+myAdjective+','+myVerb+','+myAdverb;
// Your code above this line
return result;
}
// Change the words here to test your function
wordBlanks("cat", "little", "hit", "slowly");

2.7JavaScript push()函数追加数组数据

将数据追加到一个数组末尾的最简单的方法是通过 push() 函数
var ourArray = ["Stimpson", "J", "cat"];
ourArray.push(["happy", "joy"]); 
 ourArray now equals ["Stimpson", "J", "cat", ["happy", "joy"]]
 Setup

 var myArray = [["John", 23], ["cat", 2]];
myArray.push(["dog",3]);

2.8JavaScript pop()函数弹出数组最后数据

.pop() 函数用来“抛出”一个数组末尾的值。我们可以把这个“抛出”的值赋给一个变量存储起来。
数组中任何类型的数据条目（数值，字符串，甚至是数组）可以被“抛出来” 。

举个例子, 对于这段代码
var oneDown = [1, 4, 6].pop();
现在 oneDown 的值为 6 ，数组变成了 [1, 4]

2.9JavaScript shift()函数移出数组第一个数据

.shift() 就是专门用来处理这类型需求的。它的工作原理类似 .pop()，但它移除的是第一个元素，而不是最后一个。
var ourArray = ["Stimpson", "J", ["cat"]];
removedFromOurArray = ourArray.shift();
var myArray = [["John", 23], ["dog", 3]];
var removedFromMyArray=myArray.shift();
结果为：myArray = [["dog",3]] & removedFromMyArray = ["John",23]


##学习片
###1.在w3cshool中学习复习Bootstrap的知识
###2.在w3cshool中学习复习jQuery的知识
###3.在w3cshool中学习复习初级脚本算法的知识

