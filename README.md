# yexingyu.github.io
### 准备
 这里是叶星宇的博客，正在学习如何进行各种操作。
 
 以下为Javascript学习内容


 



			可以将js代码写到外部js文件中，然后通过script标签引入
			引用后不能再在这个script标签中编写代码，可以新建一个标签编写


		<!--<script type="text/javascript" src="scripts/main.js"></script>-->
      
          <script type="text/javascript">
	      document.write("hello");
        // 向text中写入内容


         //alert("hell");
		 //弹窗内容


		 //console.log("hello");
		//控制台输出










/*
字面量和变量：
		字面量：一些不可改变的值，可以直接使用（12343等）
        变量：保存字面量。
		var:声明变量


		标识符：自主声明的字符



数据类型
		String  字符串   打引号或双引号
		Number  数值   浮点数，整数   ***Infinity表示正无穷，加负号表示负无穷Number.MAX_VALUE    ***NaN  表示不是数字（NaN是数字） Number.MIN_VALUE表示0以上的最小值
		                进行浮点数运算时得到的结果可能不精确
		Boolean 布尔值  只有两个，用于逻辑判断   真  假  true  +表示真     false    -表示假   var bool=ture;
		Null    空值  只有一个  就是null   var a = null   专门用来表示一个为空的对象  用typeof检查类型时会返回object
		Undefined  未定义     只有一个undefined 声明变量未赋值时为此类型                                                     前五个为基本数据类型
		Object    对象    引用数据类型
		用typeof检查类型
		*/
		//var str = "hello";
		//str = "hhh";
		//console.log(Number.MAX_VALUE);//输出最大数
		//alert (str);//弹窗
		/*
		数据转换   例子：一：将其他类型转换为String
		1.调用（）的toString方法   该方法不会影响原变量，会将转换的结果返回
		调用xxx的yyyfangfa   即   xxx.yyy()
		例：
		var a = 123;
		var b = a.toString();
		console.log(typeof b);
		console.log(b);
		注意  null和undefind没有toString();
		2.调用String函数将a转换为字符串；
		a=String(a);
		*****对于Number和Boolean实际上是调用toString方法
		*****但对于null和undefined就不会调用，将null直接转换为“null”，后者一样
		
		二：将其他类型转换为Number
		1.使用Number函数
		a = Number(a);
		纯数字字符串直接转化为数字
		有非数字内容转化为NaN
		字符串是空串或全是空格的字符，则转化为0
		布尔值true转化为1，false转化为0
		Null转化为数字0
		undefined转化为数字NaN
		2.
		专门用来对付字符串的方法
		parseInt()把一个字符串转化为一个整数
		parseFloat()把一个字符串转化为一个浮点数  a = parseInt(a);如果a = 123qwer231   输出为123，231无法输出
		这个函数先将数据类型转换为string，再进行处理
		三：
		将其他类型转化为boolean
		var a=123;
		a=boolean(a);
		数字转boolean，除了0和NaN，其他都是ture。
		字符串转boolean，除了空串，其余都是ture。
		null和undefined都是false。





算术运算符：
	   +：
	   对非number（除字符串）运算自动转为number

	   任何值与NaN运算都得NaN

	   两个字符串 相加  拼串
	   如：
	   var a = qwe+
	   rty+
	   uiop;
	   输出a为qwertyuiop。

	   有字符串，把其他转换为字符串拼串

	   console.log("a = "+ a);
	   输出为a = 123.




	   -：把其他类型转化为number运算



	   *：把其他类型转化为number运算


	   /：把其他类型转化为number运算



	   %：取模运算



一元运算符
	   +：正号
	   -：负号



自增自减：
a++      a--    ++a      --a

		
        
		
		
		
进制
		js中，输出16进制数，用0x开头（输出时都会转化为10进制输出）
		0开头为8进制      0b开头为2进制（部分浏览器不支持）
		

逻辑运算符
       与  &&
	   或  ||
	   非  ！
	   布尔值运算

	   非布尔值运算
	   &&
	   俩个值都时true，则返回后者，如：  1&&6返回6
	   前false则返回前者，前true返回后者
	   ||
	   与&&xiangfan
	   都为true返回前者



赋值运算符：
       将右侧值赋给左边变量




关系运算符
      <
	  >
	  >=
	  <=
	  ==(会自动进行字符转换)
	  ===（全等）
	  ！=(自动进行类型转换)
	  ！==(不全等)
	  比较两个数大小关系



条件运算符
      条件表达式?语句1:语句2;
	  运算流程：
	  首先对条件表达式进行求值，
	  如果值为true，执行语句一；如果值为false，执行语句2.
	  var max = a > b? (a > c? a : c) : (b > c? b : c);      

      
代码块
		用{}来为代码分组，叫代码块，要么都执行，要么都不执行
		内部内容可以在外部访问
	



条件判断语句
     语法1   if语句
	 if（条件表达式）
	 语法2   
	 if（）
	 {
		语句1
	 }
	 else
	 {
		语句2
	 }

语法3
     if（）
     else if（）
      else if（）
     else ...


条件分支语句
      switch语句
   语法：
      case 1 ：
      语句
      case 2 ：
      语句
          ............,搭配break；
     default：
     语句
     break；




循环语句
      while循环
       do while循环
      for循环

    var score  =  prompt("请输入内容")
           用于输入内容的函数prompt 


    console.time("test");
          语句；
    console.time("test");
         用于测试运行时间；


     通过Math.sqrt()
             开平方

对象 
     string  字符串
     Number  数字
     Boolean  布尔值
     Undefind  未定义

     只要不是以上5种基本数据类型，都是对象
     基本数据类型都是单一的值
     值和值之间没有任何联系
     Object 对象
     对象属于一种复合的数据类型，在对象中可以保存不同数据类型的属性
     对象的分类
     1.内建对象
          由ES标准中定义的对象，在任何ES的实现中都能使用
     如  Math String Number Boolean Function Object
     2.宿主对象
       由JS运行环境提供的对象
     3.***自定义对象***



     创建对象
      使用new关键关键字调用的函数constructor*/

     //向对象中保存的值称为属性
     //向对象中添加属性
     //语法： 对象.属性名 = 属性值
//var obj = new Object();
//obj.name = "帅哥";
//obj.gender = "男";
//obj.age= 18;
     //读取对象中的属性值
//console.log (obj);
     //语法： 对象.属性名
     //修改对象中的属性值
     //语法： 对象.属性名 = 新值
//obj.name = "tom";
     //删除对象属性
     //语法：delete 对象 属性名
//delete obj.name;

     //对象随意取名，不能用点！

/*
使用特殊的属性名，不能采用.的方式
需要用[]
格式：对象["属性名"] = 属性值
使用[]这种形式去操作属性，更加的灵活
在[]中可直接传递一个变量，这样变
量值是多少就会去读取那个属性


举例*/


/*var obg = new Object;
obg["123"]=789;
obg["nihao"]="你好";
var n = "nihao";
console.log(obg[n]);*/


//输出   你好
/*对象指向对象
如
var text = new Object;
obg.text="大哥";
*/

/*in 运算符
//可以检测对象中是否有对应的属性
//有返回true  没有返回false
//语法
//属性名  in 对象
如 */  
//console.log("text2" in obg);


//对象字面量：
/*var obg2 = {
	name : "帅哥",
	age : "20"
}*/
//更好的简单的进行定义字面量
		//console.log(obg2);





//函数
      //函数也是对象  
      //创建一个函数对象
    //var fun = new Function("console.log('Hello,hanshu');");
	//或function 函数名 ([形参1，形参2，......]){语句...}
      //函数声明
	  /*function fun (){
		console.log('Hello,函数');
	  }
	  //调用函数
	fun();
	  */
	 //函数表达式
      //var 函数名 = function ([形参]){语句}；
      //匿名函数，赋值给变量
      


	  //函数的参数
	/* function sum(a,b){
		console.log(a+b);
	 }
	 
     sum(100,100);
	 */
     //实参可以传入对象，也可以传入函数



//函数的返回值
	  //使用return，其后不接值或不写return返回undefined
	   //fun函数名   :调用函数
       //fun函数名() :函数对象
       //返回值也可以是对象或函数


//立即执行函数
       /*(function(a){
	       console.log("a = "+a);
        })(8);
		*/
         //函数的属性值也可以是函数，调用这个函数就叫调用这个对象的方法


//枚举对象中的属性语法
        //for (var 变量 in 对象){ console.log("属性名 = " +n);    console.log("属性值 = "+obg[n]) ;  }
		//每次执行会将属性赋值给变量
		
		
		
//this 		
        /*解析器调用函数时每次都会向内部传递一个隐含的参数
		这个参数就是this  this指向的是一个对象
		根据函数调用方式的不同，this会指向不同的对象
		1.函数形式调用时，this指向window
		2.方法形式调用时，this指向点调用方法的对象
		例子                                */
		/*function fun(){
			console.log(this);
		}
		//fun();
		var obg3 = {
			name : "第一",
            sayname: fun
		}
		var obg4 = {
			name:"第二",
			sayname: fun
		}
		//fun();
		obg4.sayname();  */



//构造函数
       /*
      *function Dog(name)
      {
	      this.name = name;
	      this.sayname = function(){
		      alert(this.name);
	      }
      }
      var a = new Dog("帅哥");
                                                           */


/*原型函数
        原型prototype
		创建的每一个函数，解析器都会向函数中添加一个属性
		函数作为普通函数调用时prototype没有任何作用
		函数以构造函数的形式调用时，他的对象中都会有一个隐藏属性
		指向该构造函数的原型对象，通过__proto__来访问
		*/
		/*function Myclass(){
           
		}*/
        //向Myclass中添加属性a
		/*Myclass.prototype.a = 12345;
		var q = new Myclass();
		var w = new Myclass();
		q.a= "q内";
		w.a="w内";
		//q内没有a则到prototype中找a
		console.log(q.a);
		//像原型作用域中添加sayName
		Myclass.prototype.sayName = function(){
			alert("Hello,我是：");
		}
		console.log(q.sayName);
		*/
		
//tosring



		/*function Person(name,age,gender){
			this.name=name;
			this.age=age;
			this.gender=gender;
		}
		
		var per = new Person("帅哥1",18,"男");
		var per2 = new Person("帅哥2",19,"男");
                   //当我们直接在页面中打印一个对象时；事实上输出的是tostring()方法的返回值
                   //如果我们希望在输出对象时，可以为对象添加tostring()方法
		Person.prototype.toString = function(){
			return "Person[name="+this.name+",age="+this.age+",gender="+this.gender+"]"
		}
		console.log(per2);
		*/
		
		
//数组   Array    是一个对象
 /*        //创建数组对象
		 var arr = new Array();
		 //使用字面量创建数组
		 var arr = [1,2,3,4,5];(分别为5个元素)
		 //使用构造函数创建数组，可在创建时就指定数组中的元素
		 var arr2 = new Array(7);(长度为7)
		 //向数组中添加元素  数组[索引]=值
		 arr[0]=10;
         arr[1]=20;
		 arr[2]=30;
		 arr[7]=70;
		 console.log(arr);
         //使用length设置或获取数组长度(元素个数)
		 console.log(arr.length);//获取
		 arr.length = 10;//设置
		//向数组最后添加元素
		arr[arr.length] = 220;
		arr[arr.length] = 320;
		arr[arr.length] = 420;
*/
//       数组元素可以是任意类型
/*
        arr = ["hello",1,true,null,undefined];
        也可以是对象
		var obj = {name:"帅哥"};
		arr[arr.length] = obj;
		console.log(arr[5].name);
		也可以是函数
		arr = [function(){alert(1)},function(){alert(2)}];
		也可以放数组
		arr = [[1,3,4],[2,5,6]];
                       */
//数组的方法
/*concat()  连接两个或更多的数组并返回；     数组名.concat(数组名，数组名,'a')，不会改变原数组
join()  把数组所有元素放入一个字符串，元素通过指定分隔符进行分隔    数组名.join(<>),括号中的内容分隔每个元素
pop()   删除并返回数组的最后一个元素    修改原数组
***push()  向数组末尾添加一个或更对元素，并返回新的长度
reverse()  颠倒数组中元素的顺序    修改原数组，arr.reverse()
shift()  删除并返回数组的第一个元素
slice()  从某个已有的数组返回选定的元素     数组名.slice(0,2);取得0和1;不变原数组，数组名.slice(1);取1后所有元素
sort()  对数组元素进行排序   arr.sort(),按Unicode编码排序
内可指定排序规则
在sort中添加回调函数  定义两个形参
根据返回值决定元素顺序，返回0，负数，位置不变，返回大于0的数，交换位置
arr.sort(function(a,b)){
if(a>b){
	return 1;
}else if(a<b){
	return -1;
}else{
	return 0;
}
}
//或
arr.sort(function(a,b)){
	return a-b;
}


splice()  删除元素并向数组中添加新元素   数组名.splice(0,2,'a','b');会改变原数组，删除1，2；并将0，1，元素改为a，b
toSource()  返回对象的源码
toString()  把数组转换为字符串并返回结果
toLocaleString()  把数组转化为本地数组，并返回结果
unshift()  向数组开头添加一个或更多元素，并返回结果
valueOf()  返回数组对象的原始值
*/
/*
		var arr = ["a","b","c"];
        arr.push("小叶","xiaoye");
		console.log(arr);
		result=arr.pop();
		console.log("result = "+result);
*/
//数组遍历（循环）
//forEach()遍历
//需要函数做参数
         /*var arr = [1,2,3,4,5];
        arr.forEach(function(a,b,c){
	    console.log("a = "+a);
	    console.log("b = "+b);
	    console.log("c = "+c);
	       //a为元素，b为角标，c为整个数组
         });    */
        //数组中有几个元素函数执行几次,每次执行时会将遍历到的函数以实参的形式传递出来，我们可以定义实参读取这些内容
//call()和apply  都是函数对象的方法，需要通过函数对象调用
/* function fun(a,b){
		//alert(this.name);
		console.log("a = "+a);
		console.log("b = "+b);
	 }

	 var obj = {
		name:"obj",
		sayname:function(){
			alert(this.name);
		}
		};
      fun.apply();
	  fun.call();
	  fun();
	 在调用call和apply可以将一个对象指定为第一个函数 
	 此时这个对象将会成为函数执行时的this
	  call可以将实参在对象之后依次传递
      apply方法需要将实参封装在数组中

		fun.call(obj,1,2);
		fun.apply(obj,[1,2]);

		var obj2 = {name:"obj2"};    */
		//fun.call(obj);
		//fun.apply(obj);
		//obj.sayname.apply(obj2);
		

//arguments    是一个类数组对象，可以通过索引获取数据，也可以获取长度
/*
      在调用函数时，所使用的实参都会在arguments中保存
	  arguments.length可以用来获取实参的长度
	  不定义形参，也可以通过arguments来使用实参
	  arguments[0]表示第一个实参，arguments[1]表示第二个实参，。。。。
	  里面有一个callee属性，就是当前正指向的函数对象
*/
//Date 对象  表示一个时间
       /*使用构造函数创建一个Date对象，则会封装为当前代码执行的时间
       var d = new Date();
       console.log(d);
       */
//创建一个指定时间的对象，需要在构造函数中传递一个表示时间的字符串作为参数
 //月 日 年 时
 /*    
        var d2 = new Date("11/3/2019 11:12:3");
        console.log(d2);
*/
      //  getdate()  获取当前日期  几日
      //  getDay()   获取当前日期为该星期的第几天，返回0——6，0表示周日
	  //  getMonth()  获取月份 返回0——11，0表示一月
      //  getFullYear() 获取年份 
	//    getHours(),getMinutes(),getSenconds(),    getMilliseconds()获取毫秒
    // getTime()  获取当前对象的时间戳，时间戳指从格林威治标准时间的1970年1月1日0时0分0秒到当前日期所花费的毫秒数(1秒=1000毫秒)


//Math    与其他对象不同，不是一个构造函数，属于工具类，封装了数学相关属性和方法
/*    math.PI  圆周率，还有LN2,LN10,LOG2E,LOG10E,SORT2等
      abs(x)	返回 x 的绝对值。
      acos(x)	返回 x 的反余弦值，以弧度为单位。
      acosh(x)	返回 x 的双曲反余弦值。
      asin(x)	返回 x 的反正弦值，以弧度为单位。
      asinh(x)	返回 x 的双曲反正弦值。
      atan(x)	返回 x 的反正切值，返回的值是 -PI/2 到 PI/2 之间的弧度值。
      atan2(y, x)	返回其参数商的反正切值。
      atanh(x)	返回 x 的双曲反正切值。
      cbrt(x)	返回 x 的三次方根。
      ceil(x)	返回 x，向上舍入为最接近的整数。
      clz32(x)	返回 x 的 32 位二进制表示中前导零的数量。
      cos(x)	返回 x 的余弦值（x 以弧度为单位）。
      cosh(x)	返回 x 的双曲余弦值。
      exp(x)	返回 Ex 的值。
      expm1(x)	返回 Ex 减去 1 的值。
      floor(x)	返回 x，向下舍入为最接近的整数。
      fround(x)	返回数的最接近的（32 位单精度）浮点表示。
      log(x)	返回 x 的自然对数。
      log10(x)	返回 x 的以 10 为底的对数。
      log1p(x)	返回 1 + x 的自然对数。
      log2(x)	返回 x 的以 2 为底的对数。
      max(x, y, z, ..., n)	返回值最高的数字。
      min(x, y, z, ..., n)	返回值最小的数字。
      pow(x, y)	返回 x 的 y 次幂值。
      random()	返回 0 到 1 之间的随机数。
      round(x)	将 x 舍入为最接近的整数。
      sign(x)	返回数的符号（检查它是正数、负数还是零）。
      sin(x)	返回 x 的正弦值（x 以弧度为单位）。
      sinh(x)	返回 x 的双曲正弦值。
      sqrt(x)	返回 x 的平方根。
      tan(x)	返回角度的正切值。
      tanh(x)	返回数的双曲正切值。
      trunc(x)	返回数字 (x) 的整数部分
      */























		
	
	

		



		

