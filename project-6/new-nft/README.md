## Installation

```shell
npm i @metaplex-foundation/mpl-token-metadata

npm i @metaplex-foundation/umi-bundle-defaults

npm i @solana-developers/helpers
```

## Config

```shell
solana config set --keypair ~/.config/solana/id.json

solana config get

solana address

npx esrun create-collections.ts
```

## Run

### Create Collection

``` shell
alex@MacBook-Air new-nft % npx esrun create-collections.ts
Loaded user AHdyMbVNGT8YVWCMZnfakVv53GwiJwvEFbkCYruZikZC
Set up Umi instance for user
Created Collection 📦! Address is https://explorer.solana.com/address/2WoYAJZ1qQEWVa21XmvAqBRQRRTtpCv9Dg3EBB4RHqsk?cluster=devnet
```

### Create NFT

```shell
alex@MacBook-Air new-nft % npx esrun create-nft.ts        
Loaded user AHdyMbVNGT8YVWCMZnfakVv53GwiJwvEFbkCYruZikZC
Set up Umi instance for user
Creating NFT...
🖼️ Created NFT! Address is https://explorer.solana.com/address/GjP5f8jz21q7cuCmCb2QrLTJRHPEw6cmyhMB7gg9qBrQ?cluster=devnet
```

### Verify NFT belong to Collection

```shell
alex@MacBook-Air new-nft % npx esrun verify-nft.ts 
Loaded user AHdyMbVNGT8YVWCMZnfakVv53GwiJwvEFbkCYruZikZC
Set up Umi instance for user
✅ NFT GjP5f8jz21q7cuCmCb2QrLTJRHPEw6cmyhMB7gg9qBrQ verified as member of collection 2WoYAJZ1qQEWVa21XmvAqBRQRRTtpCv9Dg3EBB4RHqsk! See Explorer at https://explorer.solana.com/address/GjP5f8jz21q7cuCmCb2QrLTJRHPEw6cmyhMB7gg9qBrQ?cluster=devnet
```
