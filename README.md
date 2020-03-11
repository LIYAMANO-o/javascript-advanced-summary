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
















