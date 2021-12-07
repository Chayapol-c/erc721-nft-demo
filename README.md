# Create and Deploying an NFT

## Deploy images with 2 ways
- ipfs
- pinata

Deploying a contract to rinkeby test net
```
brownie scripts/advanced_collectible/deploy_and_create.py --network rinkeby
```
Create a random collectible in [`pug`](./img/pug.png), [`shiba`](./img/shiba-inu.png), and [`bernard`](./img/st-bernard.png)
```
brownie scripts/advanced_collectible/create_collectible.py --network rinkeby
```
Create a metadata of each NFT as JSON file
```
brownie scripts/advanced_collectible/create_metadata.py --network rinkeby
```
Set a token uri to [opensea testnet](https://testnets.opensea.io/)
```
brownie scripts/advanced_collectible/set_tokenuri.py --network rinkeby
```

## running test
development
```
brownie run test
```
rinkeby testnet
```
brownie run test --network rinkeby
```