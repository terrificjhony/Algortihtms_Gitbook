## 算法设计的准则
### 面向契约编程

在作者介绍算法的时候，第一件事情往往是给写API，然后再给具体的实现。最初按照这个思路学起来比较费劲，但是到了后来才慢慢理解，这其实是最正确的做法。抽象数据类型(abstract data type)的目的就是给用户(client)提供服务，用户完全不需要知道ADT的具体实现，只需要知道它有哪些功能。因此，首先需要确定一个ADT将要提供哪些服务。API也不只是对客户有帮助，它同样可以帮助实现者明确自己的任务。

#### 典型接口
* Comparable
* Iterable

其中，Compareble接口的实现，是希望传入的对象能够相互比较，而Iterable相当于一个语法糖，相关类在实现的时候需要实现hasNext(),isEmpty()。这样便可以使用`foreach`操作数据。


### 泛型

Java是静态类型语言，并且不同于ML这样的静态语言，它需要**显示声明**参数的类型。因此这就产生了一个**矛盾**：函数需要接受特定的类型，但是该函数又希望适用于所有数据类型。经过一系列的演化，Java最终引入了泛型(generics)。泛型的常见写法如下：

```
private static void stack<Item>{
······}
```







