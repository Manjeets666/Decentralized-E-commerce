# Decentralized: E-commerce Store

**Overview**: This is a simple E-commerce DApp store where anyone can sell/buy products. Truffle framework has been used to build the entire app end-to-end.

By utilizing IPFS to host the site(image files first, site fully with other assests would be shift to IPFS later in the future) to make it truly decentralized. 
- The contract will also feature an escrow system, which involves a 3-person approval to release funds. This means that instead of the buyer sending money to the sender directly, a third person holds the funds until the others have agreed funds should be released (or refunded). **To be added**

## User Stories
The following user stories are completed:

- [x] Users can see products for sale, and buy them through a web interface.
- [x] Users can add products for sale using a web interface.
- [x] Product images are being hosted on IPFS.
- [x] The WebUI is updated as the user makes transactions, by listening to Solidity Events.
- [x] A functioning escrow system:
  * Instead of transferring money directly to the buyer, money is sent to an "escrow" holder.
  * This person will release funds or refund funds based on consensus from 2 out of the 3 parties.
  * The escrow contract will deduct a 1% fee for these services.

## Development

> *Prerequisites*
> - [truffle](http://truffleframework.com/)
> - [ipfs](https://ipfs.io/docs/install/)

### Building and Deploying the contract

```
$ truffle compile
$ truffle migrate
```

### Start the Web App

```
$ npm install
$ npm run dev
```

#### Live deploy link
> [Decentralized E-commerce](https://dapp-ecom.netlify.app/)
