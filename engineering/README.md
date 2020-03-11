Tyron's design implements several cutting-edge technologies, many of them in active development by the open source community.

### General overview of tyron's stack
```
|----------------------------------------------------------------------------------------|
|                                     |-> Hyperledger Aries                              |
|                                     |  ------------------------------------------------|
|    Self-Sovereign Identity (SSI)    |-> Sidetree Protocol                              |
|                                     |  ------------------------------------------------|
|                                     |-> Decentralized Identifiers (DIDs)               |
|----------------------------------------------------------------------------------------|      
|                                     |-> Off-chain workers                              |
|                                     |  -------------- ^ -------------------------------|
| Distributed Ledger Technology (DLT) |                 |                |-> WebAssembly |
|                                     |                 |                |  -------------|
|                                     |-> Substrate blockchain framework |-> Rust        |
|                                                                        |  -------------|
|                                                                        |-> libp2p      |
|----------------------------------------------------------------------------------------|

```

[Hyperledger Aries](https://github.com/hyperledger/aries)|
[Sidetree Protocol](https://github.com/decentralized-identity/sidetree/blob/master/docs/protocol.md)
[Substrate](https://substrate.dev)
