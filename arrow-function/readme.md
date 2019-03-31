# 箭头函数 即 匿名函数
let fun = ()  =>{
    consloe.log('lala');
}
-  箭头函数是 匿名函数 不能作为构造函数， 不能使用new
构造函数：
 function Person（name）{
     this.name =name;
     consloe.log(name);
 }
 const p1 = new Person('cst');
- 箭头函数不能绑定 arguments，取而代之用 ...rest参数 解决
- 箭头函数不能绑定 this 
- 箭头函数没有原型属性
##  怎么用
只有一个参数时， 可以省去 ( )
只有一条语句的时候 可以省去 {  return }

## 注意
参数,箭头之间不能换行
返回一个对象时候

## arguments
普通函数可以定义重复的形参 functoin f(a,a){ }
- 所有函数里面 (除了箭头函数之外) 都可以用的变量
- [arg1,arg2,arg3]

## 区别
- 箭头函数不支持重复命名形参，普通函数可以
- 箭头函数不能使用call apply 等方法改变 this 的指向
- 箭头函数没有 this 它的 this 指向定义时所处的上下文（外部函数）的 this 
- 箭头函数没有原型对象 .prototype
- 箭头函数不能作为构造函数
- 箭头函数没有 arguments 

## new.target
- es6 引进的 返回 new 作用的那个构造函数（构造函数之中）
