# Bitcoin Transaction Utils 
> Utilities for bitcoin transactions 

---

**⚠️ This is experimental. Please use at your own risk.⚠️**

---

## Install
> Add package to Cargo.toml file
```rust
[dependencies]
bitcoin-transaction-utils= "0.1.0"
```

## Usage:
```rust
use bitcoin_transaction_utils::{
  is_transaction_hex_segwit,
}
let segwit_transaction_hex = "020000000001017fc0bfbe2b2e06e33723bec965db6f99edfcfdf0eb17a70b3bd4f708a02052830100000000ffffffff02a078aa000000000017a9144417c11f4b80a25b559e56df5daf9e715eaa27228721732301000000001600140f410abac0a0de8320891834565410bb010cda2602483045022100fe4b42cfc8390a00c1eb32da5ce2805f0321cdb0f2404210e94120fd6e48a55002204bee731f2f9fc0b2449266664669c7f99eb832b65c006fc8bcb5bc33b5a971d00121020b6ce55fabe6456bda581678a78276ce8c0c8a4799ada99f835342263d2e2d9100000000".to_string();

let non_segwit_transaction_hex = "0100000001f5bf38188b302dc80f5b0f979a924736dd6a48f95931c51e7182c75229957ccd000000006b483045022100ea408778a04d6c3d23c5184631b811d484480c7259e37c1ef5c29dbf1e05749d022038ac87e2327aa82e8fa5dc7c4d63fd70cd4b8eee2a7222fcc31151e4c935985f01210369e03e2c91f0badec46c9c903d9e9edae67c167b9ef9b550356ee791c9a40896ffffffff02d2b6f601000000001976a9149f21a07a0c7c3cf65a51f586051395762267cdaf88ac48720900000000001976a9145ac4968f9d4061da0023e6e204e22a1a2182820488ac00000000".to_string();

is_transaction_hex_segwit(&segwit_transaction_hex) // => true
is_transaction_hex_segwit(&non_segwit_transaction_hex) // => false
```


## Related
- [bitcoin-address](https://github.com/joegesualdo/bitcoin-address) - Utilities for Bitcoin addresses
- [bitcoid-request](https://github.com/joegesualdo/bitcoind-request) - Request Bitcoin blockchain data from a node
- [bitcoin-node-query](https://github.com/joegesualdo/bitcoin-node-query) - Query Bitcoin Node for information
- [bitcoin-terminal-dashboard](https://github.com/joegesualdo/bitcoin-terminal-dashboard) - Bitcoin Dashboard in the terminal

## License
MIT © [Joe Gesualdo]()
 

