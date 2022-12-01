# Hi! 

This is one of my first projects. I learned all of these skills from Free Code Camp with Patrick Collins as the instructor. I highly recommend checking them out if you are interested in learning about and partaking in this amazing ecosystem as well.
The purpose of this contract is to have a place where anyone can send money, though only the person who deployed the contract can withdraw the funds from it. This is the back-end of the fullstack application.  

This project has been a great way to familiarise myself with the different frameworks for developing, testing, and deploying blockchain applications.  

It has also been great for really understanding important principles for smart contract development!  

Now, onto the project

# Project

## The requirements to run this code

- `git --version` 
- `node --version` 
- `yarn --version`

## Start
1. 
```
$ git clone 
$ cd hardhat-fund-me-fcc
$ yarn
```

## Deployment to testnet

2. Set `GOERLI_RPC_URL`, `PRIVATE_KEY` and add them to a `.env` file, chainging `.env.example` to `.env`.

- `PRIVATE_KEY`: The private key of your metamask
- `GOERLI_RPC_URL`: This is url of the goerli testnet node. Get it from: [RPC's](https://rpc.info/)

3. Make sure you have testnet ETH!!

Go to [faucets.chain.link](https://faucets.chain.link/) to get some!

4. Deploy

```
yarn hardhat deploy --network goerli
```

## Scripts

After deploy to a testnet, you will be able to run the scripts.  
To fund the contract:

```
yarn hardhat run scripts/fund.js --network goerli
```

To withdraw the funds from the contract:
```
yarn hardhat run scripts/withdraw.js --network goerli
```

Go on over to the front end to being interacting via a minial GUI. [full-stack-fund-me](https://github.com/jnealew/full-stack-fund-me)


