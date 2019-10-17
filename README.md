# Tic-Tac-Toe
The task is to create a basic two player command line tic tac toe game
backend in node js with ethereum based payment state channel

## What are state channels?

It’s a scaling solution to create decentralized applications and smart contracts that can be used by millions of users in almost real-time. They work by initiating a channel between 2 or more users in which they exchange encrypted, signed messages with the information of the transaction they want to execute.

They are called “state” because each interaction has to have a state that can be updated. 

State channels were created because ethereum applications quickly grew in popularity making the blockchain unusable since it was developed with a moderate use. They allow continuous transactions without paying for gas or waiting for miners to process the transactions.

## What do we need to set up a state channel?

At least 2 users that will interact with each other. A channel needs to be opened between 2 or more users. Similar to a chat application.

A smart contract with the state channel logic that will open and close it.

If the state channel will be used in a game, an escrow will be required for both users. That escrow in ether will be stored in the smart contract when opening the channel.

 A javascript application that will generate the signed messages that will be exchanged off-chain between the users.

 Metamask or a similar tool for signing messages. Signing messages don’t cost gas and they are executed instantly. It’s required from both users to sign the messages to guarantee that tehy are the ones generating such transaction.

 Email or any external application to exchange those signed messages to make that application possible.


## Requirements

You will need NodeJS and NPM installed, on linux:

```
sudo apt-get install nodejs
```
Once installed, this project uses EthJS for the blockchain interactions, and express as a simple we server.
In the project folder run:

```
npm install web3 ethjs express
```
Finally, to run the game you will need to create an ethereum account. For testing purposes I advise getting a Kovan testnet wallet and some Kovan ether to play around:



## Usage

Once the setup complete, start the webserver:
```		
nodejs app.js
```






