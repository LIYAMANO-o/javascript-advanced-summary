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
  简单值  JavaScript中的数组是通过数字索引的一组任意类型的值，字符串和数组类似，但是他们的行为特征不同。基本类型中定义了几个特殊的值。null类型只有一个值null，undefined类型也只有一个值undefined，所有变量在赋值之前默认值都是undefined，void运算符返回undefined，数字类型有几个特殊值包括NAN。
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


