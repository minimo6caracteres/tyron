Tyron's design implements several cutting-edge technologies, many of them in active development by the open source community.

### General overview of tyron's stack
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

[Hyperledger Aries](https://github.com/hyperledger/aries)

[Sidetree Protocol](https://github.com/decentralized-identity/sidetree/blob/master/docs/protocol.md)

**[Substrate](https://substrate.dev)**: It is a blockchain development framework written in Rust and with a runtime that compiles to WebAssembly. Substrate leverages [libp2p](https://libp2p.io), a peer-to-peer networking stack modularized out of the [InterPlanetary File System (IPFS)](https://github.com/ipfs/ipfs). Substrate is developed by [Parity Technologies](https://parity.io), the company behind the most popular Ethereum client and founded by Ethereum's co-founder, [Gavin Wood](https://twitter.com/gavofyork).
- -> [Rust](https://www.rust-lang.org): For the fourth year in a row, Rust is the most loved programming language according to the [Developer Survey Results 2019 by Stack Overflow](https://insights.stackoverflow.com/survey/2019). Rust is very fast and powerful, like C++ but for the 21st century. It has a growing open-source community, and its design is modern and [easy to learn](https://doc.rust-lang.org/book/).
- [WebAssembly (Wasm)](https://webassembly.org): 
