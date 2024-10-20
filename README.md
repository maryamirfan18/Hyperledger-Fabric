# Hyperledger-Fabric
## Introduction
A blockchain is essentially an immutable ledger of transactions maintained across a distributed network of *peer nodes*. Each node in the network holds a copy of the ledger and updates it by applying transactions that have been validated through a consensus mechanism. These transactions are grouped into blocks, each containing a cryptographic hash linking it to the previous block, ensuring data integrity.<br/>

The first widely known application of blockchain technology was Bitcoin, a cryptocurrency. Ethereum, another prominent cryptocurrency, introduced a similar concept but extended it by incorporating smart contracts, enabling the development of decentralized applications (dApps). Both Bitcoin and Ethereum represent **public, permissionless blockchains**, where anyone can join the network, and participants remain anonymous.<br/>

As Bitcoin, Ethereum, and related technologies gained traction, interest grew in applying blockchain principles to innovative enterprise solutions. However, many business use cases demand features that public blockchains currently cannot provide. For instance, enterprise applications often require participant identity verification, as seen in financial transactions governed by Know-Your-Customer (KYC) and Anti-Money Laundering (AML) regulations.

Enterprise blockchain solutions must address specific requirements, including:<br/>
- **Identifiable participants** to meet regulatory and business needs.<br/>
- **Permissioned networks** to control access.<br/>
- **High transaction throughput** to handle large-scale operations.<br/>
- **Low latency** for faster transaction confirmation.<br/>
- **Privacy and confidentiality** for sensitive business data.<br/>

Although some public blockchain platforms are being adapted for enterprise use, **Hyperledger Fabric** was purpose-built with business applications in mind. The following sections highlight the distinct features of Hyperledger Fabric and explore the architectural choices that set it apart from other blockchain platforms.



# Hyperledger Fabric
Hyperledger Fabric is an open source enterprise-grade permissioned distributed ledger technology (DLT) platform, designed for use in enterprise contexts, that delivers some key differentiating capabilities over other popular distributed ledger or blockchain platforms.<br/>
One key point of differentiation is that Hyperledger was established under the Linux Foundation, which itself has a long and very successful history of nurturing open source projects under open governance that grow strong sustaining communities and thriving ecosystems. <br/>Hyperledger is governed by a diverse technical steering committee, and the Hyperledger Fabric project by a diverse set of maintainers from multiple organizations. It has a development community that has grown to over 35 organizations and nearly 200 developers since its earliest commits.<br/>
Fabric has a highly modular and configurable architecture, enabling innovation, versatility and optimization for a broad range of industry use cases including banking, finance, insurance, healthcare, human resources, supply chain and even digital music delivery.<br/>
Fabric is the first distributed ledger platform to support smart contracts authored in general-purpose programming languages such as Java, Go and Node.js, rather than constrained domain-specific languages (DSL). This means that most enterprises already have the skill set needed to develop smart contracts, and no additional training to learn a new language or DSL is needed.<br/>
The Fabric platform is also permissioned, meaning that, unlike with a public permissionless network, the participants are known to each other, rather than anonymous and therefore fully untrusted. This means that while the participants may not fully trust one another (they may, for example, be competitors in the same industry), a network can be operated under a governance model that is built off of what trust does exist between participants, such as a legal agreement or framework for handling disputes.<br/>
One of the most important of the platform’s differentiators is its support for pluggable consensus protocols that enable the platform to be more effectively customized to fit particular use cases and trust models. For instance, when deployed within a single enterprise, or operated by a trusted authority, fully byzantine fault tolerant consensus might be considered unnecessary and an excessive drag on performance and throughput. In situations such as that, a crash fault-tolerant (CFT) consensus protocol might be more than adequate whereas, in a multi-party, decentralized use case, a more traditional byzantine fault tolerant (BFT) consensus protocol might be required.
Fabric can leverage consensus protocols that do not require a native cryptocurrency to incent costly mining or to fuel smart contract execution. Avoidance of a cryptocurrency reduces some significant risk/attack vectors, and absence of cryptographic mining operations means that the platform can be deployed with roughly the same operational cost as any other distributed system.<br/>
The combination of these differentiating design features makes Fabric one of the better performing platforms available today both in terms of transaction processing and transaction confirmation latency, and it enables privacy and confidentiality of transactions and the smart contracts (what Fabric calls “chaincode”) that implement them.

