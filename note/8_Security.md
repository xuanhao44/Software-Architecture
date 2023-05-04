# 8 Security

## definition

安全性的定义尤其重要，内容也比较多。

- **Security** is a measure of the system’s ability to protect data and information from unauthorized access while still providing access to people and systems that are authorized

  **安全性**是系统保护数据和信息不受未经授权访问的能力的度量，同时仍然提供对授权人员和系统的访问。

- An action taken against a computer system with the intention of doing harm is called an **attack**

  对计算机系统采取的意图造成损害的行为称为攻击

- Attack can be in different forms 攻击可以有不同的形式

  - unauthorized attempt to access/modify data or service

    未经授权访问/修改数据或服务的企图

  - intended to deny services to legitimate users

    拒绝向合法用户提供服务

---

区分 safety 和 security（内容来自 9 Other quality attributes）

safety 是指保护人们免受意外伤害，而 security 是指保护人们免受有意的威胁。例如，safety 问题是由意外造成，如疏忽、事故、环境、外界因素等，而 security 问题是由有意的人为因素造成，例如偷窃、间谍、抢劫、入侵等造成。

---

Security has three main characteristics, called CIA:

- **Confidentiality** is the property that data or services are protected from unauthorized access.

  **保密性**是保护数据或服务免受未经授权访问的属性。

  - For example, a hacker cannot access your income tax returns on a government computer.

    例如，黑客无法访问政府计算机上的个人所得税申报表。

- **Integrity** is the property that data or services are not subject to unauthorized manipulation.

  **完整性**是指数据或服务不受未经授权的操纵的属性。

  - For example, your grade has not been changed since your instructor assigned it.

    例如，你的分数从你的老师分配到现在就没有改变过。

- **Availability** is the property that the system will be available for legitimate use.

  **可用性**是系统可以合法使用的属性。

  - For example, a denial-of-service attack prevent you from ordering a book from an online bookstore.

    例如，拒绝服务攻击阻止您从在线书店订购图书。

Other characteristics that support CIA are

- **Authentication** verifies the identities of the parties to a transaction and checks if they are truly who they claim to be.

  **身份验证**验证交易双方的身份，并检查他们是否真的是他们所声称的那个人。

- **Authorization** grants a user the privileges to perform a task.

  **授权**授予用户执行任务的权限。

- **Nonrepudiation** guarantees that the sender/recipient of a message cannot later deny having sent/received the message.

   **不可抵赖性**保证消息的发送者/接收者以后不能否认曾经发送/接收过该消息。

## Security General Scenario

| Portion of Scenario              | Possible Values                                              |
| -------------------------------- | ------------------------------------------------------------ |
| Source                           | Human or another system which may have been previously identified (either correctly or incorrectly) or may be currently unknown. A human attacker may be from outside the organization or from inside the organization. |
| 刺激来源                         | 人类或其他系统，可能已经确定（正确或错误）或可能目前未知。人类攻击者可能来自组织外部，也可能来自组织内部。 |
| Stimulus                         | **Unauthorized attempt** is made to display data, change or delete data, access system services, change the system’s behavior, or reduce availability. |
| 刺激                             | **未经授权的尝试**显示数据、更改或删除数据、访问系统服务、更改系统行为或降低可用性。 |
| Artifact                         | System services; data within the system; a component or resources of the system; data produced or consumed by the system. |
| （因刺激运作起来的系统中的）工件 | 系统服务；系统内数据；系统的组成部分或资源；系统产生或使用的数据。 |
| Environment                      | The system is either online or offline, connected to or disconnected from a network, behind a firewall or open to a network, fully operational, partially operational, or not operational. |
| 环境                             | 系统在线或离线，连接或断开网络，位于防火墙后或向网络开放，完全运行，部分运行或不运行。 |
| Response                         | Transactions are carried out in a fashion such that<br/>- data or services are protected from unauthorized access;<br/>- data or services are not being manipulated without authorization;<br/>- parties to a transaction are identified with assurance;<br/>- the parties to the transaction cannot repudiate their involvements;<br/>- the data, resources, and system services will be available for legitimate use.<br/>The system tracks activities within it by<br/>- recording access or modification,<br/>- recording attempts to access data, resources or services,<br/>- notifying appropriate entities when an apparent attack is occurring. |
| 响应                             | 事务以下述方式进行：<br/>- 数据或服务不受未经授权的访问；<br/>- 数据或服务不受未经授权的操纵；<br/>- 交易各方得到保证的识别；<br/>- 交易各方不能否认他们的参与；<br/>- 数据、资源和系统服务将可用于合法使用。<br/ >系统通过以下方式跟踪其中的活动：<br/>- 记录访问或修改，<br/>- 记录访问数据、资源或服务的尝试，<br/>- 在明显的攻击发生时通知适当的实体。 |
| Response Measure                 | One or more of the following:<br/>- how much of a system is compromised when a particular component or data value is compromised,<br/>- how much time passed before an attack was detected,<br/>- how many attacks were resisted,<br/>- how long does it take to recover from a successful attack,<br/>- how much data is vulnerable to a particular attack |
| 响应的度量                       | 以下一个或多个：<br/>- 当一个特定的组件或数据值被破坏时，有多少系统被破坏，<br/>- 在检测到攻击之前经过了多长时间，<br/>- 抵抗了多少次攻击，<br/>- 从成功的攻击中恢复需要多长时间，<br/>- 有多少数据容易受到特定攻击 |

## Sample Concrete Security Scenario

- A disgruntled employee from a remote location attempts to modify the pay rate table during normal operations. The system maintains an audit trail and the correct data is restored within a day.

  一个心怀不满的员工从远程位置试图在正常操作期间修改工资率表。系统保持审计跟踪，在一天内恢复正确的数据。

  - Stimulus: unauthorized attempts to modify the pay rate table
  - Stimulus source: a disgruntled employee
  - Artifact: the system with pay rate table
  - Environment: during normal operation
  - Response: maintains an audit trail
  - Response measure: correct data is restored within a day

## Goal of Security Tactics

PPT 里居然没有，震惊。

## Security Tactics

![Security Tactics](../pic/Security_Tactics.png)

### Detect Attacks 检测攻击

- **Detect Intrusion**: **compare network traffic or service request patterns** within a system to a set of signatures or known patterns of malicious behavior stored in a database.

  **检测入侵**：**比较系统内的网络流量或服务请求模式**与存储在数据库中的一组签名或已知恶意行为模式。

- **Detect Service Denial**: **comparison of the pattern or signature of network traffic** *coming* *into* a system to historic profiles of known Denial of Service (DoS) attacks.

  **检测拒绝服务**：**比较进入**系统的网络流量的模式或特征与已知拒绝服务 (DoS) 攻击的历史概况。

- **Verify Message Integrity**: use techniques such as ***checksums*** or ***hash values*** to verify the integrity of messages, resource files, deployment files, and configuration files.

  **验证消息完整性**：使用 ***校验和*** 或 ***哈希值*** 等技术验证消息、资源文件、部署文件、配置文件的完整性。

- **Detect Message Delay**: checking the time that it takes to deliver a message, it is possible to detect suspicious timing behavior, i.e., man-in-the-middle attack.

  **检测消息延迟**：检查发送消息所需的时间，可以检测到可疑的定时行为，即中间人攻击。

### Resist Attacks 抵抗攻击

- **Identify Actors**: identify the source of any external input to the system.

  **识别参与者**：识别系统的任何外部输入的来源。

- **Authenticate Actors**: ensure that a user or remote computer is actually who or what it purports to be.

  **认证参与者**：确保用户或远程计算机实际上是谁或它声称是什么。

- **Authorize Actors**: ensuring that an authenticated actor has the rights to access and modify either data or services.

  **授权参与者**：确保经过认证的参与者有权访问和修改数据或服务。

- **Limit Access**: limiting access to resources such as memory, network connections, or access points.

  **限制访问**：限制对内存、网络连接或接入点等资源的访问。

- **Limit Exposure**: minimize the attack surface of a system by having the **fewest possible number of access points**.

  **限制暴露**：通过**尽可能少的接入点**，最大限度地减少系统的攻击面。

  - E.g., firewall is a single point of access to the intranet 防火墙是内网的单一访问点
  - E.g., closing a port 关闭一个端口

- **Encrypt Data**: apply some form of encryption to data and to communication.

  **加密数据**：对数据和通信应用某种形式的加密。

- **Separate Entities**: can be done through physical separation on different servers, the use of virtual machines.

  **分离实体**：可以通过物理分离在不同的服务器上完成，使用虚拟机。

- **Change Default Settings**: Force the user to change settings assigned by default.

  **更改默认设置**：强制用户更改默认分配的设置。

### React to Attacks 应对攻击

- **Revoke Access**: limit access to sensitive resources, even for normally legitimate users and uses, if an attack is suspected.

  **撤销访问**：当怀疑受到攻击时，限制敏感资源的访问权限，即使是正常合法的用户和用途也不例外。

- **Lock Computer**: limit access to a resource if there are repeated failed attempts to access it.

  **锁定计算机**：限制访问资源，如果有多次失败的尝试访问它。

- **Inform Actors**: notify operators, other personnel, or cooperating systems when an attack is suspected or detected.

  **通知相关人员**：当怀疑或检测到攻击时，通知运营商、其他人员或合作系统。
