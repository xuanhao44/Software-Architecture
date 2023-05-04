# Patterns and Tactics

这一章的内容不多，就是讲了一些常见的模式，是按照和结构对应的分类来讲的。不过更值得关注的是后面两个部分。

模式和策略的关系：从 策略 (tactics) 到 模式 (pattern)。一个模式只用于满足某个特定的质量要求，这样可能会影响到其他的质量要求的实现。

所以顺理成章的来到了 tactics 之间的关系——我更倾向于这是在讲述如何从一个 tactic 变成一个 pattern（特定的）的过程。我们在使用了一个策略的时候，我们也引入了副作用。继续使用其他的策略可以消减这种副作用的影响，直到我们应用的足够的策略，使得这些副作用小到可以忽略，或者说已经满足了系统的要求，那么这时就停止了策略的拓展，也就成了一种模式。

书中给出了很好的例子：

<img src="../pic/Tactics and Interactions.png" alt="Tactics and Interactions" style="zoom:33%;" />

- 那么首先是使用了 ping/echo 的策略来保障了可用性，但是引入这个监测器可能带来三个问题，第一个是增添了实体，第二个是 ping 洪流，第三个是产生性能开销。
- 所以我们需要继续使用性能相关的策略来尽量消除这些副作用。我们选择了增加可用的资源，但这又引入了新的问题：成本，以及资源利用（效率）的问题。
- 为此，我们继续使用性能相关的策略——调度策略。然而该策略也存在一些问题，也就是需要把调度策略加入到系统中，例如向系统添加调度器，而这涉及到可修改性。
- 继续，我们使用可修改性中的策略——使用中介。显然，使用中介又会有副作用...

这就是不断应用策略的过程。