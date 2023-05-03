# Exercise 1

- Expand your Utility Tree for the automated teller machine network with at least 6 ASRs:
  - Based on the document given in class and/or based on additional information (internet articles, interviews with the stakeholders)
    - Describe what additional materials you used

![Utility_Tree_Example](../pic/Utility_Tree_Example.png)

- Submission:
  - Deadline:  April 21st
  - Place: submit to Blackboard

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
