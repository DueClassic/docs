##### 函数式编程思想

什么是函数式编程？

> In computer science,functional programming is a programming paradigm-a style of building the structure and elements of computer programs-that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

- 纯函数（Pure Function），或函数的纯粹性（Purity），没有副作用（Side Effect），副作用是指状态的变化（mutation）

- 引用透明（Referential Transparency）对于相同的输入，总是得到相同的输出，如果f(x)的参数x和函数体都是引用透明的，那么函数f是纯函数。

```scala
//违反引用透明
var x=new StringBuilder("Hello")
> x : StringBuilder = Hello
var y=x.append(" World!")
> x : StringBuilder = Hello World!
var z=x.append(" World!")
> x : StringBuilder = Hello World! World!
```

不变性（Immutability）为了或得引用透明性，任何值都不能变化

- 函数是一等公民（First-class Function）一切都是计算，函数式编程中只有表达式，变量、函数都是表达式

  高阶函数（Higher order Function）

  闭包（Closure）

- 表达式求值策略：严格求值 和 非严格求值

  惰性求值（Lazy Evaluation）

- 递归函数（Recursive Function）

  递归实现循环

  尾递归（Tail Recursion）

