```shell
alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ solana-keygen grind --starts-with bos:1
Searching with 20 threads for:
        1 pubkey that starts with 'bos' and ends with ''
Searched 1000000 keypairs in 1s. 0 matches found.
Searched 2000000 keypairs in 3s. 0 matches found.
Searched 3000000 keypairs in 4s. 0 matches found.
Searched 4000000 keypairs in 6s. 0 matches found.
Searched 5000000 keypairs in 8s. 0 matches found.
Wrote keypair to bosyQ8VG6xa4hANEgZcWyf4duhpJHFrt72xTAh3CC6i.json


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ solana config set --keypair bosyQ8VG6xa4hANEgZcWyf4duhpJHFrt72
xTAh3CC6i.json
Config File: /home/alex/.config/solana/cli/config.yml
RPC URL: https://api.devnet.solana.com 
WebSocket URL: wss://api.devnet.solana.com/ (computed)
Keypair Path: bosyQ8VG6xa4hANEgZcWyf4duhpJHFrt72xTAh3CC6i.json 
Commitment: confirmed


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ solana config set --url https://api.devnet.solana.com
Config File: /home/alex/.config/solana/cli/config.yml
RPC URL: https://api.devnet.solana.com 
WebSocket URL: wss://api.devnet.solana.com/ (computed)
Keypair Path: bosyQ8VG6xa4hANEgZcWyf4duhpJHFrt72xTAh3CC6i.json 
Commitment: confirmed


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ solana config get
Config File: /home/alex/.config/solana/cli/config.yml
RPC URL: https://api.devnet.solana.com 
WebSocket URL: wss://api.devnet.solana.com/ (computed)
Keypair Path: bosyQ8VG6xa4hANEgZcWyf4duhpJHFrt72xTAh3CC6i.json 
Commitment: confirmed


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ solana balance
5 SOL

alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ solana-keygen grind --starts-with mnt:1
Searching with 20 threads for:
        1 pubkey that starts with 'mnt' and ends with ''
Searched 1000000 keypairs in 1s. 0 matches found.
Searched 2000000 keypairs in 3s. 0 matches found.
Wrote keypair to mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3.json


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ spl-token create-token --program-id TokenzQdBNbLqP5VEhdkAS6EPFLC1PHnBqCXEpPxuEb --enable-metadata mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3.json
Creating token mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3 under program TokenzQdBNbLqP5VEhdkAS6EPFLC1PHnBqCXEpPxuEb
To initialize metadata inside the mint, please run `spl-token initialize-metadata mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3 <YOUR_TOKEN_NAME> <YOUR_TOKEN_SYMBOL> <YOUR_TOKEN_URI>`, and sign with the mint authority.

Address:  mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3
Decimals:  9

Signature: 3M2w82GCSLomjEsU1Q4yNxBgxwBbtoiMYqzdNwZUykstX8VaJrFyShboyZmnZSptD5jGb5nTArU5FMZXBNjBg75L


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ spl-token initialize-metadata  mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3 'Example' 'EXMPL' https://raw.githubusercontent.com/mikemaccana/token-command-line/main/metadata.json

Signature: 5cEMFJ7UpnKnS8t2nBXvFH4hitLFTSTEv5trwY824zgpqd4EgmSZiEt8q9HDW1gFZNg5Zn6gHVHpoviTPHMkVd7C

https://explorer.solana.com/address/mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3?cluster=devnet


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ spl-token create-account mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3
Creating account HcdCLVRwnzx6sCbYdDb9JApZEDMGA4tL9PKBuT6KEb7x

Signature: 2jAwaXp8s2jS6RhDjNSXxDqoX4B3dkKy4cmeu4Rj6KKysFYL6XgXWLePZRcusHngxPaWpqt3DyQ2Bq6aTDtEbWzG


alex@DESKTOP-UKE5TJQ:~/sol_dev_camp/solana-developer-bootcamp-2025/project-5/new-token$ spl-token mint mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3 1000
Minting 100 tokens
  Token: mntaoFwwQZ6YHcHM7fjAoq4HdiEbSZ6CTWeAdkh41V3
  Recipient: HcdCLVRwnzx6sCbYdDb9JApZEDMGA4tL9PKBuT6KEb7x

Signature: 28axmXdNx4Mxpz5MvSk9oMwx2D7CEwyeP1zUpztH9A1a1tmJmwg8Jh8TT7dLP1HcUz6a2XS3haiBjWW2dkWxn1b3
```
