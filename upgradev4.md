# Glacier Verifier Node v3

- Official Docs: [Here](https://docs.glacier.io/getting-started/glacier-nodes/run-testnet-nodes)

- If you are just starting you can follow the previous guide

## Step-by-Step Guide
1. Stop&Remove Docker Container
```console
docker stop glacier-verifier 
```
```console
docker rm glacier-verifier 
```

2. Run Node
```console
docker run -d -e PRIVATE_KEY=YOUR_PRIVATE_KEY --name glacier-verifier docker.io/glaciernetwork/glacier-verifier:v0.0.4
```
- Enter your node wallet private key without 0x

3. Check Logs
```console
docker logs -f glacier-verifier
```

##

https://testnet.nodes.glacier.io/status
---

That's all !

* [Twitter](https://twitter.com/cryptokhenzar)
