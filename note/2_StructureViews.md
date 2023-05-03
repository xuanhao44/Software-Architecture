# Architectural structures and views

参考资料：https://blog.csdn.net/qq_29025955/article/details/123908794

看到标题先回顾一下 Introduction 里的区分这俩东西的部分：视图是结构的表示。

这篇的大纲就是先讲几种结构，再讲一些视图，最后是软件体系结构的文档（视图 + 其他说明的部分）。还需要注意的前提是：这里讲到的结构和视图、还有构建文档的知识都只列举的一部分而非全部。

## 1 Architectural structures

介绍了三种结构：模块结构、组件 - 连接器结构、分配结构。实际上在理解这些的时候就有一个难点就是，我们对结构的理解就是一个结构由很多个块组成——这让我们之只能想到模块结构，而不太能理解其他两种结构。

组件 - 连接器结构：我的理解是这里的组件确实是较为实际的部分，而这些部分之间有各种交互，这种交互用连接器（一些线条）来表示。

分配结构：将组件 - 连接器结构或者模块结构映射到非软件的事物上去：如、通常是硬件、团队及文件系统。所以这种结构讲的是如何部署 (Deployment)，或者结构中的元素是如何映射到文件结构中的 (Implementation)，或者各个模块是由什么团队进行负责的 (Work Assignment)。

看了这些之后就能隐隐的理解到，三种结构之前似乎有着某种递进的关系——逐渐的变得具体了起来。详细的对比见 PPT。

具体的在参考资料中理解：https://blog.csdn.net/qq_29025955/article/details/123908794

## 2 Views

视图这块没什么好说的，就是讲了定义、用途等。需要关注的点有：用的符号、对应不同类结构的视图。

符号中强调了非正式的符号 UML，同时 符号的选择还是要考虑实际情况，即做出取舍和选出最适合的。

对应不同类结构的视图就是上面讲的三种结构对应的视图。

## 3 Documentation

构建软件体系结构的文档这块的点就比较多了，不仅和作业有关，比较重要的知识也不少。

---

首先是**如何选择视图**。在学习了这么多种类的视图之后，应该是能根据实际的结构选择合适的视图的。同时，我们也可以从标准中寻找到启示。最后，从不同的**利益相关者**的角度也能有不同的视图，比如终端用户和开发者对于一个系统的视图就可以是不一样的。

需要注意的是，上面提到的都是选择视图的办法（不过也许能从中产生出新种类的视图），故而之前第二部分讲的一些视图就是用来在这个环节备选的，两者并不矛盾。

关联作业：[Exercise3_ans](../exercise/Exercise3_ans.md) 就是为当前系统创造两个不同于 PPT 已有的视图，老折磨了。

---

4+1 View Model 和 C4 Model 略。

---

最后提到的是文档包 (Documentation Package)。构成就是 views + documentation（比较宽泛的概念，没啥大用）。

关于 Document Behavior 能说的比较多，因为很多都是熟悉的知识。比如：

- Use Case Diagram, Use Case Description 用例图和用例描述
- Sequence Diagram 序列图
- Communication Diagram 协作图
- Activity Diagram 活动图