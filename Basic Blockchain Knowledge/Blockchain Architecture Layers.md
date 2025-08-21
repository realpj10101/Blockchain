
When discussing **blockchain architecture**, we refer to the components, layers, and overall technology that comprise a complete blockchain system. Each layer has a unique role, from storing data to maintaining network connectivity and ensuring consensus across the system.

Understanding how these layers work together to make up a system is crucial for blockchain, **smart contract developers**, and anyone seeking to leverage **blockchain technology** effectively.

In this article, we’ve broken down the intricacies of **blockchain architectures into easy-to-understand pieces**. We’ll explain what is the scalability trilemma, what blockchain functional layers are and how they work together to form the architecture of the layer 1,2, and 3 chains we’ve heard about.

Before getting into the different parts making up a complete blockchain architecture, it is important to understand the issues that all of these components try to solve: **making the blockchain scalable.**

##  What is blockchain scalability?

The term "**scaling**" in blockchain technology means improving the system's (chain) capacity for processing transactions, typically measured in **transactions per second** or **TPS**, a key metric that defines the ability of a payment system to serve, or not, a **considerable number of users**.

This isn’t a new metric for payment systems - **Visa**, for example, a traditional payment system, can handle more than **65,000 TPS**. On the other hand, **Bitcoin** has a TPS (transactions per second) **processing power of only 4 to 7**. This makes chains need to scale and improve their ability to serve more users (transactions per second).

The reality is that scaling a chain isn’t as simple as it sounds. There’s in fact one issue - called the **Blockchain Scalability Trilemma**

## The blockchain Scalability Trilemma

• **Decentralization**

**‍**• **Security**

**‍**• **Scalability**

[[trilemma.png]]

‍The thesis of this trilemma is that a blockchain **can only achieve two of these three goals** simultaneously.

The trilemma suggests that making a blockchain highly scalable and secure might require some degree of centralization. If you want it to be highly decentralized and secure, it might struggle with scalability, as each node in the network might have, for example, to validate every transactions, which can slow down processing times and increase costs.

To solve this problem, clever developers have decided to take blockchains like **Ethereum** or **Bitcoin** and instead of trying to create a single chain that is both scalable, secure, and decentralized, they would make two chains:

- **Layer** **1** (Ethereum, Bitcoin):  to focus on fundamental changes in blockchains at their core
- **Layer 2** (zkSync, LightingNetwork): to add additional structures on top of layer 1 to enhance performance without compromising the blockchain's core functionality. For example, if a layer one blockchain focuses on security and decentralization, it can be the job of an L2 to focus on scale.

Before getting too in-depth into **what Layer 1 and Layer 2 blockchains are**, let’s understand what we mean when we refer to the term “layer” in the context of blockchain architectures.

‍

