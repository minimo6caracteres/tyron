<a href="/">Back to homepage</a>

---

Tyron's design implements several cutting-edge technologies, many of them in active development by open source communities.

## Tyron's stack
```
|------------------------------------------------------------------------------------------------|
|                                        |--> Hyperledger Aries                                  |
|                                        |   ----------------------------------------------------|
|     Self-Sovereign Identity (SSI) ---->|--> Sidetree Protocol                                  |
|                                        |   ----------------------------------------------------|
|                                        |--> Decentralized Identifiers (DIDs)                   |
|------------------------------------------------------------------------------------------------|      
|                                        |--> Off-chain workers                                  |
|                                        |   -------------- ^ -----------------------------------|
| Distributed Ledger Technology (DLT) -->|                  |                   |--> WebAssembly |
|                  &                     |                  |                   |   -------------|
|           Smart contracts ------------>|--> Substrate blockchain framework -->|--> Rust        |
|                                                                               |   -------------|
|                                                                               |--> libp2p      |
|------------------------------------------------------------------------------------------------|

```
- [Hyperledger Aries](https://github.com/hyperledger/aries): Hosted at [The Linux Foundation](https://www.linuxfoundation.org/), the [Hyperledger](https://www.hyperledger.org/) open source projects focus on enterprise-grade blockchain deployments. 

---

- [Sidetree Protocol](https://github.com/decentralized-identity/sidetree/blob/master/docs/protocol.md): Developed by the engineering-driven [Decentralized Identity Foundation](https://identity.foundation/), this protocol is meant to optimize DIDs throughput by batching multiple CRUD operations into one Sidetree transaction. The batch file gets stored in a DCAS (distributed content-addressable storage), an anchor file is created with its metadata, and the hash of the latter anchored on the blockchain. 

---

- [Decentralized Identifiers](https://w3c.github.io/did-core/): DIDs are a new type of Uniform Resource Locator (URL), that act as web addresses for digital identities anchored in a shared root of trust, such as a distributed ledger. This allows digital identities to interact in a verifiable way without introducing a centralized authority or a single point of failure. Tyron combines distributed ledger technology (DLT) with a decentralized identity management system to enable their users to create and manage their own identifiers. DIDs are being standardized by the World Wide Web Consortium (W3C).

---

- [Substrate](https://substrate.dev): It is a blockchain development framework written in Rust and with a runtime image (the chain logic that includes the STF - state transition function) compiled with WebAssembly and stored on-chain. This allows **forkless upgrades**, a significant advantage compared to other blockchain platforms. Substrate leverages the [Rust implementation](https://github.com/libp2p/rust-libp2p) of [libp2p](https://libp2p.io), a peer-to-peer networking stack modularized out of the [InterPlanetary File System (IPFS)](https://github.com/ipfs/ipfs). Substrate is developed by [Parity Technologies](https://parity.io), the company behind the most popular Ethereum client and founded by Ethereum's co-founder, [Gavin Wood](https://twitter.com/gavofyork). Furthermore, Substrate provides support for **light clients** and **off-chain workers**.

---

- [Rust](https://www.rust-lang.org): For the fourth year in a row, Rust is the most loved programming language according to the [Developer Survey Results 2019 by Stack Overflow](https://insights.stackoverflow.com/survey/2019). Rust is very fast and powerful, like C++ but for the 21st century. It has a growing open-source community, and its design is modern and [easy to learn](https://doc.rust-lang.org/book/foreword.html).
  
---

- [WebAssembly (Wasm)](https://webassembly.org): It is a new type of code, a portable target for compilation of high-level languages like Rust, that can be run with near-native performance in modern web browsers alongside JavaScript. Wasm is being developed as a web standard via the W3C WebAssembly Working Group.

---

<a href="/">Back to homepage</a>

To contribute with tyron's POC1 [check this out](/engineering/poc1.md
