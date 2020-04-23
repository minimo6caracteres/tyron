# Tyron's proof-of-concept 1: "Own your data" - POC_1
Let's explore the key features, their feasibility and the overall functionality of tyron's POC_1.

 - Product: Open-source eCommerce app for peer-to-peer private transactions where the user owns their data. 
 - Purpose: To give people the ownership of their data.
 
## Product features
 List of key features:  
 [1. Self-sovereign identity (SSI)](#1-self-sovereign-identity-ssi)  
 [2. Blockchain, distributed ledger technology (DLT)](#2-blockchain-distributed-ledger-technology-dlt)  
 [3. Rust & Web-Assembly](#3-rust--webassembly)

Any ideas? Feel free to add them below and send a pull request. 
> [Contributing guideline](https://github.com/tyronNetwork/tyron/blob/master/CONTRIBUTING.md)  
[Code of conduct](https://github.com/tyronNetwork/tyron/blob/master/CODE_OF_CONDUCT.md).

| Issue | Description | Idea or question | Username |
|---|---|---|---|

### 1. Self-sovereign identity (SSI)
There are several protocols, standards and specifications developing how digital identity can be independent of any centralized trust system - like the government or your bank - but using instead a ledger distributed among many organizations. Then that computer system becomes independent of any single party and is tamper-resistant. Decentralized identifiers (DIDs) are anchored in such a system, and there are several [implementations](https://w3c-ccg.github.io/did-method-registry/#the-registry) of this new type of URL.

Tyron could have its own DID method specification in compliance with [W3C's specification](https://w3c.github.io/did-core/). There are other interesting method specifications such as:
- [Sovrin DID](https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html)
- [Peer DID](https://openssi.github.io/peer-did-method-spec/index.html)
- [IPID: Interplanetary Identifiers DID](https://did-ipid.github.io/ipid-did-method/)
- [KILT DID](https://github.com/KILTprotocol/kilt-did-driver/blob/master/DID%20Method%20Specification.md)

### 2. Blockchain, distributed ledger technology (DLT)
[Bitcoin](https://bitcoin.org/bitcoin.pdf) changed the world, and it's an inspiration in terms of community and decentralization. Proof-of-work, however, is not sustainable for tyron.

The tyron.network will be built with blockchain technology as a decentralized system that is:
- Permissioned: Organizations would have to go through legal compliance to become tyron nodes operators. 
- Proof-of-stake: Network validators would have to stake assets to secure the system.

The DLT chosen for tyron is [Substrate](https://substrate.dev/) given its use of Rust and WebAssembly. Furthermore, Substrate implements [libp2p](https://libp2p.io/) in Rust, off-chain workers and smart contracts in Wasm.

### 3. Rust & WebAssembly
