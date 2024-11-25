# GlacierVerifier guide by KHENZAR

Official Docs: [Here](https://docs.glacier.io/getting-started/glacier-nodes/run-testnet-nodes)

Follow More: [X / Twitter](https://twitter.com/cryptokhenzar)



# Step-by-Step Guide
## Hardware Requirement
Minimum Requirement: 
*   CPU with 1+ cores
*   2GB RAM
*   4 MBit/sec download internet service

Recommended:
* Fast CPU with 2+ cores
* 4GB+ RAM
* 8 MBit/sec download internet service

We need a wallet for the Verifier Node. It is recommended to use a Burner wallet.
1. Create New Wallet
2. Visit [Faucet](https://docs.bnbchain.org/bnb-smart-chain/developers/faucet/#claim-tbnb-from-online-faucet) and get some tBNB to new wallet
3. Visit [Bridge](https://opbnb-testnet-bridge.bnbchain.org/deposit) and bridge tBNB from BNB testnet to opBNB testnet
4. Copy private_key of node wallet (without 0x)


## Run a Node
```console
docker run -d -e PRIVATE_KEY=$YOUR_PRIVATE_KEY --name glacier-verifier docker.io/glaciernetwork/glacier-verifier:v0.0.2
```
Make sure to take faucet before running

## Check Logs
*You can run this command in Screen*
```console
docker logs -f glacier-verifier
```

## Check Status
https://testnet.nodes.glacier.io/status
