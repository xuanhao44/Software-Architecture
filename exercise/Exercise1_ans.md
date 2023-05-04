# Exercise 1

- Expand your Utility Tree for the automated teller machine network with at least 6 ASRs:
  - Based on the document given in class and/or based on additional information (internet articles, interviews with the stakeholders)
    - Describe what additional materials you used

- Submission:
  - Deadline:  April 21st
  - Place: submit to Blackboard

## Reference

- For the examples of utility tree please see the textbook as well as the PPT slides from our lecture, we also did a review of utility tree in our exercise class, the example is in these PPR as well.
- The utility tree for this assignment does not need to be complete, you were just asked to have 6 ASRs in your tree.
- First, pick your ASRs – you need to decide by yourself what requirements are important for this system and describe them using the concrete scenario form – the concrete scenario form can be found in our PPT.
- Then organize your ASRs based on quality attributes to build a tree, make sure that there is a root node in your tree and that you assigned priorities (impact on architecture and business value) to your ASRs.
- Below is an example of a utility tree for another system.

![Utility_Tree_Example](../pic/Utility_Tree_Example.png)

## My answer

Utility Tree:

| Quality Attribute | Attribute Refinement                                  | ASR                                                          |
| ----------------- | ----------------------------------------------------- | ------------------------------------------------------------ |
| Performance       | Concurrency in transactions                           | Each bank may be processing transactions from several ATMs at the same time. (H,H) |
|                   | Normal actions after a period of processing time      | If there is no response from the bank computer after a request within 2 minutes the card is reject with an error message. (L,M) |
| Security          | Access denied for unauthorized/unauthencated attempts | The ATM dispenses money if and only if the withdrawal from the account is processed and accepted by the bank. (H,H) |
|                   |                                                       | It must be impossible to plug into the network. (H,H)        |
|                   |                                                       | Only maintainer are allowed to connect new ATM's to the network. (H,H) |
| Availability      | Keep running with no downtime                         | The ATM network has to be available 24 hours a day. (H,H)    |
