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
