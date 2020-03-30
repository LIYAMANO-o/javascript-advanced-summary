# javascript-advanced-summary
《深入理解javascript》   
第一章 基础JavaScript  
一个单独的等于号（=），用于为变量赋值    三个连续的等于号（===），用于比较两个值  
一、语句和表达式  
语句：用来声明（或创建）一个变量 var foo;   表达式：表达式产生值  
二、分号  
分号用于结束语句，而不是数据块  
三、注释  
单行注释：由两个斜杠//开始  多行注释：限定在/*和*/之间  
四、变量和赋值  
JavaScript里的变量在声明后使用 var foo;变量声明和赋值可以同时进行 var foo=6; 也可以为一个已有变量进行赋值 foo=4；  
五、值    
在JavaScript中所有的值都有属性，每一个属性都有一个key（或者是name）和一个value，通过点（.）操作符可以读取属性 value.propkey，点操作符同样可以用于给属性赋值，也可以通过点操作符来调用方法。  
六、原始值和对象  
原始值包括布尔值、数字、字符串、null和undefined，其他的值都是对象。原始值特点：按值进行比较、不可改变  
七、对象  
简单对象：可以通过对象字面量来创建。数组：可以通过数组字面量来创建。正则表达式：可以通过正则表达式字面量来创建。  
对象特点：按引用进行比较、默认可变  
八、undefined和null  
undefined的意思是“没有值”，未被初始化的变量即为undefined，丢失的参数也会是undefined。  
null的意思是“没有对象”。在用到对象的时候它表示空值。  
使用typeof和instanceof对值分类  
typeof用法形如：typeof value   instanceof用法形如： value instanceof constr  
布尔值：原始布尔类型包含true和false两个值  
二元逻辑运算符：与、或、非  
等式运算符：常规的，或“宽松的”相等（或不相等）：==和！=  严格的相等：===和！==  
数字：JavaScript中所有的数字都是浮点数，也包含一些特殊的数字：NAN，infinity  
运算符：加法、减法、乘法、除法、取模、增量、减量、负数、转变成数字  
字符串：反斜杠\用于转义字符及产生一些控制字符，可以通过方括号来访问字符串中的单个字符，字符串的length属性可以对字符的个数进行计数。  
字符串运算符：字符串可以通过加号进行连接，如果其中一个运算数是字符串的话，另一个运算数将被转换成字符串。  
字符串方法：slice、trim、indexof...  
语句：条件语句：if语句有一个then从句以及一个可选else语句、switch语句  
循环语句：for循环、while循环、do-while循环  
break可以跳离循环 continue会开始一个新的循环迭代  
函数：可以通过函数声明的方式来定义函数。  
特殊的变量：arguments  在JavaScript中，函数的所有参数都可以被自由调用，它会通过arguments变量来使所有参数可用。  
强制参数长度：arguments.length  
将arguments转换为数组：function toArray(arrayLikeObject){  
return Array.prototype.slice.call(arrayLikeObject);  
}  
异常捕获：使用try语句包裹关键代码，如果try语句有异常会被抛出那么catch语句就会执行。  
严格模式：激活更多的警告以及使JavaScript变得更干净，要切换到严格模式，在JavaScript文件或者<script>标签第一行输入：'use strict'；  
变量作用域和闭包：在变量前使用var语句声明变量，可以使用单个var语句声明和初始化多个变量。  
变量的提升特性：声明会被移动到函数的开始处，而赋值则仍然会在原来的位置进行。闭包：create Incrementor()的返回其实就是一个闭包。  
八、对象和构造函数  
  单一对象：在JavaScript中，可以直接通过对象字面量去创建普通对象，可以获取get以及设置set属性以及使用this对调用它们的对象进行引用，使用in运算符检查属性是否存在。  
  方法中的函数：将this保存在不同的变量中、利用foreach的第二个参数，它可以给this指定一个值。构造函数：构造函数包含两部分，第一部分，point函数
设置实例数据。第二部分，point.prototype属性包含一个带有方法的对象。通过new运算符来使用point：var p=new point(3,5);  
  九、数组  
  数组字面量可以方便地创建数组元素、length属性表明数组有多少元素、in操作符也可以在数组中正常使用。  
  数组方法：slice  push  pop  shift   unshift  indexof...  
  遍历数组：foreach以及map  
  十、正则表达式  
  test()方法：匹配吗、exec（）方法：匹配以及捕获分组、replace()方法：搜索和替换  
  标准库和其他功能：Date、JOSN  
  第二章  为什么选择JavaScript  
  JavaScript语言的规范，他是一个ISO标准，有着许多独立的实现，其中一些是开源的。  
  类库：JavaScript有大量的类库，从解系JavaScript到处理和显示PDF文件。  
  Node.js 允许编写服务端代码以及shell脚本  
  JSON 是一种基于JavaScript的数据格式，已经成为网上流行的数据交换格式  
  NoSQL 数据库  
  JavaScript被广泛使用，好处：JavaScript相关的文档和各式各样的支持、JavaScript开发人员需求量大。  
  JavaScript有一个光明的未来：语言是稳步发展的、有许多JavaScript相关的创新、JavaScript的网络平台是一个必须的组成部分，正在迅速成熟、JavaScript是被联盟广泛支持的，而不是被单独的人或公司控制。  
  
  
  
  《你不知道的JavaScript》  
  第一章  类型  
  七种内置类型：空值、未定义、布尔值、数字、字符串、对象、符号  
  使用typeof运算符查看值的类型，JavaScript中的变量时没有类型的，只有值才有。变量在未持有值的时候为undefined，此时typeof返回undefined。  
  JavaScript有七种内置类型：null   undefined  boolean   number  string  object  symbol   
  第二章 值  
  数组  数组可以容纳任何类型的值，使用delete可以将单元从数组中删除 类数组  
  字符串不是字符数组，字符串不可变，数组可变。字符串不可变是指字符串的成员函数不会改变其原始值，而是创建并返回一个新的字符串。  
  JavaScript中的数字常量一般用十进制表示，数字前面的0也可以省略，小数点后小数部分最后面的0也可以省略。  
  整数的检测Number.isinteger()  
  undefined类型只有一个值，即undefined。void，undefined是一个内置标识符，他的值为undefined，通过void运算符即可得到该值。  
  NAN not a number  
  简单值  JavaScript中的数组是通过数字索引的一组任意类型的值，字符串和数组类似，但是他们的行为特征不同。基本类型中定义了几个特殊的值。null类型只有  一个值null，undefined类型也只有一个值undefined，所有变量在赋值之前默认值都是undefined，void运算符返回undefined，数字类型有几个特殊值包括NAN。  
  第四章  强制类型转换  
  对象的toString  
一般对象的toString方法，将会显示该对象的[[class]]  
数组的toString  
数组由于自身重写过toString方法，数组的toString方法会返回逗号连接的字符串  
JSON.stringify()  
JSON.stringify()方法用于将数据转换为JSON格式的字符串，但是对于undefined, function, symbol类型的数据，在转换时会选择抛弃，从而返回undefined  转换对象在数组中时，这些值会被赋值为null  如果转换对象出现循环引用，那么在转换的时候会抛出异常。  
为了使得我们所有的对象在转换成JSON字符串的时候可以正常转换，我们可以定义toJSON方法，该方法在JSON.stringify调用前会进行调用，对数据进行处理
对象转Number  
遵循toPrimitive的规则，如果对象存在valueOf方法，则调用该方法，如果调用后返回的结果为基本类型
toBoolean
boolean类型转换过程只会进行真假值的检查，其中假值包括: false, '', null, undefined, NaN, +0, -0，假值将会转换为false，假值以外的其他值均为真值，转换为true
对于一个特殊的对象Object.create(null)，由于原型链的继承关系，该对象不继承Object，所以不存在valueOf和toString方法，那么在进行转换的时候将抛出异常
显示类型转换
String()和Number()转换
按照基本类型转换 的toString和toNumber的规则进行转换
一元运算符转换
使用一元运算符(+, -)会将数据转换为number类型，相当于Number(data)
symbol()对象转换
Symbol对象不能通过隐式转换进行，如果要进行转换必须使用构造方法来显示转换（似乎只能转为字符串）。
隐式类型转换
逻辑语句中的类型转换
作为逻辑语句中的判断条件，将转换为boolean值进行处理
||和&&
||和&&的操作，返回结果并不是boolean值，而是根据短路规则，判断操作数的Boolean()结果，返回两个操作数的其中之一，其中||在true时进行短路返回，&&在false时进行短路返回
  
  
《深入理解JavaScript》  
第八章 值  
一、JavaScript中的类型体系  
1.JavaScript类型  
ECMAscript语言类型包括：undefined,null,Boolean,String,Number,Object  
2.静态与动态  
静态一般是指“编译时”或者“非运行时”，动态指的是“运行时”。  
3.静态类型与动态类型  
在静态类型语言中，变量、参数和对象成员都有编译器编译时能识别的类型。在动态类型语言中，变量依然有一个动态的类型，是指在某一时刻变量值的类型。  
JavaScript是动态类型的语言，变量的类型在编译的时候是不确定的。  
4.静态类型检查和动态类型检查  
静态类型检查语言会在编译期间进行检查， 动态类型检查语言会在执行期间进行检查。  
5.强制转换  
二、原始值和对象  
1.原始值  
布尔值：true,false  
数字：1736,1.351  
字符串：'abc',"abc"  
两个空值：undefined，null  
原始值特点：①按值进行比较  
②不可改变  
③固定类型组合  
2.对象  
简单对象，可以通过对象字面量来创建  
数组，可以通过数组字面量来创建 ['apple', 'banana' , 'cherry']  
正则表达式，可以通过正则表达式字面量来创建。  
对象特点：①按引用进行比较  
②默认可变  
③用户可扩展  
三、undefined和null  
1.undefined和null的出现场景  
undefined出现的场景  
未初始化的变量是undefined：var foo;  foo;  
缺失的参数是undefined：function f(x){return x}  f();  
如果访问一个不存在的属性，会返回undefined：var obj={}; obj.foo  
如果函数中没有显式地返回任何值，函数会隐式返回undefined：function f() {}  
null的出现场景  
null是原始链最顶端的元素 Object.getPrototypeOf(Object.prototype)  
当字符串中没有匹配到正则表达式的结果时，RegExp.prototype.exec()会返回null  
2.检测undefined和null  
检测null  
通过严格相等检测null：if(x===null)...  
检测undefined  
通过严格相等检测undefined：if(x===undefined)...  
也可以通过typeof运算符检测undefined  
检测undefined或null  
有一种显式的比较方式用来检测他们：if(x!==undefined&&x!==null){...}  
另一种检测方式是利用undefined和null都可被认为是false的特性：if(x){...} if(!x){...}   
3.undefined和null的历史  
遇到未初始化的变量和缺失的参数等异常情况时需要一个值来表示，null是一个很好的选择，但是要避免两种情况：  
这个值不应该具有指向性，因为它表达的不仅仅是一个对象  
这个值强制转换不应该为0，因为这会使错误难以发现  
因此，将undefined作为另外一个空值加进了JavaScript。  
4.修改undefined  
技巧一：隐藏全局undefined（因为它可能是错误的值）  
(function (undefined){
if(x===undefined)...
}());  
技巧二：和'void 0'进行比较，'void 0'总是undefined if(x===void 0)  
四、原始值的包装对象  
1.包装对象不同于原始值  
包装实例是对象  
2.原始值的包装与去包装  
通过调用包装构造函数来对原始值进行包装：  
new Boolean(true)  
new Number(123)  
new String('abc')  
通过调用valueOf()来对原始值进行去包装  
new Boolean(true).valueOf()  
new Number(123).valueOf()  
new String('abc').valueOf()  
把包装对象转换为原始值时只能正确地提取出数字和字符串，二布尔值则不能。  
Boolean(new Boolean(false))  
Number(new Number(123))  
String(new String('abc'))  
3.原始值从包装器借调方法  
'abc'.charAt===String.prototype.charAt  
在宽松模式中，原始值会在运行过程中转换为包装器：  
String.prototype.sloppyMethod=function(){
console.log(typeof this);  
console.log(this instanceof String);  
};  
''.sloppyMethod();  
在严格模式中，对包装器原型调用是透明的  
String.prototype.sloppyMethod=function(){
'use strict';  
console.log(typeof this);  
console.log(this instanceof String);  
};  
''.sloppyMethod();   
五、强制类型转换  
1.强制类型转换会隐藏bug  
2.转换成布尔值、数字、字符串和对象的函数  
Boolean() 转换为布尔值。 undefined，null，false，0，NAN，'' 转换为false  
Number() 转换为数字。 undefined会转换成NaN。  
null会转换成0。  
false会转换成0，true 会转换成1。  
字符串会被解析。  
对象会先转换为原始值，然后再转换为数字。  
String() 转换为字符串。  
Object() 对象会转换为它们自身，undefined和null会转换成空对象，而原始值会转
换为包装后的原始值。  
3.算法：ToPrimitive() 将值转换为原始值  
ToPrimitive(input, PreferredType?)  
(1)如果input是原始值，返回这个值(没有其他需要做的)。  
(2)否则，如果input是对象，调用input. value0f()。如果结果是原始值，
返回结果。  
(3)否则，调用input. toString()。如果结果是原始值，返回结果。  
(4)否则，抛出一一个TypeError (说明将输入转换为原始值出错了)。  
如果PreferredType是字符串，第二步和第三步会进行交换。PreferredType 也可以
被省略，这种情况下，日期会被认为是String而其他值会被认为是Number.因此，
+运算符和== =运算符可以操作ToPrimitive()。  

《JavaScript权威指南》  
第三章 类型、值和变量  
一、数字  
1.整型直接量
在JavaScript程序中，用一个数字序列来表示一个十进制整数。JavaScript同样能识别十六进制值，但在  
ECMAscript6的严格模式下，八进制直接量是明令禁止的。  
2.浮点型直接量  
浮点型直接量可以含有小数点  
3.JavaScript中的算数运算  
运算符：加法运算符(+) 、减法运算符(-)、乘法运算符(*) 、除法运算符(/) 和求余(求整除后的余数)运算符(%)   
JavaScript预定义了全局变量infinity和NAN，用来表示正无穷大和非数字值。  
4.二进制浮点数和四舍五入错误  
当在JavaScript中使用实数的时候，常常只是真实值的一个近似表示。  
5.日期和时间  
Date()构造函数 var then = new Date(2011, 0, 1); /1 2011年1月1日  
var later = new Date(2011, 0, 1, 17, 10，30);// 同一天，当地时间5:10:30pm,  
varnow口newDate();//当前日期和时间  
var elapsed = now - then; //日期减法:计算时间间隔的毫秒数  
later . getFullYear() // => 2011  
later . getMonth() /1 => 0;从0开始计数的月份  
later . getDate() // => 1:从1开始计数的天数   
later. .getDay() // => 5:得到星期几，0代表星期日， 5代表星期一  
later . getHours() // =>当地时间17: 5pm  
later . getUTCHours() //使用UTC表示小时的时间，基于时区  
二、文本  

《JavaScript权威指南》
第8章

#### prototype属性  
每一个函数都包含一个prototype属性，这个属性是指向一个对象的引用，这个对象称做“原型对象”(prototype object)。每一个函数都包含不同的原型对象。当将函数用做构造函数的时候，新创建的对象会从原型对象上继承属性。  
#### toString()方法  
和所有的JavaScript对象一样，函数也有toString()方法，ECMAScript规范规定这个方法返回一个字符串，这个字符串和函数声明语句的语法相关。实际上，大多数(非全部)的toString()方法的实现都返回函数的完整源码。内置函数往往返回一个类似“[Inative code]”的字符串作为函数体。  

#### 函数调用形式  
1. 作为函数直接调用  
2. 作为对象方法调用  
3. 作为构造函数调用  
4. 通过 call/apply 间接调用  
以上是调用的四种方法  
##### 函数调用  
1. 在一个调用中，每个参数表达式(圆括号之间的部分)都会计算出一个值，计算的结果作为参数传递给另外一个函数。这些值作为实参传递给声明函数时定义的形参。在函数体中存在一个形参的引用，指向当前传人的实参列表，通过它可以获得参数的值。  
2. 对于普通的函数调用，函数的返回值成为调用表达式的值。如果该函数返回是因为解释器到达结尾，返回值就是undefined.如果函数返回是因为解释器执行到一条return语句，返回值就是return之后的表达式的值，如果return语 句没有值，则返回undefined.  
3. 根据ECMAScript 3和非严格的ECMAScript 5对函数调用的规定，调用上下文(this的值)是全局对象。然而，在严格模式下，调用上下文则是undefined.  
4. 以函数形式调用的函数通常不使用this关键字。不过，“this” 可以用来判断当前是否是严格模式。  
##### 方法调用  
1. 对方法调用的参数和返回值的处理，和上面所描述的普通函数调用完全一致。但是，方法调用和函数调用有一个重要的区别，即:调用上下文。属性访问表达式由两部分组成:一个对象和属性名称  
2. 大多数方法调用使用点符号来访问属性，使用方括号(的属性访问表达式)也可以进行属性访问操作。  
3. 方法和this关键字是面向对象编程范例的核心。任何函数只要作为方法调用实际上都会传入一个隐式的实参这个实参是一个对象，方法调用的母体就是这个对象。通常来讲，基于那个对象的方法可以执行多种操作，方法调用的语法已经很清晰地表明了函数将基于一个对象进行操作  
4. js语法不允许给this赋值  
5. 和变量不同，关键字this没有作用域的限制，嵌套的函数不会从调用它的函数中继承this。如果嵌套函数作为方法调用，其this的值指向调用它的对象。如果嵌套函数作为函数调用，其this值不是全局对象(非严格模式下)就是undefined (严格模式下)。如果你想访问这个外部函数的this值，需要将this的值保存在一个变量里，这个变量和内部函数都同在一个作用域内。  
##### 构造函数调用  
1. var o = new Object();  
构造函数调用创建一个新的空对象， 这个对象继承自构造函数的prototype属性。构造函数试图初始化这个新创建的对象，并将这个对象用做其调用上下文，因此构造函数可以使用this关键字来引用这个新创建的对象。注意，尽管构造函数看起来像一个方法调用，它依然会使用这个新对象作为调用上文。也就是说，在表达式new o.m()中，调用上下文并不是o。  
2. 构造函数通常不使用return关键字，它们通常初始化新对象，当构造函数的函数体执行完毕时，它会显式返回。在这种情况下，构造函数调用表达式的计算结果就是这个新对象的值。然而如果构造函数显式地使用return语句返回一个对象，那么调用表达式的值就是这个对象。如果构造函数使用return语句但没有指定返回值，或者返回一个原始值,那么这时将忽略返回值，同时使用这个新对象作为调用结果。  
##### 间接调用  
JavaScript中的函数也是对象，和其他JavaScript对象没什么两样，函数对象也可以包含方法。其中的两个方法ca11()和apply()可以用来间接地调用函数。两个方法都允许显式指定调用所需的this值，也就是说，任何函数可以作为任何对象的方法来调用，哪怕这个函数不是那个对象的方法。两个方法都可以指定调用的实参。ca11()方法使用它自有的实参列表作为函数的实参, apply()方 法则要求以数组的形式传入参数。  
#### 函数的形参和实参  
1. 省略的实参将是undefined，多出的参数会自动忽略  
2. JavaScript方法的形参并未声明类型，在形参传入函数体之前也未做任何类型检查。可以采用语义化的单词来给函数实参命名，或者像刚才的示例代码中的arraycopy()方法一样给实参补充注释，以此使代码自文档化，对于可选的实参来说，可以在注释中补充一下“这个实参是可选的”。当一个方法可以接收任意数量的实参时，可以使用省略号  
#### 作为值的函数  
1. 函数可以定义，也可以调用，这是函数最重要的特性。函数定义和调用是JavaScript的词法特性，对于其他大多数编程语言来说亦是如此。然而在JavaScript中， 函数不仅是一种语法，也是值，也就是说，可以将函数赋值给变量,存储在对象的属性或数组的元素中，作为参数传入另外一个函数等。  
2. function square（x）{return x*/x；}  
这个定义创建一个新的函数对象，并将其赋值给变量square。函数的名字实际上是看不见的，它(square) 仅仅是变量的名字，这个变量指代函数对象。函数还可以赋值给其他的变量，并且仍可以正常工作:   
var S = square;   //现在s和square指代同一个函数  
square(4);        // => 16  
s(4);             // => 16   
3. 除了可以将函数赋值给变量，同样可以将函数赋值给对象的属性。当函数作为对象的属性调用时，函数就称为方法:  
var o = {square: function(x) { return x*/x; }}; //对象直接量   
var y = o.square(16);  //y等于256  
#### 闭包  
1. 函数对象可以通过作用域链相互关联起来，函数体内部的变量都可以保存在函数作用域内，这种特性在称为“闭包"  
2. 闭包可以捕捉到局部变量(和参数)，并一直保存下来，看起来像这些变量绑定到了在其中定义它们的外部函数。  
#### 函数式编程  
##### 使用函数处理数组  
可以使用数组方法map()和reduce()来实现同样的计算，这种实现极其简洁：  
//首先定义两个简单的函数  
var sum = function(x,y) { return x+y; };  
var square = function(x) { return x*/x; };  
//然后将这些函数和数组方法配合使用计算出平均数和标准差  
var data = [1,1,3,5,5];  
var mean = data. reduce(sum)/data .1ength;  
var deviations = data . map(function(x) {return x-mean;});  
var stddev = Math.sqrt(deviations.ap(square).reduce(sum)/(data.1ength-1));  
(高阶函数)  
1. 所谓高阶函数，就是操作函数的函数，它接收一个或多个函数作为参数，并返回一个新函数

#### call/apply/bind方法  
（ toString 方法：返回一个表示当前函数源代码的字符串。valueOf方法：返回函数本身）  
（this关键字：在function内部被创建；指向调用时所在函数所绑定的对象；this 不能被赋值，this 的值取决于函数被调用的方式） 
1. call方法  
 语法： fn.call(thisObj，arg1，arg2，...)  
 参数：arg1,arg2,...：被调用函数的实参（是一个参数序列）  
      thisObj：将函数对象中的 this 指向 thisObj 对象  
 说明：1. 如果 thisObj 未传递，this 指向全局对象 window  
      2. 如果传递为 undefined/null，this 指向全局对象 window  
      3. 如果传递为数字，字符串，布尔值，this 指向该原始值的包装对象  
 返回值：与 fn 普通调用相同  
 作用：调用函数，并改变函数执行的 this 指向  
2. apply（）方法  
语法： fn.apply(thisObj，[arg1，arg2，...])（是一个参数数组）  
其他用法均与call（）方法一样  
【call()、apply()使用仍然是执行原来对象的方法里面的代码，只是代码中的this指向改变了。如果调用的对象方法里面没有this，那么使用call()和apply()没有任何改变，也没有意义  
        var x = 100;  
        var obj = {  
            x: 50  
        };  
        var foo = {  
            x: 0,  
            getX: function () {  
                return this.x;  
            }  
        };  
        console.log(foo.getX()); //0  
        console.log(foo.getX.call(obj)); //50  
        console.log(foo.getX.apply(obj)); //50  
        //call()、apply()没有指定对象时 默认指向全局对象（window）  
        console.log(foo.getX.call()); //100  
        console.log(foo.getX.apply()); //100  】  
3.  bind () 方法  
语法： fn.bind(thisObj，arg1，arg2,...)    
参数： 当绑定函数调用时，thisObj 参数作为原函数运行时的 this 指向。  
        arg1,arg2,...  当绑定函数被调用时，这些参数加上绑定函数本身的参数会按照顺序作为 原函数运行时的参数。（预设参数）  
返回值：返回一个原函数的拷贝（绑定函数），并拥有指定的 this值和初始参数  
 bind 不会调用函数，即不会执行原函数中的代码  
4. 总结：  
 apply，call，bind 三个方法第一个参数都是改变函数在调用时 this 指向的对象  
 apply，call，bind  第一个参数为空，null，undefined，this 指向的是 window  
 apply，call 两个方法只是参数形式有所不同，apply 参数是一个数组，call 参数则是列表序列  
 apply，call 都会立即调用函数执行，bind 不会立即调用函数

3. 通过 Function 构造函数创建函数  
  可以传入任意数量的实参  
  最后一个实参为函数体  
  函数体中 javascript 语句之间分号隔开  
  Function 构造函数创建一个匿名函数  
如：var max = new function("a","b","return a>b?a:b;");  
Function构造器执行传给它的JavaScript代码字符串。var add=new Function('x','y','return x+y')  
Function( )构造函数允许JavaScript在运行时动态地创建并编译函数。每次调用Function()构造函数都会解析函数体，并创建新的函数对象。如果是在一个循环或者多次调用的函数中执行这个构造函数，执行效率会受影响。相比之下，循环中的嵌套函数和函数定义表达式则不会每次执行时都重新编译。最后一点，也是关于Function()构造函数非常重要的一点，就是它所创建的函数并不是使用词法作用域，相反，函数体代码的编译总是会在顶层函数

### 函数  
1. 实参>形参----额外的参数会被忽略（arguments除外），实参<形参，丢失的参数是undefined  
2. 闭包：函数以及它所连接的周围作用域中的变量即为闭包。  
3. JavaScript中函数的3种形式：  
①非方法的函数  
②构造器 通过new操作符来调用一个函数   
③方法 将一个函数存储为一个对象的属性。 
4. “形参”和“实参” 形参被用在定义函数时，实参在函数调用时被使用    
#### 函数定义形式  
1. 函数是什么？函数是可以通过外部代码调用的一个“子程序”。一个函数由称为函数体的一系列语句组成。值可以传递给一个函数，函数将返回一个值。  
2. 函数定义方式  
 （1）通过函数声明的形式来定义  
      函数声明定义了一个新的变量，创建了一个函数对象，并将对象赋值给这个新的变量。  
 （2）通过函数表达式的形式来定义  
      函数表达式  
      函数表达式的值可以赋给一个变量，可以作为传入别的函数的参数等。  
      普通的函数表达式没有名字，称为匿名函数表达式。  
      具名函数表达式：具名函数表达式的名字只能在函数表达式内部被访问。 
 （3）通过 Function 构造函数实例化的形式来定义  
3. 通过 Function 构造函数创建函数  
  可以传入任意数量的实参  
  最后一个实参为函数体  
  函数体中 javascript 语句之间分号隔开  
  Function 构造函数创建一个匿名函数  
如：var max = new function("a","b","return a>b?a:b;");  
Function构造器执行传给它的JavaScript代码字符串。var add=new Function('x','y','return x+y')  
Function( )构造函数允许JavaScript在运行时动态地创建并编译函数。每次调用Function()构造函数都会解析函数体，并创建新的函数对象。如果是在一个循环或者多次调用的函数中执行这个构造函数，执行效率会受影响。相比之下，循环中的嵌套函数和函数定义表达式则不会每次执行时都重新编译。最后一点，也是关于Function()构造函数非常重要的一点，就是它所创建的函数并不是使用词法作用域，相反，函数体代码的编译总是会在顶层函数  
4. 函数定义三要素：函数名、函数的参数、函数的返回值 （但都不是必须有）  
5. ①匿名函数（如函数表达式，即没有函数名的函数）  
 单独的匿名函数是无法运行的  
 可以把匿名函数赋值给变量或立即执行  
   ②具名函数优势  
 当遇到错误时，堆栈跟踪会显示函数名，容易寻找错误






《深入理解JavaScript》  
第15章  
一、JavaScript中函数的3种形式  
1.非方法的函数  
2.构造器 通过new操作符来调用一个函数  
3.方法 将一个函数存储为一个对象的属性。  
二、术语：“形参”和“实参”  
形参被用在定义函数时，实参在函数调用时被使用  
三、定义函数  
1.函数表达式  
函数表达式的值可以赋给一个变量，可以作为传入别的函数的参数等。  
普通的函数表达式没有名字，称为匿名函数表达式。  
具名函数表达式  
具名函数表达式的名字只能在函数表达式内部被访问。 
2.函数声明  
函数声明定义了一个新的变量，创建了一个函数对象，并将对象赋值给这个新的变量。  
3.Function构造器  
执行传给它的JavaScript代码字符串。var add=new Function('x','y','return x+y')  
4.函数提升  
将函数的声明放到作用域的开始  
①函数声明是完全提升的，所以在函数声明前可以进行函数调用。  
②使用var的定义也会进行代码提升，但只对于声明有效，对于赋值过程是无效的。  
5.函数的名称  
函数的声明会创建非标准的name属性，匿名函数表达式的name是一个空字符串，具名函数表达式也有一个name。  
6.哪个更好，函数声明还是函数表达式  
函数声明的优势  
①函数声明会做代码提升，因此可以在源码中先于函数的定义来调用函数  
②它们具有名字，不过，JavaScript引擎也在对匿名函数表达式的名字引用做优化。  
7.控制函数调用：call(),apply()和bind()  
①func.apply(thisValue,argArray)  
此方法在调用函数func时，argArray参数将作为函数的arguments传递给函数，而thisValue这个参数则可以指定执行func时的this值。  
apply()用在一个函数需要以类似数组的形式接受多个参数。  
②func.bind(thisValue,arg1,...,argN)  
这个方法会执行部分的函数功能，它会创建-一个新的函数,这个函数会调用func,
并会将thisValue指定为this,同时应用以下参数: arg1 直到argN,紧随其
后的是新函数的实际参数。  
8.参数缺失或者超出时的处理  
实参数量多于形参：多余的参数会被忽略，但是能在类数组的arguments中被获取到。  
实参数量小于形参：缺失的形参都会被赋予undefined值。  
①通过索引访问所有参数：神奇的arguments变量  
arguments变量：只存在于函数中，是一个类数组对象，包含了当前函数调用的所有实参。  
特征：它是类数组的，但又非数组。一方面，它有一个length属性，所有的参数都可以通过索引值来进行读写。 
另一方面，arguments不是一个数组，仅仅是类似，并没有数组的方法。  
它是一个对象，因此它支持所有的对象方法和操作。  
arguments的废弃特性  
arguments. callee指向了当前调用的函数。它一般用于匿名函数的自递归
调用，但是它在严格模式中是禁用的。  
在非严格模式中，当改变一个参数，arguments会实时地变化，但是在严格模式中，并不支持这一特性。  
严格模式禁用了对变量arguments的分配。  
②强制性参数，限制参数数量的最小值  
判断一个参数是否缺失：第一种，检测它的值是否为undefined。第二种，将参数转化为布尔值。undefined会被认为false。第三种，用arguments.length来检测并强制指定参数数量的最小值。  
最后一种方式相比前两种有一些区别:  
前两种方式无法区分foo ()和foo (undefined)。它们对于两种情况会抛一
样的错误。  
第三种方式会对foo()抛错,而对于foo (undefined)会正常使用undefined
传人函数并调用。  
③可选参数  
四种处理可选参数的选择：第一种，检测undefined。第二种，将可选参数转换为布尔值。第三种，使用或运算符，如果左侧操作数不是false值，则返回左侧的操作数，否则将返回右侧的操作数。第四种，使用arguments.length来检测函数支持的最小数量的参数。  
同样的，最后一种方式有别于其他的方式:  
前三种方式无法区分bar (1,2)和bar (1, 2, undefined)。这两种情况下，
opt ional的值都是默认值。  
第四种方式对于bar (1,2)会使用默认值，而对于bar (1, 2, undefined)
会保留undefined的传人。  
④模拟参数的引用传递  
在JavaScript中，不能传递参数的引用，当将一个变量传递给一个函数，它的值会被复制一份并传递给函数。  
⑤陷阱：非预期的可选参数  
将一个函数c作为另一个函数f的参数传入，两种情况：  
函数f签名声明需要传人的参数。f可能会提供多个参数,而c可以决定使用
这些参数中的哪几个。  
C的实际签名，它有可能支持可选参数。  
当不明确函数或者方法的调用方式时，要格外明确函数接受哪些参数，同时传入哪些参数。  
9.具名参数  
调用函数或者方式时，将实参和形参做映射，有两种方式：  
通过位置来映射的位置型参数。第一个实参对应第一一个形参， 第二个实参对应
第二个形参，以此类推。  
具名参数则通过名称(标识)来做变量的映射。在一个函数的定义中名称会与
形参做关联，在函数调用中，名称则与实参做关联。只要参数的名称正确，你不需
要关心参数名的顺序。  
具名参数有两个优点:它们对函数的参数进行了描述，同时它们对于处理可选参数
的场景也很有用。  
①具名参数可作为描述信息  
一个函数selectEntries()，它会从数据中返回一个入口。  
②可选的具名函数  
对于可选的位置型参数，只有当它们被放置在参数的最后时才可能正确地工作，否则，就要通过对中间的参数传入例如null的值来保持每个参数所在位置的正确性。  
③在JavaScript中模拟具名参数  
通过对象字面量来命名参数，并将对象作为一个实参传入函数。  
也可以将位置型参数和具名参数相结合。  


第16章
### 作用域、环境和闭包  
1.定义变量  
在JavaScript中，在使用变量前，你可以通过var语句来定义变量:  
var foo;  
foo = 3; // OK, has been declared  
bar = 5; // not 0K, an undeclared variable  
你也可以将赋值语句与变量定义语句合并进行变量的初始化:  
var foo = 3;  
一个未初始化的变量的值是undefined  
2. 静态性  
可以无须执行程序而只从程序源码的角度来看程序的工作。下面的代码，函数g被函数f包围在内部:
function f() {  
   function g() {  
   }  
 }  
描述性的词法就像是静态声明，因为它们都涉及了程序的词法(单词、源码)。  
3. 动态性  
它表示一个程序在运行期所表现出来的特性。  
function g() {  
}  
function f() {  
   g();  
}  
当我们调用f()，它会调用g()。在执行期间，g被f调用代表了一种动态的关系。  
4. 作用域  
(1)变量的作用域：  
变量的作用域是指变量在何处可以被访问到。例如:  
function foo() {  
var x;  
}  
这里，x的直接作用域是函数foo()。  
(2)词法作用域  
JavaScript中的变量都是有词法作用域的，因此一个程序的静态结构决定了一个变量的作用域(这个作用域并不会被函数从哪里调用等影响)。  
(3)嵌套作用域  
如果在一个变量的直接作用域中嵌套有多个作用域，那么这个变量在所有的这些作用域中都可以被访问:  
function foo(arg) {  
   function bar() {  
      console. log('arg:' +arg);  
   }  
   bar();  
}  
console. log(foo( 'hello')); // arg: hello  
arg的直接作用域是foo () ,但是它同样可以在嵌套的作用域bar ()中被访问。我们说嵌套，foo ()是外部的作用域，而bar ()是内部作用域。  
(4)覆盖  
如果在一个作用域中声明了一个与外层作用域同名的变量，那么在这个内部作用域以及其内部的所有作用域中将会访问不到外面的变量。而内部的变量的变化并不影响外部的变量，当离开内部作用域，外部变量又可以被访问了。  
var x = "global";  
   function f() {   
   var x = "local";  
   console.log(x); // local  
   }  
f();  
console.log(x); // global  
在函数f()中，全局的x被本地x所覆盖。  
5. 变量以函数为作用域  
JavaScript 的变量是函数级作用域的:只有函数可以产生新的作用域;  
代码块在作用域中是不起作用的。例如:  
function main() {  
   { // block starts  
      var foo = 4;  
   } // block ends  
   console. log(foo); // 4  
}  
换句话说，foo 在main()中都是可以被访问到的，而不仅仅是在块中。  
6. 变量声明的提前  
JavaScript会提前所有的变量声明，它会把所有的声明移到直接作用域的最前面。   
function f() {  
   console. log(bar); // undefined  
   varbar='abc';  
   console. log(bar); // abc  
}  
我们可以看到变量bar在函数f()的第一行已经存在了，只是还没有值;因此，被提前的是变量的声明，而非变量的复制。实际上，JavaScript 中是这样执行f()的:  
function f() {  
   var bar;  
   console. log(bar); // undefined  
   bar = ' abc';  
   console. log(bar); // abc  
}  
如果你定义一个已经被定义过的变量，那么什么也不会发生(包括变量的值，也不会变化):  
>var x=123;  
>var x;  
>X  
123  
函数的声明也会被提前，但是与变量截然不同，函数声明会被整体提前，而不仅仅是变量的创建的那部分  
7. 通过IIFE引入新的作用域  
关于IIFE,我们有一些要注意的:   
(1)它是立即执行的  
函数的结束大括号后面的括号是用来立即调用函数的。函数体会立即执行。  
(2)它必须是一个表达式  
如果一个语句以function关键词开头，解析器会认为它是一个函数定义。但是一个函数声明并不会立即执行。因此，我们在语句前加了一个左括号告诉解析器function关键词是处于一个函数表达式的开
头。在括号中，只存在表达式。  
(3)别忘了后面的分号  
7.1  
可以通过前缀运算符来强制执行一个表达式。例如，可以用逻辑非:  
!function () { // open IIFE  
   // inside IIFE  
}(); // close IIFE  
或者是void运算符  
void function () { // open IIFE  
   // inside IIFE  
}(); // close IIFE  
使用前缀运算符的好处是忘了分号结尾并不会造成任何问题。  
7.2 预内置表达式上下文  
为IIFE强制执行表达式上下文并不是必需的，如果已经在一个表达式的上下文里面，那么不必使用括号或者前缀操作符。  
7.3 传参的IIFE  
可以使用参数的方式在IIFE的内部定义变量:  
varx=23;  
(function (twice) {  
  console. log(twice);   
}(x * 2));  
这就类似于:  
varx=23;  
(function () {  
   vartwice=x\*2;  
   console. log( twice);  
}());  
7.4 IIFE的应用  
IIFE使得可以获取函数中的私有数据。不必定义全局变量也可以严密地将函数本身的逻辑包装在一起。这样就可以避免对全局命名空间的污染:  
var setValue = function (){  
   var prevValue;  
   return function (value) { // define setValue  
   if (value !== prevValue) {  
      console . log( 'Changed: ' + value);  
      prevValue = value ;  
   }  
   };  
}();    
8. 全局变量  
①包含整个程序的作用域叫做全局作用域或是程序作用域。在全局作用域中，可定义函数来创建嵌套的作用域。每一个作用域都可以访问它内部以及其父作用域中的变量。由于全局作用域包含了所有的作用域，它里面的变量便可以在任何地方被访问到  
②全局作用域有两大劣势。首先，程序中依赖全局作用域的代码片段会产生一些边缘效应，程序可能不够健壮，会产生一些不可预期的效果，重用性更低。其次,一个Web页面上面的所有JavaScript都共享一个相同的全局作用域以及其全局变量:代码、内置的插件、分析代码、社交媒体按钮等。这意味着可能会产生名字的冲突的问题。这也是为什么要将变量隐藏于全局作用域之外的原因。  
9. 全局对象  
JavaScript有一些不常用的特性可以通过一个对象来为全局的变量创建环境，这个对象就叫做全局对象，全局对象可以用来创建、读取或是修改全局变量，在全局作用域中，this指向全局对象。  
注：全局对象有原型，如果要罗列它所有的属性，可以使用类似getAllPropertyNames（）的函数。  
①浏览器和Node.js全局变量引用全局对象的不同：  
浏览器中的全局对象是window,它是文档对象模型(DOM)的一部分，而非ECMAScript5的一部分。在每-一个帧或者window中，都有一一个全局对象。  
Node.js中的全局对象是global,它是-一个Node.js专属的变量。每一个模块都有它自己的作用域,在这些作用域中this指向了这个作用域的对象。因此，this和global在模块中是不同的。  
②window的使用场景  
场景一：创建全局变量  
代码前面的window前缀直观的表示了代码指向了一个全局变量而非一个本地变量 var foo=123;  
这样使得程序变得脆弱，如果将foo从全局作用域移到另一个作用域中，可能会使得程序停止工作   
(function (){  
    var foo=123;  
    console.log(window.foo);  
    }());  
因此，最好将foo用一个变量来进行引用，而不是作为window的属性，加上一个例如g_的前缀。  
场景二：内置插件  
场景三：风格检查器  
JSLint,JSHint，使用window意味着,如果在当前文件中引用了一个并不定义在该文件中的全局变量,将不会得到错误提示。然而,这两个工具都会提供方式告诉它们这样的变量并避免这样的错误。  
场景四：检测一个全局变量是否存在  
if(window.someVariable){....}  
这是一种安全的检测方式,而下面的语句会在someVariable未被定义时抛出异常:  
// Don't do this  
if (someVariable) { ... }  
另外还有两种通过window来检查的方式:它们大致相同，但是更为明确:  
if (window. someVariable !== undefined) { ... }  
if ('someVariable' in window) { ... }  
检查一个变量是否存在(并是否有值)的常用方法是通过typeof   
if (typeof someVariable !== ' undefined') { ... }  
场景五：在全局作用域中创建内容  
借助window向全局作用域添加新的内容，  
if(!window.someApiFunction){
    window.someApiFunction=...;
}   
当处在全局作用域，通常将变量添加到全局作用域的最好方式是使用var，相比之下，使用window结合响应的条件判断更为清晰。  
10.环境：变量的管理  
变量有两种传递的方式，如果有必要，有两种维度。  
(1)动态维度:调用函数  
每当一个函数被调用，它就需要给它的参数和变量准备新的存储空间。当调用结束之后，空间通常会被释放。  
function fac(n) {  
if (n<= 1) {  
return 1;  
return n * fac(n - 1);  
(2)词法维度:与外部作用域进行关联  
无论一个函数被调用了多少次，它总要访问它自己(最新)的本地变量和外部作用域的变量。例如下面的doNTimes 函数，它内部有一个辅助函数doNTimesRec,当doNTimesRec多次调用自己的时候,每一次调用都会创建一个新的环境。然而，doNTimesRec 在这多次调用中却一直与doNTimes的环境保持着联系(类似于所有的函数都共享了同一个全局环境)。在第一行中，doNTimesRec就需要通过这个联系来访问action。  
function doNTimes(n, action) {  
function doNTinesRec(x) {  
if(x>=1){  
action(); // (1)  
doNTinmesRec(x-1);  
}  
}  
doNTinesRec(n);  
}  
总结：  
(1)动态维度:执行上下文的栈
函数每调用一次，就会创建-一个新的环境将(变量和参数的)标识符和变量做映射。对于递归的情况，执行上下文，即环境的引用是在栈中进行管理的。这里的栈对应了调用栈。  
(2)词法维度:环境链  
为了支持这一维度， JavaScript 会通过内部属性[ [Scope]]来记录函数的作用域。在函数调用时，JavaScript 会为这个函数所在的新作用域创建一个环境。这个环境有一个外层域(outer) ,它通过[ [Scope]]创建并指向了外部作用域的环境。因此，在JavaScript中一直存在一个环境链，它以当前环境为起点, 连接了一层外部的环境。每一个环境链最终会在全局环境(它是所有函数初始化调用的作用域）终结。而全局环境的外部环境指向了null。  
例：  
function myFunction(myParan) {  
var myVar = 123;  
return myFloat;  
var myFloat = 1.3;  
// Step 1  
myFunction( 'abc'); // Step 2  
执行过程：  
(1)myFunction和myFloat被存在全局环境中(#0)。要注意的是myFunction所引用的函数对象通过内部属性[[Scope]]指向了它自己的作用域(全局作用域)。  
(2)而对于执行期的myFunction('abc'), JavaScript 会创建一个新的环境(#1)用来管理参数和本地变量。函数通过(从myFunction. [ [Scope] ]初始化出来的)外层链来引用外部的环境。由于外层环境链，使得myFunction可以访问到
myFloat。  
11.闭包：使得函数可以维持其创建时所在的作用域  
闭包是一个函数外加上该函数创建时所建立的作用域。  
①通过环境来控制闭包  
function createInc( startValue) {  
return function (step) {  
startValue += step;  
return startVa lue;  
};  
}  
将createInc()函数，拆解为4步：  
(1)这一步在交互之前，在createInc定义之后。createInc的入口被添加到全局的环境中(#0)并指向一个函数对象。  
(2)这一步发生在函数调用createInc的执行期间。JavaScript为createInc创建了一个新的环境，并将这个环境推到栈中。它的外层环境是全局环境(即createInc. [[Scope]] )。环境中存在startValue这个变量。  
(3)这一步发生在给inc赋值时。当createInc调用结束，它所指向其环境的执行上下文就从栈中被移除了,但是其环境还存在于堆当中,因为inc. [[Scope]]还引用着。inc 是一个闭包(函数加上其创建时的环境)。  
(4)这一步在inc(1)的执行期间。一个新的环境(#1)被创建并且一个指向它的执行上下文被推入栈中。它的外层环境是inc的[[Scope]].外部环境使得inc可以访问到startValue.  
②陷阱：不经意间的环境共用  
有时候创建的函数行为可能会受当前作用域中变量的影响，通常来说每个函数应该配合函数创建时的变量值，然而，由于函数变成了闭包，函数总是会使用当前的变量值，在for循环中，这可能会使函数的工作不符合预期。  
解决方法：  
（1）为每个函数在返回的数组中创建一个新的环境。  
（2）在这个创建的新环境中存储当前i的值。  


《你不知道的JavaScript》上卷  
第一章  
#### 编译原理  
源代码在执行之前的三个步骤：  
1.分词/词法分析：会将由字符组成的字符串分解成有意义的代码块，这些代 码块被称为词法单元。  
2.解析/语法分析：将词法单元流（数组）转换成一个由元素逐级嵌套所组成的代表了程序语法 结构的树。  
3.代码生成：将 AST 转换为可执行代码的过程称被称为代码生成。  
#### 理解作用域  
var a = 2;   
引擎： 从头到尾负责整个 JavaScript 程序的编译及执行过程。  
编译器：引擎的好朋友之一，负责语法分析及代码生成等脏活累活。  
作用域：引擎的另一位好朋友，负责收集并维护由所有声明的标识符（变量）组成的一系列查 询，并实施一套非常严格的规则，确定当前执行的代码对这些标识符的访问权限。  
对于var a=2;编译器进行如下处理：  
1. 遇到 var a，编译器会询问作用域是否已经有一个该名称的变量存在于同一个作用域的 集合中。如果是，编译器会忽略该声明，继续进行编译；否则它会要求作用域在当前作 用域的集合中声明一个新的变量，并命名为 a。  
2. 接下来编译器会为引擎生成运行时所需的代码，这些代码被用来处理 a = 2 这个赋值 操作。引擎运行时会首先询问作用域，在当前的作用域集合中是否存在一个叫作 a 的 变量。如果是，引擎就会使用这个变量；如果否，引擎会继续查找该变量。  
LHS,RHS  
当变量出现在赋值操作的左侧时进行 LHS 查询，出现在右侧时进行 RHS 查询。  
LHS 和 RHS 的含义：“赋值操作的左侧或右侧”并不一定意味着就是“= 赋值操作符的左侧或右侧”。赋值操作还有其他几种形式，因此在概念上最 好将其理解为“赋值操作的目标是谁（LHS）”以及“谁是赋值操作的源头 （RHS）”。  
#### 作用域嵌套  
当一个块或函数嵌套在另一个块或函数中时，就发生了作用域的嵌套。  
在当前作用 域中无法找到某个变量时，引擎就会在外层嵌套的作用域中继续查找，直到找到该变量， 或抵达最外层的作用域（也就是全局作用域）为止。  
例：  
function foo(a) {     
console.log( a + b );   
}   
var b = 2;   
foo( 2 ); // 4  
对b进行的 RHS 引用无法在函数 foo 内部完成，但可以在上一级作用域中完成。  
遍历嵌套作用域链的规则：引擎从当前的执行作用域开始查找变量，如果找不到，就向上一级继续查找。当抵达最外层的全局作用域时，无论找到还是没找到，查找过程都会停止。  
#### 异常  
function foo(a) {     
console.log( a + b );    
b = a;   
}   
foo( 2 );  
第一次对 b 进行 RHS 查询时是无法找到该变量。 
如果 RHS 查询在所有嵌套的作用域中遍寻不到所需的变量，引擎就会抛出 ReferenceError 异常。  
严格模式：在 严格模式中 LHS 查询失败时，并不会创建并返回一个全局变量，引擎会抛出同 RHS 查询 失败时类似的 ReferenceError 异常。  
注：不成功的 RHS 引用会导致抛出 ReferenceError 异常。不成功的 LHS 引用会导致自动隐式 地创建一个全局变量（非严格模式下），该变量使用 LHS 引用的目标作为标识符，或者抛 出 ReferenceError 异常（严格模式下）。  

第二章 
#### 词法作用域  
1.词法阶段  
function foo(a) {     
var b = a * 2; 
    function bar(c) {       
    console.log( a, b, c );    
    } 
    bar( b * 3 );   
    }     
foo( 2 ); // 2, 4, 12  
三个逐级嵌套的作用域：  
①包含着整个全局作用域，其中只有一个标识符：foo。
②包含着 foo 所创建的作用域，其中有三个标识符：a、bar 和 b。
③包含着 bar 所创建的作用域，其中只有一个标识符：c。
作用域查找会在找到第一个匹配的标识符时停止。在多层的嵌套作用域中可以定义同名的 标识符，这叫作“遮蔽效应”。  
全局变量会自动成为全局对象（比如浏览器中的 window 对象）的属性，因此 可以不直接通过全局对象的词法名称，而是间接地通过对全局对象属性的引 用来对其进行访问。  
#### 欺骗词法  
eval（执行动态创建的代码）：可以接受一个字符串为参数，并将其中的内容视为好像在书 写时就存在于程序中这个位置的代码。  
如果 eval(..) 中所执行的代码包含有一个或多个声明（无论是变量还是函 数），就会对 eval(..) 所处的词法作用域进行修改。  
setTimeout(..) 和 setInterval(..) 与eval方法相似，第一个参数可以是字符串，字符串的内容可以被解释为一段动态生成的函数代码。  
new Function(..) ，最后一个参数可以接受代码字符串，并将其转 化为动态生成的函数。  
with：重复引用同一个对象中的多个属性的快捷方式  
with 可以将一个没有或有多个属性的对象处理为一个完全隔离的词法作用域， with 块可以将一个对象处理为词法作用域，但是这个块内部正常的 var 声明并不会被限制在这个块的作用域中，而是被添加到 with 所处的函数作 用域中。  
eval和with:  
eval(..) 函数如果接受了含有一个或多个声明的代码，就会修改其所处的词法作用域  
with 声明实际上是根据传递给它的对象凭空创建了一个全新的词法作用域。  
注：  
①词法作用域意味着作用域是由书写代码时函数声明的位置来决定的。  
②JavaScript 中有两个机制可以“欺骗”词法作用域：eval(..) 和 with。  
第三章  
#### 函数中的作用域  
函数作用域的含义：属于这个函数的全部变量都可以在整个函数的范围内使用及复用  
隐藏内部：  
隐藏：：从所写的代码中挑选出一个任意的片段，然后用函数声明对它进行包装。  
隐藏的好处：可以避免同名标识符之间的冲突  
1.全局命名空间  
变量冲突存在于全局作用域中，当程序中加载了多个第三方库时，如果没有妥善地将内部私有的函数或变量隐藏起来，就会很容易引发冲突。  
这些库在全局作用域中声明一个名字足够独特的变量，通常是一个对象（库的命名空间）  
2.模块管理  
从众多模块管理器中挑选一个来使用  

var a = 2;   
function foo() {  
    var a = 3;    
    console.log( a );   
}   
console.log( a );   
问题：  
①必须声明一个具名函数 foo()， foo 这个名称“污染”了所在作用域。  
②必须显式地通过函数名（foo()）调用这个函数才能运行其 中的代码。  
解决方案：  
var a=2;  
(function foo(){   
    var a = 3;     
    console.log( a );   
})();  
console.log( a );   
①包装函数的声明以 (function... 开始  
②区分函数声明和表达式最简单的方法是看 function 关键字出现在声明中的位置  
注：函数声明和函数表达式之间最重要的区别是它们的名称标识符将会绑定在何处。  
#### 匿名和具名  
匿名函数表达式：  （function().. 没有名称标识符）  
setTimeout( function() {    
console.log("I waited 1 second!");  
}, 1000 );  
缺点：  
1. 匿名函数在栈追踪中不会显示出有意义的函数名，使得调试很困难。  
2. 如果没有函数名，当函数需要引用自身时只能使用已经过期的 arguments.callee 引用，比如在递归中。另一个函数需要引用自身的例子，是在事件触发后事件监听器需要解绑自身。   
3. 匿名函数省略了对于代码可读性 / 可理解性很重要的函数名。一个描述性的名称可以让代码不言自明。  
立即执行函数表达式：  
var a = 2;   
(function foo() {   
    var a = 3;     
    console.log( a );   
})();   
console.log( a );   
通过在末尾加上另外一个 (  ) 可以立即执行这个函数。  
IIFE （立即执行函数表达式 ）  
① var a = 2;    
(function IIFE() {   
    var a = 3;    
    console.log( a );   
})();     
console.log( a );   
②IIFE另一个用法：把它们当作函数调用并传递参数进去。  
var a = 2;   
(function IIFE( global ) {   
    var a = 3;    
    console.log( a );     
    console.log( global.a );   
})( window );   
console.log( a );  
将 window 对象的引用传递进去，但将参数命名为 global。  
③另一个应用场景：解决 undefined 标识符的默认值被错误覆盖导致的异常  
(function IIFE( undefined ) {   
    var a;     
    if (a === undefined) {    
    console.log( "Undefined is safe here!" );   
    }   
})();  
④倒置代码的运行顺序  
(function IIFE( def ) {      
def( window );   
})(function def( global ) {   
    var a = 3;     
    console.log( a );     
    console.log( global.a );   
});  
#### 块作用域  
（一）with  
with 关键字，它不仅是一个难于理解的结构，同时也是块作用域的一 个例子（块作用域的一种形式），用 with 从对象中创建出的作用域仅在 with 声明中而非外部作用域中有效。  
（二）try/catch   
 try/catch 的 catch 分句会创建一个块作 用域，其中声明的变量仅在 catch 内部有效。  
（三）let  
1. let 关键字可以将变量绑定到所在的任意作用域中（通常是 { .. } 内部）。换句话说，let 为其声明的变量隐式地了所在的块作用域。  
var foo = true;   
if (foo) {     
   let bar = foo * 2;     
   bar = something( bar );      
   console.log( bar );  
 }   
console.log( bar ); // ReferenceError  
2. 用 let 将变量附加在一个已经存在的块作用域上的行为是隐式的。只要声明是有效的，在声明中的任意位置都可以使用 { .. } 括号来为 let 创建一个用于绑 定的块。 
3. 使用 let 进行的声明不会在块作用域中进行提升。声明的代码被运行之前，声明并不 “存在”。
{     
   console.log( bar ); // ReferenceError!     
   let bar = 2;  
}  
4. let循环  
for 循环头部的 let 不仅将 i 绑定到了 for 循环的块中，事实上它将其重新绑定到了循环 的每一个迭代中，确保使用上一个循环迭代结束时的值重新进行赋值。  
由于 let 声明附属于一个新的作用域而不是当前的函数作用域（也不属于全局作用域）， 当代码中存在对于函数作用域中 var 声明的隐式依赖时，就会有很多隐藏的陷阱，如果用 let 来替代 var 则需要在代码重构的过程中付出额外的精力。  
（四）const  
 const，同样可以用来创建块作用域变量，但其值是固定的 （常量）  
 第四章  
 (一)  
①JavaScript会提前所有的变量声明，它会把所有的声明移到直接作用域的最前面。  
function f() {  
console. log(bar); // undefined  
var bar='abc';  
console. log(bar); // abc .  
我们可以看到变量bar在函数f()的第- -行已经存在了，只是还没有值;因此，被提前的是变量的声明，而非变量的复制。实际上,JavaScript中是这样执行f()的:  
function f() {  
var bar;    
console. log(bar); // undefined  
bar = ' abc';  
console. log(bar); // abc  
②如果你定义-一个已经被定义过的变量,那么什么也不会发生(包括变量的值，也不会变化):  
var x=123;  
var X;  
X  
123  
③函数的声明也会被提前，但是与变量截然不同，函数声明会被整体提前，而不仅仅是变量的创建的那部分  
④函数声明会被提升，但是函数表达式却不会被提升。
foo(); // 不是 ReferenceError, 而是 TypeError!  
var foo = function bar() {     // ... };  
⑤使用：  
foo(); // TypeError   
bar(); // ReferenceError  
var foo = function bar() {     // ... };  
这个代码片段经过提升后，实际上会被理解为以下形式：  
var foo;   
foo(); // TypeError  
bar(); // ReferenceError  
foo = function() {     
   var bar = ...self...     
   // ...   
}  
 （二）  
函数优先  
函数声明和变量声明都会被提升。但是一个值得注意的细节（这个细节可以出现在有多个 “重复”声明的代码中）是函数会首先被提升，然后才是变量。  
考虑以下代码：  
foo(); // 1   
var foo;   
function foo() {     
   console.log( 1 );  
}   
foo = function() {  
   console.log( 2 );  
};  
会输出 1 而不是 2 ！这个代码片段会被引擎理解为如下形式：  
function foo() {    
   console.log( 1 );  
}   
foo(); // 1  
foo = function() {    
   console.log( 2 );  
};  
注意，var foo 尽管出现在 function foo()... 的声明之前，但它是重复的声明（因此被忽略了），因为函数声明会被提升到普通变量之前。  
尽管重复的 var 声明会被忽略掉，但出现在后面的函数声明还是可以覆盖前面的。
foo(); // 3   
function foo() {     
   console.log( 1 );  
}   
var foo = function() {     
   console.log( 2 );  
};   
function foo() {     
   console.log( 3 );  
}  

第五章  
function foo() {     
   var a = 2;   
   function bar() {        
      console.log( a );  
   }   
   return bar;   //们将 bar() 函数本身当作 一个值类型进行传递  
}  
var baz = foo();  
baz(); // 2 —— 这就是闭包的效果  
在 foo() 执行后，其返回值（也就是内部的 bar() 函数）赋值给变量 baz 并调用 baz()，实 际上只是通过不同的标识符引用调用了内部的函数 bar()。  
bar() 显然可以被正常执行。但是在这个例子中，它在自己定义的词法作用域以外的地方执行。  
在 foo() 执行后，通常会期待 foo() 的整个内部作用域都被销毁，但是闭包会阻止这件事的发生，事实上内部作用域依然被bar()本身使用，依然存在，因此没有被回收。由于bar()声明的位置，它拥有涵盖 foo() 内部作用域的闭包，使得该作用域能够一 直存活，以供 bar() 在之后任何时间进行引用。bar() 依然持有对该作用域的引用，而这个引用就叫作闭包。  
无论使用何种方式对函数类型的值进行传递，当函数在别处被调用时都可以观察到闭包：  
function foo() {     
   var a = 2;   
   function baz() {     
      console.log( a ); // 2   
   }   
   bar( baz );  
}   
function bar(fn) {     
   fn(); // 这就是闭包！  
}  
把内部函数 baz 传递给 bar，当调用这个内部函数时（现在叫作 fn），它涵盖的 foo() 内部 作用域的闭包就可以观察到了，因为它能够访问 a。  
传递函数当然也可以是间接的：  
var fn; 
function foo() {  
   var a = 2;   
   function baz() {        
      console.log( a );   
   }   
   fn = baz; // 将 baz 分配给全局变量 
}   
function bar() {     
   fn(); // 这就是闭包！  
}   
foo();   
bar(); // 2  
无论通过何种手段将内部函数传递到所在的词法作用域以外，它都会持有对原始定义作用 域的引用，无论在何处执行这个函数都会使用闭包。  
循环和闭包：  
预期是分别输出数字 1~5，每秒一次，每次一个。  
for (var i=1; i<=5; i++) {     
   (function() {         
      setTimeout( function timer() {          
         console.log( i );        
      }, i\*1000 );    
   })();  
}  //这样不能满足预期效果，只会输出5次6  
改进：  
for (var i=1; i<=5; i++) {    
   (function(j) {         
      setTimeout( function timer() {           
         console.log( j );       
      }, j\*1000 );    
   })( i );  
}  
模块  
（1）模式需要具备两个基本条件  
①必须有外部的封闭函数，该函数必须至少被调用一次（每次调用都会创建一个新的模块 实例）。  
②封闭函数必须返回至少一个内部函数，这样内部函数才能在私有作用域中形成闭包，并 且可以访问或者修改私有的状态。  
一个具有函数属性的对象本身并不是真正的模块。从方便观察的角度看，一个从函数调用 所返回的，只有数据属性而没有闭包函数的对象并不是真正的模块。  
（3）  
function CoolModule() {    
    var something = "cool";   
    var another = [1, 2, 3];   
    function doSomething() {          
      console.log( something );    
    }   
    function doAnother() {    
      console.log( another.join( " ! " ) );   
    }   
    return {       
      doSomething: doSomething,     
      doAnother: doAnother    
    };  
 }   
var foo = CoolModule();    
foo.doSomething(); //  cool   
foo.doAnother(); // 1 ! 2 ! 3  
这个模式在 JavaScript 中被称为模块。最常见的实现模块模式的方法通常被称为模块暴露， 这里展示的是其变体  
（4）模块也是普通的函数，因此可以接受参数。模块模式另一个简单但强大的变化用法是，命名将要作为公共 API 返回的对象  
（5）模块有两个主要特征： ①为创建内部作用域而调用了一个包装函数；②包装函数的返回值必须至少包括一个对内部函数的引用，这样就会创建涵盖整个包装函数内部作用域的闭包。  













 
























   





















