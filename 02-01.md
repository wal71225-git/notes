# 函数式编程概念
-函数式编程：对运算过程进行抽象 例如：y=f(x)
-函数式编程中的函数指的是不是函数中的方法，而是数学中的映射关系。
-相同的输入得到相同的输出
//函数式编程概念
//非函数式
let num1 = 1;
let num2 = 2;
let sum= num1 + num2;

//非函数式
function sum(num1,num2){
    return num1 + num2;
}
let result = sum(2,3);


# 1.函数是一等公民

 *函数可以存储在变量中
 *函数可以作为参数
 *函数作为返回值
 

# 2.高阶函数

*把函数作为参数传递给另一个函数
function forEach(array,fn){
    for (let i = 0; i < array.length; i++) {    
        fn(array[i]);
    }
}

let array = [1,3,5,7,9];
forEach(array,item => {
    console.log(item);
})

*把函数作为另一个函数的返回结果


# 3.常用的高阶函数
-map
-forEach
-fitter
-reduce