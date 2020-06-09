Let's explore some key features, their feasibility and overall functionality.

# List of key features:  
 [1. Self-sovereign identity (SSI)](#1-self-sovereign-identity-ssi)  
 [2. Blockchain, distributed ledger technology (DLT)](#2-blockchain-distributed-ledger-technology-dlt)  
 [3. Rust & Web-Assembly](#3-rust--webassembly)

## 1. Self-sovereign identity (SSI)
There are several protocols, standards and specifications developing how digital identity can be independent of any centralized trust system - like the government or your bank - but using instead a ledger distributed among many organizations. Then that computer system becomes independent of any single party and is tamper-resistant. Decentralized identifiers (DIDs) are anchored in such a system, and there are several [implementations](https://w3c-ccg.github.io/did-method-registry/#the-registry) of this new type of URL.

Interesting DID method specifications in compliance with [W3C's specification](https://w3c.github.io/did-core/):
- [Sovrin DID](https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html)
- [Peer DID](https://openssi.github.io/peer-did-method-spec/index.html)
- [IPID: Interplanetary Identifiers DID](https://did-ipid.github.io/ipid-did-method/)
- [KILT DID](https://github.com/KILTprotocol/kilt-did-driver/blob/master/DID%20Method%20Specification.md)

## 2. Blockchain, distributed ledger technology (DLT)
[Bitcoin](https://bitcoin.org/bitcoin.pdf) changed the world, and it's an inspiration in terms of community and decentralization.

### DLT [Substrate](https://substrate.dev/): built with Rust and WebAssembly.
Substrate is a blockchain development framework that you can use to create an independent chain that can also easily connect to other Substrate-based chains, which allows blockchain interoperability. Moreover, Substrate implements [libp2p](https://libp2p.io/) in Rust, off-chain workers and smart contracts in Wasm.

## 3. Rust & WebAssembly
[Rust](https://www.rust-lang.org/) is a powerful programming language, and its advanced trait system makes blockchain even more powerful. And you can compile software written in Rust to the new and super fast WebAssembly (Wasm).  
The cool thing about [Wasm](https://webassembly.org/) is that you can run it in the browser, which opens up new opportunities for blockchain development. 

> To name a few, Wasm powers light clients, allows forkless updates and takes smart contracts to the next level. 

Both Rust and WebAsembly are open-source software supported by large communities and corporations like Microsoft, Mozilla, AWS, Google and Apple.

Parity Technologies develops Substrate, and there are other blockchain networks written in Rust such as [Libra](https://github.com/libra/libra). 
