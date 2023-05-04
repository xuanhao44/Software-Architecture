# 1 Introduction

## 1 main concepts

- 首先比较重要的是软件体系结构的定义。
  - The software architecture of a system is **the set of structures needed to reason about the system**, which comprise software elements, relations among them, and properties of both.
- 再一个比较重要的是例子的结论。
  - 两个功能相同的系统可以有不同的架构。
  - 架构决策不是基于功能需求做出的。
  - 架构是由质量需求驱动的。
  - 两个功能不同的系统可以有相同的架构。
- 关于软件体系结构的更多细节主要是进一步解释定义。
  - 软件体系结构是软件系统 (software system) 的结构 (structures)。
  - 软件体系结构是创建这样结构和系统的学科。
  - 再次强调：软件体系结构是一系列软件结构组成的。
  - 软件体系结构是不同于设计 (design) 的。
  - 软件体系结构处于抽象层面。
- 结构和视图 (Views)
  - 由于我们在前面已经说过软件体系结构就是结构 (structure)，所以基本可以等同。
  - Views 是结构的表示。
  - 结构是客观存在的，我们用视图去描述它。
  - 视图画法：用一些符号 (notations) 和线条。
- 好的结构
  - 来自于经验 (rules of thumb)。

## 2 importance

这一块的提到的东西太多太杂，我下面就只把标题的翻译放在下面：

- Inhibiting or Enabling System’s Quality Attributes 抑制或启用系统质量属性
- Reasoning About and Managing Change 对变化的推理和管理
- Predicting System Qualities 预测系统质量
- Enhancing Communication Among Stakeholders 加强利益相关者之间的沟通
- Earliest Design Decisions 最早的设计决策
- Defining Constraints on an Implementation 定义实现上的约束
- Influencing the Organizational Structure 影响组织结构
- Enabling Evolutionary Prototyping 实现进化原型
- Improving Cost and Schedule Estimates 改进成本和进度估算
- Transferable, Reusable Model 可转移、可重用的模型
- Using Independently Developed Components 使用自主开发的组件
- Restricting Design Vocabulary 限制设计词汇
- Basis for Training 培训基础

## 3 many concepts

这个板块的逻辑比较清晰。总的来说，提到了软件体系结构和其背景因素的互相影响的关系，也就是说技术、项目生命周期、商业、专业的背景因素会影响到软件体系结构，而结构也会影响这四个背景因素。所以将其称之为 Architecture Influence Cycle。

另外提到的是利益相关者 (stakeholders)，这也是很重要的一个方面。书上图中给出的例子有：

- Develop Team
- Marketing Team
- End User
- Maintenance Team
- Customer (购买软件的客户，和终端用户还是有区别的)
