除了之前介绍过的基本运算符，Swift 还提供了数种可以对数值进行复杂运算的高级运算符。它们包含了在 C 和 Objective-C 中已经被大家所熟知的**位运算符**和**移位运算符**。

与 C 语言中的**算术运算符**不同，**Swift 中的算术运算符默认是不会溢出的**。所有溢出行为都会被捕获并报告为错误。如果想让系统允许溢出行为，可以选择使用 Swift 中另一套默认支持溢出的运算符，比如**溢出加法运算符**（`&+`）。所有的这些溢出运算符都是以 `&` 开头的。

**自定义结构体、类和枚举时，如果也为它们提供标准 Swift 运算符的实现，将会非常有用**。在 Swift 中为这些运算符提供自定义的实现非常简单，运算符也会针对不同类型使用对应实现。

我们不用被预定义的运算符所限制。在 Swift 中可以自由地定义中缀、前缀、后缀和赋值运算符，它们具有自定义的优先级与关联值。这些运算符在代码中可以像预定义的运算符一样使用，你甚至可以扩展已有的类型以支持自定义运算符。