[Back to the homepage](/tyron)

Tyron's design implements several cutting-edge technologies, many of them in active development by the open source community.

## General overview of tyron's stack
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
- [Hyperledger Aries](https://github.com/hyperledger/aries)

- [Sidetree Protocol](https://github.com/decentralized-identity/sidetree/blob/master/docs/protocol.md)

- [Decentralized Identifiers](https://www.w3.org/TR/did-core/): DIDs are a new type of Uniform Resource Locator (URL), that act as web addresses for digital identities anchored in a shared root of trust, such as a distributed ledger. This allows digital identities to interact in a verifiable way without introducing a centralized authority or a single point of failure. Tyron combines distributed ledger technology (DLT) with a decentralized identity management system to enable their users to create and manage their own identifiers. DIDs are being standardized by the World Wide Web Consortium (W3C).

- [Substrate](https://substrate.dev): It is a blockchain development framework written in Rust and with a runtime image (the chain logic that includes the STF - state transition function) compiled with WebAssembly and stored on-chain. This allows **forkless upgrades**, a significant advantage compared to other blockchain platforms. Substrate leverages the [Rust implementation](https://github.com/libp2p/rust-libp2p) of [libp2p](https://libp2p.io), a peer-to-peer networking stack modularized out of the [InterPlanetary File System (IPFS)](https://github.com/ipfs/ipfs). Substrate is developed by [Parity Technologies](https://parity.io), the company behind the most popular Ethereum client and founded by Ethereum's co-founder, [Gavin Wood](https://twitter.com/gavofyork). Furthermore, Substrate provides support for **light clients** and **off-chain workers**.
  - [Rust](https://www.rust-lang.org): For the fourth year in a row, Rust is the most loved programming language according to the [Developer Survey Results 2019 by Stack Overflow](https://insights.stackoverflow.com/survey/2019). Rust is very fast and powerful, like C++ but for the 21st century. It has a growing open-source community, and its design is modern and [easy to learn](https://doc.rust-lang.org/book/).
  - [WebAssembly (Wasm)](https://webassembly.org): It is a new type of code, a portable target for compilation of high-level languages like Rust, that can be run with near-native performance in modern web browsers alongside JavaScript. Wasm is being developed as a web standard via the W3C WebAssembly Working Group.
  
[Back to the homepage](/README.md)
