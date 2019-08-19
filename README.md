# myBook
# 坚持每天使用琉璃說APP练习英语     ———坚持   杨国涛
## 安装篇
### 安装ubuntu 16.04系统
1.在ubuntu官网下载ubuntu 16.04ISO
2.利用u盘安装ubuntu 16.04系统
3.安装路径
4.空间分配
5.源更新方法
## 安装vscoed
1.在vscoed官网下载vscoed对应的版本安装
###在VScode上安装Markdown插件 
###安装git
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
###2.在w3cshool复习JavaScript的知识（重点）
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

2.10JavaScript JSON操作

    JavaScript Object Notation 简称 JSON，它使用JavaScript对象的格式来存储数据。JSON是灵活的，因为它允许 数据结构 是 字符串，数字，布尔值，字符串，和 对象 的任意组合。
    这里是一个JSON对象的示例：
    var ourMusic = [
    {
    "artist": "Daft Punk",
    "title": "Homework",
    "release_year": 1997,
    "formats": [ 
    "CD", 
    "Cassette", 
    "LP" ],
    "gold": true
    }
    ];
    这是一个对象数组，并且对象有各种关于专辑的 详细信息。它也有一个嵌套的 formarts 的数组。附加专辑记录可以被添加到数组的最上层。
    提示
    数组中有多个 JSON 对象的时候，对象与对象之间要用逗号隔开。

2.11JavaScript 获取JSON属性值

    通过串联起来的点操作符或中括号操作符来访问JSON对象的嵌套属性。
    下面是一个嵌套的JSON对象：
    var ourStorage = {
    "desk": {
    "drawer": "stapler"
    },
    "cabinet": {
    "top drawer": { 
    "folder1": "a file",
    "folder2": "secrets"
    },
    "bottom drawer": "soda"
    }
    }
    ourStorage.cabinet["top drawer"].folder2;// "secrets"
    ourStorage.desk.drawer; // "stapler"

2.12JavaScript 获取JSON数组值

    正如我们在前面的例子所见，JSON对象可以嵌套对象和数组。与访问嵌套对象一样，用中括号操作符同样可以访问嵌套数组。
    下面是如何访问嵌套数组的例子：
    var ourPets = { 
    "cats": [
    "Meowzer",
    "Fluffy",
    "Kit-Cat"
    ],
    "dogs": [
    "Spot",
    "Bowser",
    "Frankie"
    ]
    };
    ourPets.cats[1]; // "Fluffy"
    ourPets.dogs[0]; // "Spot"

2.13JavaScript 使用random()生成随机小数

    随机数对于创建随机行为很有用,计算机的行为只有两种：确定性和随机性。
    而随机数最适合用来创建这种随机行为。
    Math.random()用来生成一个在0(包括0)到1(不包括1)之间的随机小数，因此Math.random()可能返回0但绝不会返回1。

2.14JavaScript 使用random()生成随机数

    用 Math.random() 生成一个随机小数。
    把这个随机小数乘以 20。
    用 Math.floor() 向下取整 获得它最近的整数。
    记住 Math.random() 永远不会返回 1。同时因为我们是在用 Math.floor() 向下取整，所以最终我们获得的结果不可能有 20。这确保了我们获得了一个在0到19之间的整数。

    把操作连缀起来，代码类似于下面：
    Math.floor(Math.random() * 20);
    我们先调用 Math.random()，把它的结果乘以20，然后把上一步的结果传给 Math.floor()，最终通过向下取整获得最近的整数。

2.15JavaScript 使用random()在一个范围内生成随机数

    我们之前生成的随机数是在0到某个数之间，现在我们可以生成一个落在两个特定数字范围内的随机数间。
    我们需要定义一个最小值和一个最大值。
    下面是我们将要使用的方法，仔细看看并尝试理解这行代码正在干什么：
    Math.floor(Math.random() * (max - min + 1)) + min
    例子
    function ourFunction(ourMin, ourMax) {
    return Math.floor(Math.random() * (ourMax - ourMin + 1)) + ourMin;
    }
    ourFunction(1, 9);
    function randomRange(myMin, myMax) {    
    var randomRange=Math.floor(Math.random()*(myMax-myMin+1))+myMin;
    return randomRange; // Change this line
    }
    var myRandom = randomRange(5, 15);

2.16JavaScript 使用正则表达式操作字符串

    Regular expressions 正则表达式被用来根据某种匹配模式来寻找strings中的某些单词。
    例如：如果我们想要找到字符串The dog chased the cat中单词 the，我们可以使用下面的正则表达式: /the/gi
    我们可以把这个正则表达式分成几段：
    / 是这个正则表达式的头部
    the 是我们想要匹配的模式
    / 是这个正则表达式的尾部
    g 代表着 global(全局)，意味着返回所有的匹配而不仅仅是第一个。
    i 代表着忽略大小写，意思是当我们寻找匹配的字符串的时候忽略掉字母的大小写。

2.17JavaScript 使用正则表达式选取空白字符

    我们也可以使用正则表达式选择器 \s 来查找一个字符串中的空白。
    空白字符有 " " (空格符)、\r (回车符)、\n (换行符)、\t (制表符) 和 \f (换页符)。
    空白正则表达式类似于：
    /\s+/g

2.18JavaScript 使用正则表达式反转匹配

    可以用正则表达式选择器的大写版本来反转任何匹配（相反意思）。
    例如：\s 匹配任何空白字符，\S 匹配任何非空白字符。

##学习片
###1.在w3cshool中学习复习Bootstrap的知识
1.1使用Bootstrap设计响应式页面

    Bootstrap会自动获取使用者屏幕的大小,并根据屏幕的大小自动调整HTML元素的宽度和高度来适配屏幕,因此称之为--响应式布局。
    通过响应式布局,你不再需要为你的Web站点重新设计一个手机版的页面,Bootstrap会自动帮你调整好在手机页上的页面显示,事实上,Bootstrap在任何宽度的设备上都能适应得很好。
    使用Bootstrap也非常简单,你只需要把下面的链接添加到你需要使用Bootstrap来进行布局的应用的头部：
    <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap /3.3.1/css/bootstrap.min.css"/>

1.2通过Bootstrap使图片适配手机显示

    通过Bootstrap，我们只要给图片添加 img-responsive 的class属性,图片的宽度就能自动适配你手机屏幕的宽度。

1.3通过Bootstrap使文本居中

    Bootstrap除了可以使图片自适应以外,还可以很简单的让头部标题的文字居中,使标题看起来更美观。我们只需要给h2标签添加text-center的class属性,标题文字就可以居中了。
    提醒：可以使用空格给标签定义多个class,就像下面这样：
    <h8 class="red-text text-center">your text</h8>

1.4为所有按钮添加Font Awesome图标

    Font Awesome是一个方便的图标库。 这些图标都是矢量图形，以.svg文件格式存储。 这些图标可以像字体一样被处理,你可以使用像素设置字体大小一样指定这些图标的大小，并且这些图标可以继承父类HTML标签的字体大小。 

###2.在w3cshool中学习复习jQuery的知识
2.1开始学习jQuery和准备工作

    在我们开始学习使用jQuery之前，需要在HTML文件中添加一些代码。
    首先，在页面顶部添加一行script元素，然后在下一行写上结束符。
    浏览器会运行script里所有的Javascript，包括jQuery。
    在你的script元素里，添加这段代码：$(document).ready(function() {到你的script中，然后在下一行用});结束它。
    接下来我们将学习如何写function，需要注意的是，function里面的代码会在浏览器加载页面后立即运行。
    这很关键，因为在没有document ready function以前，你的代码可能会在HTML渲染完成之前就执行了，这样会产生bug。

2.2jQuery使用选择器获取HTML元素

    现在，我们已经了解了document ready function。
    接下来，让我们开始写第一个jQuery语句，所有jQuery方法都是以$开头，通常称为 美元符号，或者简称为bling。
    jQuery通过选择器来选择一个HTML元素，然后对元素做些改变。
    例如，要让所有的button元素有弹回效果，只要把这段代码写在document ready function里面就可以了：
    $("button").addClass("animated bounce");
    注意，我们已经在后台为你引入了jQuery库和Animate.css库，你可以在编辑器里直接使用这两个库，从而通过jQuery给button元素添加Animate.css的bounce回弹动画效果。

2.3使用jQuery删除HTML元素的class

    你可以通过jQuery的addClass()方法给元素添加class，同样的，也可以通过jQuery的removeClass()方法删除元素的class。
    例子：
    <button class="btn btn-default target" id="target4">#target4</button>
    以下是对button元素执行的操作：
    $("#target2").removeClass("btn-default");

2.4使用jQuery删除一个HTML元素

    jQuery 有一个.remove()的方法，可以彻底删除一个HTML元素。
    使用.remove()方法来删除页面中的target4元素。
    $("#target4").remove();

2.5jQuery使用appendTo()移动HTML元素

    jQuery有一个appendTo()方法，可以让你把选中的HTML元素附加到其他元素中。

    比如，我们想让target4从right-well移动到left-well，我们用以下代码：
    $("#target4").appendTo("#left-well");

2.6jQuery使用clone()方法复制元素

    jQuery有一个clone()方法，可以复制元素。
    例如，如果我们想把target2从left-well复制到right-well，我们用以下代码：
    $("#target2").clone().appendTo("#right-well");

2.7jQuery使用parent()操作父级元素

    每个HTML元素都有一个parent元素，并从中继承属性。
    例如，你的jQuery Playground中的h3元素的父元素是<div class="container-fluid">，<div class="container-fluid">的父元素是body。
    jQuery有一个parent()方法，可以允许你访问选定元素的父元素。
    以下例子显示如何使用parent()设定left-well元素的父元素的背景色为蓝色：
    $("#left-well").parent().css("background-color", "blue")

2.8jQuery使用children()操作子级元素

    许多HTML元素都有children(子元素)，子元素从父元素那里继承属性。
    例如，每个HTML元素都是body的子元素，你的jQuery Playground中的h3元素是<div class="container-fluid">的子元素。
    jQuery有一个children()方法，可以让你访问选定元素的子元素。
    以下例子显示如何使用children()方法设置left-well元素的子元素的文本颜色为蓝色：
    $("#left-well").children().css("color", "blue")

2.9jQuery使用target:nth-child(n) CSS选择器获取子元素

    你已经看到了用jQuery选择器通过id属性来获取元素的是非常方便的，但你不可能总是写这么整齐的id。
    幸运的是，jQuery有一些另外的技巧来获取正确的元素。
    jQuery用CSS选择器来获取元素，target:nth-child(n)CSS选择器允许你通过目标类或元素类型选择目标元素的所有子元素。
    以下代码显示如何给jQuery Playground中的每个井中（left well和right well）的第三个子元素添加bounce类：
    $(".target:nth-child(3)").addClass("animated bounce");

###3.在w3cshool中学习复习初级脚本算法的知识
.split()

    定义和用法
    .split() 方法用于把一个字符串分割成字符串数组。

    语法
    stringObject.split(separator,howmany)

    参数      	描述
    separator 	必需。字符串或正则表达式，从该参数指定的地方分割 stringObject。
    howmany 	可选。该参数可指定返回的数组的最大长度。如果设置了该参数，返回的子串不会多于这个参数指定的数组。如果没有设置该参数，整个字符串都会被分割，不考虑它的长度。

    返回值
    一个字符串数组。该数组是通过在 separator 指定的边界处将字符串 stringObject 分割成子串创建的。返回的数组中的字串不包括 separator 自身。
    但是，如果 separator 是包含子表达式的正则表达式，那么返回的数组中包括与这些子表达式匹配的字串（但不包括与整个正则表达式匹配的文本）。
    提示和注释

    注释：如果把空字符串 ("") 用作 separator，那么 stringObject 中的每个字符之间都会被分割。
    注释：String.split() 执行的操作与 Array.join 执行的操作是相反的。

.reverse()将数组反转

定义和用法
    reverse() 方法用于颠倒数组中元素的顺序。

    语法
    arrayObject.reverse()

    提示和注释
    注释：该方法会改变原来的数组，而不会创建新的数组。

.join("")

    定义和用法
    join() 方法用于把数组中的所有元素放入一个字符串。
    元素是通过指定的分隔符进行分隔的。

    语法
    arrayObject.join(separator)

    参数      	描述
    separator 	可选。指定要使用的分隔符。如果省略该参数，则使用逗号作为分隔符。

    返回值
    返回一个字符串。该字符串是通过把 arrayObject 的每个元素转换为字符串，然后把这些字符串连接起来，在两个元素之间插入 separator 字符串而生成的。

.replace() 方法
    定义和用法
    replace() 方法用于在字符串中用一些字符替换另一些字符，或替换一个与正则表达式匹配的子串。

    语法
    stringObject.replace(regexp/substr,replacement)

    参数 	            描述

    regexp/substr 	
    必需。        规定子字符串或要替换的模式的 RegExp 对象。
    请注意，如果该值是一个字符串，则将它作为要检索的直接量文本模式，而不是首先被转换为 RegExp 对象。

    replacement 	必需。一个字符串值。规定了替换文本或生成替换文本的函数。

    返回值
    一个新的字符串，是用 replacement 替换了 regexp 的第一次匹配或所有匹配之后得到的。

    说明

    字符串 stringObject 的 replace() 方法执行的是查找并替换的操作。它将在 stringObject 中查找与 regexp 相匹配的子字符串，然后用 replacement 来替换这些子串。如果 regexp 具有全局标志 g，那么 replace() 方法将替换所有匹配的子串。否则，它只替换第一个匹配子串。

    eplacement 可以是字符串，也可以是函数。如果它是字符串，那么每个匹配都将由字符串替换。但是 replacement 中的 $ 字符具有特定的含义。

    如下表所示，它说明从模式匹配得到的字符串将用于替换。
    字符 	替换文本
    $1、$2、...、$99 	与 regexp 中的第 1 到第 99 个子表达式相匹配的文本。
    $& 	与 regexp 相匹配的子串。
    $` 	位于匹配子串左侧的文本。
    $' 	位于匹配子串右侧的文本。
    $$ 	直接量符号。

    注意：ECMAScript v3 规定，replace() 方法的参数 replacement 可以是函数而不是字符串。在这种情况下，每个匹配都调用该函数，它返回的字符串将作为替换文本使用。该函数的第一个参数是匹配模式的字符串。接下来的参数是与模式中的子表达式匹配的字符串，可以有 0 个或多个这样的参数。接下来的参数是一个整数，声明了匹配在 stringObject 中出现的位置。最后一个参数是 stringObject 本身。

toLowerCase() 方法

    定义和用法
    toLowerCase() 方法用于把字符串转换为小写。

    语法
    stringObject.toLowerCase()

    返回值
    一个新的字符串，在其中 stringObject 的所有大写字符全部被转换为了小写字符。

charAt() 方法

    定义和用法
    charAt() 方法可返回指定位置的字符。

    请注意，JavaScript 并没有一种有别于字符串类型的字符数据类型，所以返回的字符是长度为 1 的字符串。

    语法
    stringObject.charAt(index)

    参数 	 描述
    index 	必需。表示字符串中某个位置的数字，即字符在字符串中的下标。
    提示和注释

    注释：字符串中第一个字符的下标是 0。如果参数 index 不在 0 与 string.length 之间，该方法将返回一个空字符串。

.indexOf()

    定义和用法
    indexOf() 方法可返回某个指定的字符串值在字符串中首次出现的位置。

    语法
    stringObject.indexOf(searchvalue,fromindex)

    参数   	描述
    searchvalue 	必需。规定需检索的字符串值。
    fromindex 	可选的整数参数。规定在字符串中开始检索的位置。它的合法取值是 0 到 stringObject.length - 1。如省略该参数，则将从字符串的首字符开始检索。

    说明
    该方法将从头到尾地检索字符串 stringObject，看它是否含有子串 searchvalue。开始检索的位置在字符串的 fromindex 处或字符串的开头（没有指定 fromindex 时）。如果找到一个 searchvalue，则返回 searchvalue 的第一次出现的位置。stringObject 中的字符位置是从 0 开始的。

    提示和注释
    注释：indexOf() 方法对大小写敏感！
    注释：如果要检索的字符串值没有出现，则该方法返回 -1。
