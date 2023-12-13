Clone Aptos Core
git clone https://github.com/aptos-labs/aptos-core.git

Install Aptos CLI
brew install aptos

Change Dir
cd aptos-core

Run automated Script
./scripts/dev_setup.sh

Update your current shell environment
source ~/.cargo/env

Build and Run test
cargo build
cargo test -- --skip prover

Prover (new Terminal Session)

Run the dev setup script to prepare your environment
./scripts/dev_setup.sh -yp

Update your current shell environment
source ~/.profile

Run Move Prover to prove an example
aptos move prove --package-dir aptos-move/move-examples/hello_prover/