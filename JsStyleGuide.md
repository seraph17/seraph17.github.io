# Airbnb Javascript 编码规范（ES6）笔记

---

*A mostly reasonable approach to JavaScript*

[原文](https://github.com/airbnb/javascript)

## 1. Types

* 1.2 的例子可以看出，const 引用对象本身可以改变

    ```javascript
    const foo = [1, 2];
    const bar = foo;

    bar[0] = 9;

    console.log(foo[0], bar[0]); // => 9, 9
    ```


## 2. References

* 优先使用 const，其次使用 let，避免使用 var
* const 和 let 都是块级作用域


## 3. Objects

* 可使用表达式作为属性名
* 可使用对象方法的简写
* 使用属性值的简写时应放在最前面


## 4. Arrays

* 使用扩展运算符 ... 拷贝数组
* 使用 from() 把一个类数组对象转换成数组
* 4.5没看懂？？？


## 5. Destructuring

* 使用解构访问对象和数组，可减少临时变量
* 需要返回多个值时，使用对象解构而不是数组解构


## 6. Strings

* 过长的字符串，应使用**连接符**分行。但是过多使用会影响性能？？？
* 使用模板字符串


## 7. Functions

* 不要使用arguments，可使用 ... 代替
* 给函数设定默认参数，而不要改变参数


## 8. Arrow Functions

* 使用箭头函数代替匿名函数，this会绑定
* 如果一个函数适合用一行写出并且只有一个参数，那就把花括号、圆括号和 return 都省略掉。如果不是，那就不要省略。


## 9. Constructors

* 总是使用 class，避免直接操作 prototype
* 使用 extends 继承
* 如果没有指定，类有默认的构造函数


## 10. Modules

* 建议使用 ES6 模块。可以编译成其他非标准模块系统。


## 11. Iterators and Generators

* 不要使用 iterators
* 现在不要使用 generators, 因为不能很好的编译成 ES5


## 12. Properties

## 13. Variables

* 用 const 声明每一个变量
* 在合理的地方声明变量，因为 let 和 const 是块级作用域(不会提升)


## 14. Hoisting

* 注意 let 和 const 的暂时性死区


## 15. Comparison Operators & Equality

## 16. Blocks

## 17. Comments

## 18. Whitespace

## 19. Commas

## 20. Semicolons

## 21. Type Casting & Coercion


