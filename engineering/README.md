# ENGINEERING
### INDEX

[Proof-of-concept 1: Own your data](#proof-of-concept-1-own-your-data)

[Proof-of-concept 2: Sell your data](#proof-of-concept-2-sell-your-data)

[Tyron's stack](#tyrons-stack)

## Proof-of-Concept 1: _Own your data_
Tyron will leverage self-sovereign identity (```SSI```) to give data sovereignty to their users:  
- **[did:tyron](https://github.com/julioCabDu/didtyron)**: Every time you want to buy from an online shop you have to use an account managed by them and they can store your data for a long time. What if instead of many usernames and passwords, you could use your self-sovereign identity? A digital identity that allows you to manage your privacy by creating different decentralized identifiers (DIDs). For each person/company you communicate with, you could create a unique DID and decide what private information they have access to.
 
```Blockchain``` will be the backbone technology for the peer-to-peer tyron.network, allowing their users to prove who they are without a middleman.  
- **tyron.network**: An eCommerce Sidetree-based network connected to various blockchain platforms. With versatility to support numerous financial providers and countries, focusing on privacy and regulatory compliance. With Tyron, all your data will be encrypted with your secret keys and zero-knowledge proofs.

How you store your data is decisive to claim ownership. Your did:tyron gives you the secret keys to make such claims, but how do you store and manage your data? With your agent.

- **tyron.app**: Your agent, the software that manages your [DIDs](#decentralized-identifiers), [Verifiable Credentials](https://w3c.github.io/vc-data-model/) and communication protocols ([DIDComm](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0005-didcomm)) with other agents. This technology is developed by ```Hyperledger Aries```.

:zap: To contribute to Tyron's proof-of-concept 1 [check this out!](https://github.com/wwwTyron/tyron.network/blob/master/engineering/files/POCs/POC_1.md)

## Proof-of-Concept 2: _Sell your data_
What if you could share your market data for machine learning and influence where resources shall be allocated? Sustainability is key, and Tyron believes that artificial intelligence has to be sustainable as well. Then let's start paying people for their data if they'd like to share it and make some money in return.

_Stay tuned._

## Tyron's stack
Tyron's design implements several cutting-edge technologies, many of them in active development by open source communities.
```
|-----------------------------------------------------------------------------------------------------|
|                                         |--> Hyperledger Aries                                      |
|                                         |            |                                              |
|      Self-Sovereign Identity (SSI)  --->|         GraphQL                                           |
|  with Decentralized Identifiers (DIDs)  |            |                                              |                                      
|                                         |--> Sidetree Protocol (did:tyron)                          |
|                                              |                                                      |
|                                              |                                                      |
|                                              |--> Distributed Ledger Technologies - DLT             |
|                                              |     |  (e.g. Zilliqa, Substrate)                     | 
|                                              |     |                                                |
|                                              |     |--> Smart contracts                             |                                  
|                                              |                                                      |
|                                              |--> Distributed Content-Addressable Storage - DCAS    |
|                                              |        protocol/network (e.g. IPFS)                  |
|                                              |                                                      |
|                                              ^                                                      |
|                                              |<-- libp2p                                            |
|                                              |<-- WebAssembly                                       |
|                                              |<-- Rust and Go                                       |
|-----------------------------------------------------------------------------------------------------|

```
### [Decentralized Identifiers](https://w3c.github.io/did-core/): 
DIDs are a new type of Uniform Resource Locator (URL), that act as web addresses for digital identities anchored in a shared root of trust, such as a distributed ledger. This allows digital identities to interact in a verifiable way without introducing a centralized authority or a single point of failure. Combining distributed ledger technology (DLT) with a decentralized identity management system, you can enable users to create and manage their own identifiers. DIDs are being standardized by the World Wide Web Consortium (W3C).

### [Hyperledger Aries](https://github.com/hyperledger/aries):
Hosted at [The Linux Foundation](https://www.linuxfoundation.org/), the [Hyperledger](https://www.hyperledger.org/) open-source projects focus on enterprise-grade blockchain deployments. Aries provides the cryptographic wallet with a decentralized key management system, as well as the communication protocol for off-chain interaction between blockchain clients.

### [Sidetree Protocol](https://github.com/decentralized-identity/sidetree/blob/master/docs/protocol.md):
Developed by the engineering-driven [Decentralized Identity Foundation](https://identity.foundation/), this protocol is meant to optimize DIDs throughput by batching multiple CRUD operations into one Sidetree transaction. The batch file gets stored in a DCAS (distributed content-addressable storage), an anchor file is created with its metadata, and the hash of the latter anchored on the blockchain. 

### Distributed Ledger Technologies - DLTs
- [Zilliqa](https://zilliqa.com): Born in Singapore, Zilliqa is a blockchain platform that implements sharding for high-performance in scalability. It is also powered by the safe-by-design smart contract language [Scilla](https://www.zilliqa.com/language). Furthermore, Zilliqa allows forkless upgrades.

- [Substrate](https://substrate.dev): It is a blockchain development framework written in Rust and with a runtime image (the chain logic that includes the STF - state transition function) compiled to WebAssembly and stored on-chain, which allows forkless upgrades.

### Distributed Content-Addressable Storage - DCAS
- [InterPlanetary File System (IPFS)](https://github.com/ipfs/ipfs)

### [libp2p](https://libp2p.io): 
A peer-to-peer networking stack modularized out of IPFS. Substrate leverages the [Rust implementation](https://github.com/libp2p/rust-libp2p) of libp2p.

### [WebAssembly (Wasm)](https://webassembly.org):
It is a new type of code, a portable target for compilation of high-level languages like Rust and Go, that can be run with near-native performance in modern web browsers alongside JavaScript. Wasm is being developed as a web standard via the W3C WebAssembly Working Group.

### [Rust](https://www.rust-lang.org):
A very fast and powerful programming language, with a design that is modern and [easy to learn](https://doc.rust-lang.org/book/foreword.html). Rust has a growing open-source community, and for the fourth year in a row, it is the most loved programming language according to the [Developer Survey Results 2019 by Stack Overflow](https://insights.stackoverflow.com/survey/2019).  

### [Go](https://golang.org/)
A programming language focused on concurrency ([Goroutines](https://tour.golang.org/concurrency/1)) and multiprocessing, Go powers cutting-edge open-source software such as [Kubernetes](https://github.com/kubernetes/kubernetes), [IPFS](https://github.com/ipfs/go-ipfs) and [Hyperledger Fabric](https://github.com/hyperledger/fabric).

---

<div style="text-align:center">
 <p><b>Own your data, empower your world.</b></p>
</div>

> <a href="/">Back to homepage</a>
