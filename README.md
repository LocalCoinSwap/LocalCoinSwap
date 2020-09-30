# LocalCoinSwap
:rocket: The most popular non-custodial P2P fiat on-ramp


## What is LocalCoinSwap?

LocalCoinSwap is a collection of systems which work together on multiple blockchains to provide a fast and simple way for anyone, anywhere in the world, to trade between local currency and cryptocurrency.

The user experience is an intuitive marketplace, built in a style similar to eBay. People using the protocol trade local currency directly with each other, while the cryptocurrency portion of the trade is protected under escrow.

The underlying technology is non-custodial in nature, never requiring users to trust LocalCoinSwap, or anyone else, with their private keys. However, the protocol uses special escrow techniques to protect the cryptocurrency until the local payment is completed, which allows disputes between buyers and sellers to be moderated and resolved fairly.

The governance of the system is driven a token model which shares the trade fees and decision-making of the exchange.


## How does the LocalCoinSwap protocol work?

The LocalCoinSwap trading protocol consists of 3 layers: The Blockchain layer, the API layer, and the application (or dApp) layer. Each of these layers combine to form the overall user experience.

The LocalCoinSwap governance protocol consists of a token, LCS. Holders of the LCS token can vote on key issues, and a regular percentage of the protocol revenue is given to holders in the form of buybacks. LocalCoinSwap is currently in the process of transitioning into a DAO.


### Layer 1. Blockchain

The implementation of our protocol on this layer is different for every cryptocurrency, due to differences in how individual blockchains function. On crypto such as Ethereum and Dai we use smart contracts, on cryptos such as Bitcoin we use special transaction scripts, and on substrate-based chains like Kusama we use a special module on the Blockchain runtime itself.

Regardless of the exact implementation, our first layer solution always follows the same rules:

Until a trade is completed, it must not be possible for the buyer or seller to move the cryptocurrency
The crypto must never be in possession of LocalCoinSwap. In other words: we must never have the power or ability to take the funds of the trade for ourselves
If the buyer and seller agree (for example the seller receives the cash payment, or the buyer agrees to cancel), the funds must travel only to the buyer or seller, and only after the trade is complete
If the buyer and seller disagree, then LocalCoinSwap must be able to decide who is the rightful owner of the cryptocurrency.
The layer 1 implementation must be open-source, and publicly verifiable by all parties

Our current Blockchain-layer integrations are documented here:

**Bitcoin:**  
https://github.com/LocalCoinSwap/bitcoin-trading-scripts

**Kusama:**  
https://github.com/LocalCoinSwap/kusama-multisig-implementation

**Ethereum**  
Ethereum smart contracts are publicly verifiable on Etherscan during trading, but a (v2) release is currently close to launch.


### Layer 2. API

This layer interfaces with the Blockchain layer to provide a level of persistence, such as aggregating buy and sell offers, and maintaining user profiles and trade history. This layer also provides a single unified interface for all the cryptos offered on LocalCoinSwap.

Our API layer is publicly documented so that users can build their own interfaces on top of it if they wish, for example integrating automated trades in their own applications.

You can view the surface interface of the API layer here:  
https://localcoinswap.com/api-docs/

We are constantly improving the API layer, and also welcome user input. If you have any features you want on the API layer, or are confused about how to use it, just submit an issue on our open-source examples repo, and we’ll implement your use-case and/or show you how to integrate it in your chosen language:  
https://github.com/LocalCoinSwap/api-examples


### Layer 3. Application / dApp

The application / dApp layer interacts with the persistence layer to provide a simple user interface for trading. Currently we provide the application layer in the form of the LocalCoinSwap website https://localcoinswap.com, but this is only one out of many possible application layers with the technology we have built.

We are currently investigating different ways of distributing the application layer (and the API layer), to further improve decentralization and censorship-resistance.


### Layer 4: Governance

The governance of LocalCoinSwap centers around the LCS token, and we are also investigating the launch of a LocalCoinSwap DAO. Our current implementation of LCS can be found here:  
https://github.com/LocalCoinSwap/governance-token



## LocalCoinSwap resources

Platform: https://localcoinswap.com/  
Blog: https://blog.localcoinswap.com/  
Telegram: https://t.me/localcoinswap  
Twitter: https://twitter.com/Localcoinswap_  
Facebook: https://www.facebook.com/localcoinswap  
YouTube: https://www.youtube.com/channel/UCfUR13Y6dzv84EPG9uY1BUA  
LinkedIn: https://www.linkedin.com/company/localcoinswap 
