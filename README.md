# rust-counter-near

This is the counter example and how we built it in NEAR using Rust.
This repo is applYing the tutorial called [**Building a Smart Contract in Rust**](https://docs.near.org/docs/develop/contracts/rust/intro#installing-the-rust-toolchain) from NEAR documentation.

### Prerequisites

- Rust toolchain
- A NEAR account
- NEAR command-line interface (near-cli)

### How to Use

- clone the repo
- run `cargo build`
- run `cargo build --target wasm32-unknown-unknown --release`
- login to your account using `near login`
- delpoy the contract using:
  `near deploy --wasmFile target/wasm32-unknown-unknown/release/rust_counter_tutorial.wasm --accountId YOUR_ACCOUNT_HERE`

### Contract Available Methods:

- increment

```
near call YOUR_ACCOUNT_HERE  increment --accountId YOUR_ACCOUNT_HERE

```

- decrement:

```
near call YOUR_ACCOUNT_HERE  decrement --accountId YOUR_ACCOUNT_HERE

```

- get_num : get the counter value

```
near call YOUR_ACCOUNT_HERE  get_num  --accountId YOUR_ACCOUNT_HERE
```

- reset

```
near call YOUR_ACCOUNT_HERE  reset --accountId YOUR_ACCOUNT_HERE

```
