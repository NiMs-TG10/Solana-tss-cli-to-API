Solana TSS Wallet API
A RESTful API for managing a Solana Threshold Signature Scheme (TSS) wallet, built with Rust and the Poem framework. Converted from a CLI to simplify interaction, with fixed crate versions for stability. Supports key generation, balance checks, airdrops, single-key transactions, and multi-party aggregated signing on Solana's Mainnet, Testnet, or Devnet.
Features
Generate Solana keypairs

Check account balances

Request airdrops

Send single-key transactions

Aggregate public keys for TSS

Perform multi-party signing (steps 1, 2, and signature aggregation)

Installation
Clone the repository:
bash

git clone https://github.com/0x-pankaj/solana-tss-cli-to-api.git
cd solana-tss-cli-to-api

Build the project:
bash

cargo build

Run the server:
bash

cargo run

The API will be available at http://127.0.0.1:8000/api.
```
API Endpoints
POST /api/generate: Generate a new keypair

POST /api/balance: Check account balance

POST /api/airdrop: Request an airdrop

POST /api/send_single: Send a single-key transaction

POST /api/recent_block_hash: Get recent block hash

POST /api/aggregate_keys: Aggregate public keys

POST /api/agg_send_step_one: Start TSS signing

POST /api/agg_send_step_two: Generate partial signature

POST /api/aggregate_signatures: Aggregate signatures and broadcast

```
<img width="1225" height="573" alt="image" src="https://github.com/user-attachments/assets/de03bf88-7238-4878-b840-098798377729" />
<img width="779" height="672" alt="image" src="https://github.com/user-attachments/assets/c255ef77-a977-4660-9490-a12153ea2417" />
<img width="1087" height="735" alt="image" src="https://github.com/user-attachments/assets/1fbb4576-813b-4848-a50a-842c1299ce03" />



