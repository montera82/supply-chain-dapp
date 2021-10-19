## Coffee Supply Chain System


### Motivation
The project in this repository is an Ethereum based DApp that shows the Supply chain flow between a Seller and a Buyer. The Blockchain can enable more transparent and accurate end-to-end tracking in the supply chain process and the key goal is to achieve efficient fulfillment of demand and drive outstanding customer value.


### General
A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

Find below the full personas involved in the system : 

FARMER : The farmer persona is responsible is the originator in the system and has early responsibilites including harvesting, processing and packaging the Coffee for sale.

DISTRIBUTOR : The distrubutor role is in direct contact with the farmer and has the ability to buy harvested and packaged Coffee that are available for sell.

RETAILER : The retailer has the ability to get coffee shipments 

CONSUMER :  The consumer is the end user that has the ability to purchase processed Coffeee from the retailer.

### Architecture
This project uses UML to describe the activity, sequence, state and datamodel of the entire supply chain system, highlighing the interactions and states of the system end to end.

UML was choosen because of how simple and yet clear it 
Check out the folder `./UML` for all the related diagrams. 

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

### User Interface
The DApp User Interface when running look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)

### Libraries Used
Find below the modules used in this project which are all open source.

1. truffle-hdwallet.js@1.0.17 - Since we are connecting with Infura to deploy the smart contract to the ethereum blockchain, we are choosing to use this lib, which helps elangantly manage the connection string.

2. web3.js@1.5.2- This library allows us to access the ethereum blockchain from the web browser.


### Other Library used.
1. jquery,Node v12.22.4,
2. Truffle v5.4.6 
3. Solidity - 0.4.24 (solc-js)
4. https://www.npmjs.com/package/ipfs-http-client  ( via cdn ): To interact with ipfs for file uploads

### IPFS
Because we the goal of our design is to be fully decentralised, i am choosing to host the project on IPFS, instead of a central server. Follow the linke below to see the project on IPFS.

https://bafybeicaul43frdwj24e4fvekrffifi3a2grxlvmprox6uww4r3g7uip5m.ipfs.infura-ipfs.io/


### Installing

> The code is written for **Solidity v0.4.24**. 

Find below a step by step series of examples that tell you have to get a development env running:

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

### General

The Smart contract is deployed to the Rinkeby Testnet here:
https://rinkeby.etherscan.io/address/0x2D1CC2fDee3e5A9E7584A245E3389f612e2c562d


### Invoking the tests

`truffle test --network test`

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS