# Software Architecture

软件体系结构

## 老师

Joanna Siebert

## 分数构成

- 10% - participation – class activities（homework 貌似没有，作业实际被称为 exercise）
- 30% - practical exercises
- 60% - final examination

## 考勤

报这门课的人比较少，2023 年春的课程中仅有 20 人选了这门课，然后实际来上课的人每节课不超过 7 - 8 人。

所以在第 2 - 3 节课开始，老师就开始在课间让同学们挨个签到了。同时因为人少，所以不存在帮人写名字的可能性——老师会点一遍班上人数然后和写的名字数量对照一下。

所以如果选了这门课请务必要来。

## 考试

- 形式
  - Open book 开卷
  - Multiple choice questions – 10 questions, 3 points each 单选题！
  - Short description questions – 5 questions, 6 points each
  - Case questions – 4 questions, 10 points each, 40 points in total
- 详细信息：见 [slide/25_review.pptx](slide/25_review.pptx)。
- 考试准备资料：见 for_test，note 以及 exercise 文件夹。

---

考试感想：TODO

## 参考书籍

找到的参考书的 GitHub 翻译仓库：

<https://github.com/suseme/sw_arc_in_p>

以及 gitbook 链接：

<http://arc.misday.com>

在 PPT 的构造实在看不懂的时候就该看看参考书了。目录能让你知道 PPT 那么多页大概是什么逻辑展开的，更详细的信息也都从书上来。

## 仓库构成

- slide：老师上课的 PPT，仅对名称进行微调。
- exercise：四次作业。
  - ATM System Requirements.pdf 是所有四次作业的阅读材料。
  - Homework 4.pdf 是第四次作业的阅读材料。
  - 每次作业都有一个 PPT，我的答案写在 ans 的 markdown 文档中。
- for_test：考试用精简 PPT，比起原本的 PPT 精修了一遍，比原本的 PPT 更适合阅读。(不包含 course design 和 review)
  - *introduction 的 word 是个失败的尝试，感觉还是看 PPT 好点。*
- note：包含各章节的笔记。

## PPT 的 分 Part

**首先建议看 for_test 中的整合版 PPT**。

从 review 中看来的，能分成三个 Part。

- Part 1 Introduction of software architecture
  - [1_Introduction.pptx](for_test/1_Introduction.pptx)
  - [2_Architectural_structures_and_views.pptx](for_test/2_Architectural_structures_and_views.pptx)
- Part 2 Quality attributes
  - [3_Understanding_quality_attributes.pptx](for_test/3_Understanding_quality_attributes.pptx)
  - [4_Availability.pptx](for_test/4_Availability.pptx)
  - [5_Interoperability.pptx](for_test/5_Interoperability.pptx)
  - [6_Modifiability.pptx](for_test/6_Modifiability.pptx)
  - [7_Performance.pptx](for_test/7_Performance.pptx)
  - [8_Security.pptx](for_test/8_Security.pptx)
  - [9_Other_quality_attributes.pptx](for_test/9_Other_quality_attributes.pptx)
  - [10_Patterns_and_tactics.pptx](for_test/10_Patterns_and_tactics.pptx)
  - [11_Quality_Attribute_Modelling_and_Analysis.pptx](for_test/11_Quality_Attribute_Modelling_and_Analysis.pptx)
- Part 3 Architecture in the life cycle
  - [12_Designing_for_ASRs.pptx](for_test/12_Designing_for_ASRs.pptx)
  - [13_Evaluating_architecture.pptx](for_test/13_Evaluating_architecture.pptx)

## 笔记构成

- 1，2，3，10，11，12 是概念较多的章节，所以在 pic 文件夹中你能看到 md 格式的思维导图，可在 VS Code 中使用 Markmap 插件查看图（当然 PNG 格式的图也有一份）。
- note 中不包含某些特别简单和没什么笔记的章节，如 9、11、13。
  - 9 就是很简单的其他没怎么提及的 quality attributes，没什么好说的。
  - 11 Quality Attribute Modellingand Analysis 顶级抽象的一章，作业没涉及，逻辑也怪的很，实在不好出笔记。
  - 13 是因为所有的内容基本和 exercise 4 重叠，所以把笔记都放在 exercise 4 里了。
- 4 - 8 的笔记的结构都类似，毕竟都是在讲 quality attributes 的分析：
  - definition 定义
  - General Scenario 通用场景
  - Goal of xxx Tactics 使用 xxx 策略的目的
  - xxx Tactics 某质量要求的策略的具体介绍
