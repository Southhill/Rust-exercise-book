## Rust exercise book
这是对rust官方教程上的案例实践
## 实践的案例
- 猜猜看

程序将会随机生成一个 1 到 100 之间的随机数。它接着会提示猜一个数。当我们猜了一个数之后，它会告诉我们是太大了还是太小了。猜对了，它会祝贺我们。
- 哲学家就餐问题

一个经典的并发问题。它叫做“进餐（ji）的哲学家”。

- Rust最强实力的功能：缺少实质的运行时。

启动10个线程。在每个线程中，从1数到500万。在所有10个线程结束后，打印“done”。
使用Javascript调用rust生成的库文件。

## 相关链接
- [Rust官方教程中文版](http://rustbook.cn/)
- [Rust官方网站](https://www.rust-lang.org/zh-CN/)

## 不那么重要的知识点

- 通常来讲，使用一个更慢的，不过提供了更强大的程序员生产力的语言是一个值得的权衡的问题。为了帮助缓和这个问题，它们提供了一个用C编写部分你的系统，然后接着用高级语言编写的代码调用C代码。这叫做一个“外部函数接口”，通常简写为“FFI”。
- 遮盖（赋值）：定义一个与之前变量重名的新变量，而新变量会遮盖之前的变量。这意味着使用这个变量时会看第二个值。可以用相同变量名称来遮盖它自己，以及重复使用 let 关键字来多次遮盖。  
这与将变量声明为 mut 是有区别的。因为除非再次使用 let 关键字，不小心尝试对变量重新赋值会导致编译时错误。我们可以用这个值进行一些计算，不过计算完之后变量仍然是不变的。
mut 与遮盖的另一个区别是，当再次使用 let 时，实际上创建了一个新变量，我们可以**改变值的类型**。
- **语句（Statements）是执行一些操作但不返回值的指令。表达式（Expressions）计算并产生一个值。**在**Rust**中表达式并不包含结尾的分号。如果在表达式的结尾加上分号，他就变成了语句，这也就使其不返回一个值。
- 类型转换：Rust 并不会尝试自动地将非布尔值转换为布尔值，Rust 需要在编译时就确切的知道该处变量的类型，这样它就可以在编译时证明其他使用该变量的地方它的类型是有效的。
