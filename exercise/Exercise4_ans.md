# Exercise 4

- Submit the results of your discussion on Activity 2 as Homework 4
  - Activity 2: See the worksheet for the description of the system and evaluate the architectural design decisions with sensitivity points, trade-off points and the risk points

- Submission:

  - Deadline:   April 21st 

  - Place: submit to Blackboard

## Summary and example in slide

The slide 'evaluating_architecture' tells the basic info of ATAM (Architecture Tradeoff Analysis Method), including phases of the ATAM. However, the further details of phases of the ATAM are mentioned in the slide of exercise 4.

We have done steps 1-5 previously — we created a utility tree. Steps 7-9 are evaluation.

6. Analyze Architectural Approaches
7. Brainstorm and Prioritize Scenarios
8. Analyze Architectural Approaches (performs the same activities as in step 6)

More info about **step 6**: We need to find **risk points, sensitivity points and trade-off points**.

---

Use our ATM system as an example. It uses client - server structure, and the ASRs are modifiability and performance, the following are examples:

Modifiability scenario: A developer wishes to add a new auditing business rule at design time and makes the modification, without affecting other functionality, in 10 person-days.

Performance scenario: The user can withdraw a limit of $300 from an account that has sufficient funds in less than 10 seconds.

So review the knowledge of modifiability and performance, and then **evaluate Three-tier client-server model**.

- Advantages

  - Easy to add clients

  - Servers may be replicated to support scalability and modifiability

- Disadvantages

  - Servers can be a performance bottleneck

  - A single point of failure

So the risk points, sensitivity points and trade-off points can be:

- Sensitivity point
  - Server can be a performance bottleneck and a single point of failure
- Trade-off point
  - Improves scalability and modifiability but decreases performance
- Risk point
  - Architecturally important decisions that have not been made. The architecture team has not decided what **security tactics** they will use. (Another ASR about security!)

## My answer

![Homework_4_materials_figure_5](../pic/Homework_4_materials_figure_5.png)

The chosen ASRs are availability and performance, the following are examples:

Availability scenario: Keep running with no downtime. The ATM network has to be available 24 hours a day.

Performance scenario: The user can withdraw a limit of $300 from an account that has sufficient funds in less than 10 seconds.

Review the knowledge of availability and performance, then evaluate this model that has a **backup database**. 

*In this step, there is no need to concern about the difference between active redundancy (hot spare), spare (cold spare) and passive redundancy (warm spare).*

- Advantages
  - Easy to rollback

- Disadvantages
  - Decreases performance

So the risk points, sensitivity points and trade-off points can be:

- Sensitivity point
  - **AccountDB** can be a performance bottleneck and a single point of failure
- Trade-off point
  - Improves availability, but decreases performance
- Risk point
  - It is important to choose one kind of spare strategies: hot spare, cold spare and warm spare, because the trade-off can only be measured after this choose.

