# votingdapp

## Getting Started

```shell
◇  Installation successful! ───────────────────────────╮
│                                                      │
│  That's it!                                          │
│                                                      │
│  Change to your new directory and start developing:  │
│                                                      │
│  cd ./votingdapp                                     │
│                                                      │
│  Start the app:                                      │
│                                                      │
│  npm run dev                                         │
│                                                      │
│  Run Anchor commands:                                │
│                                                      │
│  npm run anchor build | test | localnet | deploy     │
│                                                      │
├──────────────────────────────────────────────────────╯

cd anchor && anchor build

anchor test --skip-local-validator --skip-deploy

solana-test-validator

solana config get && solana config set -ul

solana-keygen new

rm -rf .next && npm run dev

cd anchor && anchor deploy
```

### Prerequisites

- Node v18.18.0 or higher

- Rust v1.77.2 or higher
- Anchor CLI 0.30.1 or higher
- Solana CLI 1.18.17 or higher
```shell
alex@root:~/sol_dev_camp/solana-developer-bootcamp-2025$ rustc --version
rustc 1.84.1 (e71f9a9a9 2025-01-27)
alex@root:~/sol_dev_camp/solana-developer-bootcamp-2025$ cargo --version
cargo 1.84.1 (66221abde 2024-11-19)
alex@root:~/sol_dev_camp/solana-developer-bootcamp-2025$ solana --version
solana-cli 2.0.25 (src:40aee13c; feat:607245837, client:Agave)
alex@root:~/sol_dev_camp/solana-developer-bootcamp-2025$ anchor --version
anchor-cli 0.30.1
```

### Installation

```shell
npm i anchor-bankrun

npm install @solana/actions
```

#### Clone the repo

```shell
git clone <repo-url>
cd <repo-name>
```

#### Install Dependencies

```shell
pnpm install
```

#### Start the web app

```
pnpm dev
```

## Apps

### anchor

This is a Solana program written in Rust using the Anchor framework.

#### Commands

You can use any normal anchor commands. Either move to the `anchor` directory and run the `anchor` command or prefix the command with `pnpm`, eg: `pnpm anchor`.

#### Sync the program id:

Running this command will create a new keypair in the `anchor/target/deploy` directory and save the address to the Anchor config file and update the `declare_id!` macro in the `./src/lib.rs` file of the program.

You will manually need to update the constant in `anchor/lib/counter-exports.ts` to match the new program id.

```shell
pnpm anchor keys sync
```

#### Build the program:

```shell
pnpm anchor-build
```

#### Start the test validator with the program deployed:

```shell
pnpm anchor-localnet
```

#### Run the tests

```shell
pnpm anchor-test
```

#### Deploy to Devnet

```shell
pnpm anchor deploy --provider.cluster devnet
```

### web

This is a React app that uses the Anchor generated client to interact with the Solana program.

#### Commands

Start the web app

```shell
pnpm dev
```

Build the web app

```shell
pnpm build
```
