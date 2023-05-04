# 12 ASR (Architecturally Significant Requirement)

这一部分的内容来自于书中第三部分 生命周期中的架构的第 16 和 17 讲，但是 PPT 的标题却仅用 16 讲的主题作为标题，很有误导性。

## ASR

ASR 的来源主要是各个利益相关者和商业目标的。这一部分最重要的两个内容是 QAW 和 Utility tree。

### QAW (Quality Attribute Workshop)

要点是：针对各个 stakeholder，细化场景 (Quality Attribute Scenarios)，且确立优先级。

*感觉这个 Part 没在作业中出现。*

---

QAW Steps:

1. QAW Presentation and Introductions. QAW 演示和介绍。

   - QAW facilitators describe the **motivation** for the QAW and explain **each step** of the QAW.

     质量保证原则促进者描述质量保证原则的动机，并解释质量保证原则的每个步骤。

2. Business/Mission Presentation. 业务/任务展示。

   - The stakeholder representing the business concerns presents the **system’s business context**, broad **functional requirements**, **constraints**, and **known quality attribute requirements**.

     代表着业务关注点的利益相关者展示**系统的业务环境**、广泛的**功能需求**、**约束**和**已知的质量属性需求**。

   - The quality attributes will be derived largely from the business/mission needs.

     质量属性将主要来源于业务/任务需求。

3. Architectural Plan Presentation. 架构设计方案展示。

   - The architect will present the **system architectural plans**.

     架构师将提交**系统架构方案**。

   - This lets stakeholders know the current architectural thinking.

     这让利益相关者了解当前的架构思维。

4. Identification of Architectural Drivers. 识别架构驱动因素。

   - The facilitators will share **their list of key architectural drivers** assembled during Steps 2 and 3,

     引导者将分享他们在步骤 2 和 3 中组装的关键架构驱动程序列表，

   - **Architectural drivers** includes overall requirements, business drivers, constraints, and quality attributes.

     **架构驱动**包括总体需求、业务驱动、约束和质量属性。

   - ask the stakeholders for clarifications, additions, deletions, and corrections, and **achieve a consensus** on the architectural drivers.

     要求利益相关者澄清、添加、删除和更正，并就架构驱动达成共识。

5. Scenario Brainstorming. 场景的头脑风暴。

   - Each stakeholder expresses a scenario representing his or her concerns with respect to the system.

     每个利益相关者表达一个场景，代表他或她对系统的关注。

   - Facilitators ensure that each scenario has an explicit stimulus and response.

     促进者确保每个场景都有明确的刺激和反应。

   - Make at least **one representative scenario** for each architectural driver listed in Step 4.

     为步骤 4 中列出的每个架构驱动程序制作至少一个代表性场景。

6. Scenario Consolidation. 场景整合。

   - Similar scenarios are consolidated where reasonable.

     合理合并类似场景。

7. Scenario Prioritization. 场景优先级。

   - Allocating each stakeholder a number of votes equal to 30 percent of the total number of scenarios.

     为每个利益相关者分配相当于场景总数 30% 的选票。

   - Each stakeholder allocate their votes to scenario.

     每个利益相关者分配他们对场景的投票。

8. Scenario Refinement. 场景细化。

   - The top scenarios are refined and elaborated.

     对顶级场景进行细化和阐述。

   - Facilitators help the stakeholders put the scenarios in the six-part scenario form.

     引导者帮助利益相关者将场景以六部分场景的形式呈现。

### Utility tree

- An ASR must have the following characteristics:

  - *A profound impact on the architecture*

    Including this requirement will very likely result in a different architecture than if it were not included.

  - *A high business or mission value*

    If the architecture is going to satisfy this requirement it must be of high value to important stakeholders.

---

- A way to **record ASRs all in one place**.

- Establishes priority of each ASR in terms of

  - Impact on architecture

  - Business or mission value

- **ASRs are captured as scenarios**.

- Draw

  - Root of tree is placeholder node called “Utility”.

  - Second level of tree contains broad QA categories.

  - Third level of tree refines those categories.

  - **Leaf nodes are the concrete quality attribute scenarios**.

- Utility Tree Example (节选)

![Utility_Tree_Example](../pic/Utility_Tree_Example.png)

- Next Steps:
  - ASRs that rate a (H,H) rating are the ones that deserve the most attention. *左边的是对架构的重要程度，右边的是对商业目标（价值）的重要程度。*
  - **A very large number of these might be a cause for concern: Is the system achievable?*
  - Stakeholders can review the utility tree to make sure their concerns are addressed.

---

关于作业：[作业 1](../exercise/Exercise1_ans.md) 就是画一个效用树。具体的画的过程和作业写在一起了。可以看到画 Utility Tree 的最后也把 ASR 画出了，算是一举两得。

## The Steps of Add

重点是分解 (Decomposition)，一次处理一个部分和迭代。

1. **Choose an element** of the system to design.
2. **Identify the ASRs** for the chosen element.
3. **Generate a design solution** for the chosen element.
4. **Inventory remaining requirements** and select the input for the next iteration.
5. Repeat steps 1–4 until all the ASRs have been satisfied.

---

关于作业：[作业 2](../exercise/Exercise2_ans.md) 就是画一个 ADD 的过程。
