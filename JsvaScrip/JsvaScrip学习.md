# ==第一部分.JavaScript==

# 1. 初识JavaScript

## `1.4` 浏览器分为渲染引擎和JS引擎

## `1.5` JS组成

- ECMAScript
- DOM
- BOM

## `第08课- JS`三种书写方式

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>初体验</title>
> </head>
> <script>
>     // 2.内嵌式写法
>     // alert('沙漠骆驼');
> </script>
> <!--3.外部写法-->
> <!--<script src="my.js"></script>   -->
> <body>
> <!--1. 内部写法-->
> <!--<input type="button" value="唐伯虎" onclick="alert('秋香姐')">-->
> </body>
> </html>
> ```
>
> > 附件:`my.js`
> >
> > ```html
> > alert('如果我是DJ')
> > ```



---



## `第09课- JS`注释

> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>   // 1. 单行注释
>  /* 2.多行注释
>   2.多行注释 */
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## `第10课- JS`输入输出语句

> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     prompt('这是一个输入框')
>     alert('这是一个弹出警示框 输出的 展示给用户的')
>     console.log('这是程序员能看到的')
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## `第10课- JS`输入输出语句

> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     prompt('这是一个输入框')
>     alert('这是一个弹出警示框 输出的 展示给用户的')
>     console.log('这是程序员能看到的')
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 





---



## `第13课`变量的使用

1. 声明变量

   1. > var age;
      >
      > 声明一个名称为age的变量

2. 赋值

   1. > age = 10
      >
      > 把10赋给变量

3. 变量的初始化

   1. >var name = 10;

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     var age;   //声明变量
>     age = 18;   // 赋值变量
>     console.log(age)   // 控制台输出结果
>     var myname = '颜霜'
>     console.log(myname)
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## `第22课`数据类型

- 在js中前面加0是八进制
- 十六进制前面加0x



---



## `第23课`判断非数字

- isNAN()
  - 是数字返回false,不是返回True



## `第26课`检测字符串长度

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<script>
    var ma = 'yan shuang'
    console.log(ma.length);   // 检测字符串长度
</script>
<body>

</body>
</html>
```



---



## `第30课`检测变量数据类型

- typeof

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<script>
    var ys = 'uanshaung'
    console.log(typeof ys);
</script>
<body>

</body>
</html>
```



---



## `第32课`转换为字符串类型

> 本节重点:
>
> > ```
> > var num = 10;
> > var str = num.toString();
> > console.log(str)
> > console.log(num + '')
> > ```

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     var num = 10;
>     var str = num.toString();
>     console.log(str)
>     console.log(num + '')
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## `第33课`转换为数字类型

> 本节重点:
>
> - ```
>   // 1.parseInt(变量)   把字符型转换为数字型 得到的是整数
>   // 2.parseFloat(变量)   把字符型转换为数字型,得到的是小数, 浮点数
>       // 3. 利用 number(变量)
>       // 4. 利用算术运算 - * / 隐式转换
>               
>   ```

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     // 1.parseInt(变量)   把字符型转换为数字型 得到的是整数
>     console.log(parseInt('3.14'))   // 取整
>     console.log(parseInt('3.94'))   // 取整
>     console.log(parseInt('120px'))   // 自动去掉px
>     console.log(parseInt('rem120px'))   // 输出NaN
>     // 2.parseFloat(变量)   把字符型转换为数字型,得到的是小数, 浮点数
>     console.log(parseFloat('3.14'))   // 3.14
>     console.log(parseFloat('120px'))   // 去电px
>     console.log(parseFloat('rem120ppx'))   // NaN
> 
> 
>     // 3. 利用 number(变量)
>     vat sty = '123';
>     console.log(Number(sty))
>     console.log(Number('123465'))
>     // 4. 利用算术运算 - * / 隐式转换
>     console.log('10' - 0);
>     console.log('123' - 123)
>     console.log('123' * 1)
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## `第34课`转换为布尔型

> 本节重点:
>
> - Boolean()



---



# `1. 运算符`

> 本章重点:
>
> > 1. 前置递增运算符
> >    1. var age = 10;
> >    2. console.log(++age + 12);
> >       1. 结果:23
> > 2. 后置递增运算符
> >    1. var ages = 10;
> >    2. console.log(ages++ + 12);
> >       1. 结果:22
> >
> > > 代码:
> > >
> > > ```html
> > > <!DOCTYPE html>
> > > <html lang="en">
> > > <head>
> > >     <meta charset="UTF-8">
> > >     <title>Title</title>
> > > </head>
> > > <script>
> > >     var age = 10;
> > >     console.log(++age + 12);
> > >     console.log(age++ + 12);
> > > </script>
> > > <body>
> > > 
> > > </body>
> > > </html>
> > > ```
>
> 2. 比较运算符:
>
>    1. ![image-20210612185733165](https://cdn.jsdelivr.net/gh/yanshaung/pic/image-20210612185733165.png)
>
>    2. 全等于号
>
>       1. ```text
>          ===
>          ```
>
>       2. 三个等于表示全等于

## 9. 逻辑运算符

| 逻辑运算符 | 说明 | 案例          |
| ---------- | ---- | ------------- |
| &&         | and  | true$$false   |
| \|\|       | or   | true\|\|false |
| !          | not  | !true         |



---



## 14. 运算符优先级

![image-20210613141916600](https://cdn.jsdelivr.net/gh/yanshaung/pic/image-20210613141916600.png)



---



## 17. if语句分支

>     if (条件表达式) {
>         执行语句
>     }

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     var age = 10;
>     var ages = 10;
>     if (age == 10) {
>         console.log('对咯')
>     }
> 
>     if (条件表达式) {
>         执行语句
>     }
>     
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## 19. if else双分支语句

if (条件表达式) {
    执行语句
}	else {

执行语句

}



---



## 21. 多分支语句

> ```html
> if (条件表达式) {
>     执行语句
> } else if (条件表达式){
>     执行语句
> } else if (条件表达式) {
>     执行语句
> } else{
>     
> }
> ```



---



## 23. 三元表达式

> var ys = 条件表达式 ? 表达式1: 表达式2;



---



## 25.switch语句

> 本节重点:
>
> >     switch (表达式) {
> >         case value1 :
> >             执行语句1;
> >             break;
> >         case value2:
> >             执行语句2;
> >             break;
> >         ...
> >         default:
> >             执行最后语句;
> >     
> >     }

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     // 1. switch 语句是多分支语句 也可以实现多选一
>     // 2. 语法结构 switch 转换 开关 case 小例子或者选项的意思
>     switch (表达式) {
>         case value1 :
>             执行语句1;
>             break;
>         case value2:
>             执行语句2;
>             break;
>         ...
>         default:
>             执行最后语句;
> 
>     }
> 	// 如果没有break会接着执行下一个case
> 
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



# 2.循环

## 1.for循环

- > 本节重点:
  >
  > ```html
  >     for (var i = 1; i <= 100; i++) {
  >         console.log('颜霜');
  >     }
  > ```
  >
  > 

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     for (var i = 1; i <= 100; i++) {
>         console.log('颜霜');
>     }
> 
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## 2.while循环

1. > ```html
   > while (条件表达式) {
   > 	循环体
   > }
   > ```
   >
   > 



---



## 3.do while循环

> - 先执行循环体
> - 在进行判断

> 代码:
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>     <meta charset="UTF-8">
>     <title>Title</title>
> </head>
> <script>
>     do {
>         循环体
>     } while (条件表达式)
> 
> </script>
> <body>
> 
> </body>
> </html>
> ```
>
> 



---



## 4.退出循环

> - continue
>   - 退出单次循环
> - break
>   - 退出整个循环



---



# 3.数组

## 1.创建数组

> - var ys = new Array();
>   - 使用new创建一个数组
> - var ys = [];
>   - 使用字面量创建数组



---



## 2.数组长度

> - 数组名.length



---



3.追加数组元素

> - ys[3] = '颜霜';
>   - 在数组中第四个位置添加颜霜
>   - 如果该位置有元素其结果为替换该位置元素



---



## 3.添加和删除数组

| 方法名         | 说明                                                     | 返回值               |
| -------------- | -------------------------------------------------------- | -------------------- |
| push(ys...)    | 末尾添加一个或者多个元素,注意修改原数组                  | 并返回新的长度       |
| pop()          | 删除最后一个元素,并把数组长度减一 无参数<br />修改原数组 | 返回它删除的元素的值 |
| unshift(ys...) | 向数组开头添加一个或更多元素<br />注意修改原数组         | 并返回新的长度       |
| shift()        | 删除数组的第一个元素,数组长度减一 无参数<br />修改原数值 | 并返回第一个元素的值 |





---



## 数组排序

| 方法名    | 说明                        | 是否修改原数组          |
| --------- | --------------------------- | ----------------------- |
| reverse() | 颠倒数组中元素的顺序,无参数 | 会改变原数组,返回新数组 |
| sort()    | 对数组的元素进行排序        | 会改变原数组,返回新数组 |





---



## 数组的索引

| 方法名                                       | 说明                           | 返回值       |
| -------------------------------------------- | ------------------------------ | ------------ |
| indexOf()<br />indexOf('查找内容', 开始位置) | 数据中查找给定元素的第一个索引 | 不存在返回-1 |
| lastindexOf()                                | 在数组中的最后一个索引         | 不存在返回-1 |





---



# 4.函数

## 1.创建函数

> 1. 生成函数
>
>    1. ```html
>       > function 函数名() {
>       > 	函数体
>       > }
>       ```
>
> 2. 调用函数
>
>    1. 函数名()
>
> 3. var ys = > function 函数名() { };
>
>    1. 简洁写法





---



## 2.函数的返回值

> - return
>   - 如果没有return则返回 undefined	



---



## 3.raguments特殊属性

> - 接收所有传递过来的参数
> - 展示形式是一个伪数组
>   - 具有length属性
>   - 按索引方式存储数据
>   - 不具有数据的push,pop方法



---



# 5.对象

## 1.创建对象

> - var ys = {};
>   - 创建对象
> - var ys = new Object();
>   - 创建对象2
> - ys.ys;
>   - 调用对象的方法
> - ys['ys'];
>   - 调用对象的方法2
> - ys.ys();
>   - 调用对象的函数



---



## 2.构造函数

> - > ```html
>   >     function 构造函数名() {
>   >         this.属性 = 值;
>   >         this.方法 = function () {
>   >                         
>   >         }
>   >     }
>   >     
>   > ```
>
>   - 构造函数
>
> - new 构造函数名()
>
>   - 使用方法



---



## 3.遍历对象

> - > for (变量 in 对象) {
>   >
>   > }
>
>   - 遍历对象



---



# 6.内置对象

- 内置对象分为三种
  - 自定义对象
  - 内置对象
    - JS自带的对象
  - 浏览器对象



## 1.查找

https://developer.mozilla.org/zh-CN/search?q=max%28%29

 

---



## 2.数学对象Math

| 名称    | 说明          |
| ------- | ------------- |
| random  | 随机数        |
| PI      | 圆周率        |
| floor   | 向下取整      |
| ceil    | 向上取整      |
| round   | 四舍五入      |
| abs     | 绝对值        |
| max/min | 最大值/最小值 |



---



3.Dare日期对象

- var date = new Date();
  - 返回当前系统时间



---



# 7.字符串操作

## 1.数组转换为字符串

| 方法名         | 说明                               | 返回值         |
| -------------- | ---------------------------------- | -------------- |
| toString()     | 把数组转换成字符串,逗号分割每一项  | 返回一个字符串 |
| join('分隔符') | 把数组中的所有元素转换为一个字符串 | 返回一个字符串 |



---



## 2.根据位置返回字符

| 方法名            | 说明                                     | 使用                            |
| ----------------- | ---------------------------------------- | ------------------------------- |
| charAt(index)     | 返回指定位置的字符(index字符串的索引号)  | str.charAt(0)                   |
| charCodeAt(index) | 获取指定位置处字符的ASCII码(index索引号) | str.charCodeAt(0)               |
| str(index)        | 获取指定位置处字符                       | HTML5, IE8+支持 和chartAt()等效 |



---



## 3.拼接以及截取字符串

| 方法名                    | 说明                                                         |
| ------------------------- | ------------------------------------------------------------ |
| concat(str1,str2,str3...) | concat()方法用于连接两个或多个字符串.拼接字符串,等效于+,+更常用 |
| substr(start,length)      | 从start位置开始(索引号), length取的个数 ==重点==             |
| slice(start, end)         | 从start位置开始索引,截取到end位置, end取不到(他们两个都是索引号) |
| substring(start, end)     | 从start位置开始, 截取到end位置, end取不到 基本和slice为相同,但是不接收负值 |



---



## 4.替换字符串以及转换为数组

- replace('被替换的字符串', '替换为的字符串')
  - 替换字符串
- split('分隔符')
  - 字符串转换为数组



---



# ==第二部分.DOM==

## 1.获取元素(数据)

- detElementByld()
  - 可以获取带有ID元素的对象
- getElementsByTagName()
  - 根据标签吗获取
  - 返回带有指定标签名的对象的集合
- getElementsByClassName('类名')
  - 根据类名返回元素对象集合
-  querySelector('选择器')
  - 选择器查找
  - 根据指定选择器返回第一个元素对象



---





## 2.执行事件(鼠标点击)

| 鼠标事件    | 触发条件         |
| ----------- | ---------------- |
| inclick     | 鼠标点击左键触发 |
| onmouseover | 鼠标经过触发     |
| inmouseout  | 鼠标离开触发     |
| onfocus     | 获得鼠标焦点触发 |
| onblur      | 失去鼠标焦点触发 |
| onmousemove | 鼠标移动触发     |
| onmouseup   | 鼠标弹起触发     |
| onmousdown  | 鼠标按下触发     |



### 3.改变网页内容

- element.innerText
  - 从起始位置到终止位置的内容,但它除去html标签,同时空格和换行也会去掉
- element.innerHTML
  - 从起始位置到终点位置的全部内容,包括HTML标签,同时保留空格和换行



---



### 4.样式属性操作

- element.style
  - 行内样式操作
- element.className
  - 类名样式操作



---



5.显示隐藏文本框内容

- 首先需要两个新事件,获得焦点onfous,失去焦点onblur



---



# 第三部分.课后补充

> vue 来定义一个变量除了该方式,还有以下两种方式

- let(变量)
- const(常量)
