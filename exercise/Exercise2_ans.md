# Exercise 2

- Based on the ASRs from your own Utility Tree, create a design fragment using the ADD method employing and instantiating a pattern.
- Submission:
  - Deadline: April 21st
  - Place: submit to Blackboard

## Reference

- Each student’s design will be different, depending on which fragment of the system the student will choose to focus on and which architectural pattern they choose.
- You just need to show one part of the design.
- We have performed the first step in class, below is our design. For your assignment you could pick any of the components from our design (for example an Web client) and decompose it into components – you could choose a layered pattern as shown in the example below.

<img src="../pic/exercise 2 example ans.jpg" alt="exercise 2 example ans" style="zoom:50%;" />

## My answer

round 1: Availability, Choose **Heartbeat Monitor**

<img src="../pic/exercise_2_round1.jpg" alt="exercise_2_round1" style="zoom:80%;" />

round 2: Security, Choose **firewall**.

![exercise_2_round2](../pic/exercise_2_round2.jpg)

## 反思

在老师给出参考和重新读了 PPT 之后，发现我原来的回答有问题。

先来回顾：

- **Design Strategy** - Decomposition
- The Steps of Add

  1. **Choose an element** of the system to design.
  2. **Identify the ASRs** for the chosen element.
  3. **Generate a design solution** for the chosen element.
  4. **Inventory remaining requirements** and select the input for the next iteration.
  5. Repeat steps 1–4 until all the ASRs have been satisfied.

所以要做的是事情大体上是**分解模块**。

步骤上说就是

1. 选择系统中的一个部分作为一轮 ADD 的主题。
1. 为该主题找到对应的 ASR。
1. 做出决策，也即选择 ASR 对应的质量要求的 Tactics。

之后就是重复。

---

显然我之前的答案不太合理——没有选择一个部分当主题，虽然结果上看上去是对着 ATM client 进行了两轮的循环，第一次处理了 Availability，第二轮处理了 Security，但没有体现出分解。这点比较 Reference 里的图示就很容易发现。
