# ethers-events-derive

Having some issues importing derive macros from ethers-rs 

The test is lib.rs, replicating the below test from ethers-contract: 

https://github.com/gakonst/ethers-rs/blob/master/ethers-contract/tests/common/derive.rs

In ethers-contract/src/lib the derive macros are under the abigen feature which is included in cargo.toml
```
#[cfg(feature = "abigen")]
#[cfg_attr(docsrs, doc(cfg(feature = "abigen")))]
pub use ethers_contract_derive::{abigen, EthAbiType, EthEvent};
```

Main error
`error[E0433]: failed to resolve: use of undeclared crate or module ethers_core`

