---
layout: post
title: Distributed Ledger Technology vs Blockchain
description: "Are Distributed Ledger Technology and Blockchain any different?"
tags: [bitcoin, blockchain, distributed ledger, ripple, certificate transparency]
categories: [Cryptocurrencies]
---

![Blockchain-based system]({{ site.url }}/images/Blockchain-based_system.png)
{: .image-right}

<h2>Hype</h2>
There was a lot of hype around blockchain in 2016. After Ethereum price [skyrocketed](https://coinmarketcap.com/currencies/ethereum/) in February, followed by numerous incredibly successful [crowdsales (ICOs)](https://en.wikipedia.org/wiki/List_of_highest_funded_crowdfunding_projects), such as The DAO, Lisk, and Waves, serious players started paying attention to this technology. Traditional financial institutions and tech giants like J.P. Morgan, Wells Fargo, IBM, and Intel initiated the [Hyperledger project](https://www.hyperledger.org/about/members). Microsoft and Consensys [integrated](https://marketplace.visualstudio.com/items?itemName=ConsenSys.Solidity) Ethereum's primary smart contract language Solidity into Visual Studio. [Governments](http://www.coindesk.com/blockchain-perfect-government-services-heres-blueprint/) started exploring opportunities to use blockchain as a substitution for cash and registries.

<h2>Distributed Ledger</h2>
The more centralized and permissioned blockchains are developed, the less popular the term “blockchain” becomes. Instead of it, the term “distributed ledger” is used more and more often. I have never understood the difference between the two, although, some sources claim they do and state that blockchain is one of possible implementations of a distributed ledger. According to [Wikipedia](https://en.wikipedia.org/wiki/Distributed_ledger) and its [citation](http://www.blockchaintechnologies.com/blockchain-definition), “a Blockchain is only one type of data structure considered to be a distributed ledger.” As examples of “different methodologies to achieve the same consensus,” they name Ripple, MultiChain, and HyperLedger Project. Let’s examine each one of them.

<h2>"Different methodologies"</h2>
**Multichain** officially calls itself an “open platform for blockchain applications” on their [main page](http://www.multichain.com/).

**HyperLedger** has a huge caption “blockchain technologies for business” on their [main page](https://www.hyperledger.org/) as well.

**Ripple** carefully tries to avoid the word “blockchain.” In the paper describing their protocol [Interledger](https://interledger.org/interledger.pdf), they state, “Unlike previous approaches, this protocol requires no global coordinating system or blockchain.” They even call blocks “ledgers.” However, they [admit](https://wiki.ripple.com/Consensus#Ledgers) that the data structure used for storing these “ledgers” is a hash tree. Also, their “ledger” is “repeatedly updated with transactions that successfully pass through the consensus process.” I will be thankful to anybody who can name the difference between these “ledgers” and blocks in Bitcoin. The data storage protocol seems to be exactly the same. The only difference lies in the consensus protocol.

<h2>Blockchain</h2>
I think there is a common misunderstanding in terms of what should be called a “blockchain.” In my opinion, the term “blockchain” should be used in its narrow sense and refer only to the data storage protocol (or “Internal State”). In the broad sense, the term “blockchain” is used to define the whole blockchain-based system, which also includes a peer-to-peer network protocol, transaction protocol, and consensus protocol (<http://chepurnoy.org/blog/2015/08/a-cryptocurrency-architecture/>). All these protocols, although necessary for any blockchain-based system, are completely independent from each other.

<h2>Certificate Transparency</h2>
An alternative point of view that “blockchain” should only refer to a particular implementation of the consensus protocol in Bitcoin, known as Proof-of-Work, can be found [here](https://tonyarcieri.com/on-the-dangers-of-a-blockchain-monoculture). The author of the article says,

>> I’ll again call out [Certificate Transparency](https://www.certificate-transparency.org/log-proofs-work) again as a system which has many of the same properties as the Bitcoin blockchain, but which I would not define as a “blockchain” and whose creators would probably not describe it as a “blockchain” either.

Here is the [answer](https://www.certificate-transparency.org/general-transparency) of the authors of Certificate Transparency:

>> These technologies are strongly related to the much-hyped blockchain. The reality, of course, is that there isn't a "the" blockchain, and that decentralisation is not always the answer. We are not making "the" blockchain, and we do not claim to support decentralisation.

I agree with them that there isn’t “the” blockchain. However, what they are doing is just “a” blockchain. If they do not decentralize their chain of blocks (Merkle tree), it will be a private blockchain with a much-simplified consensus protocol.

<h2>Summary</h2>
To sum up, I admit that the word “blockchain” causes a lot of confusion because people interpret it differently. However, I do not think calling it a distributed ledger is a good idea because it causes even more confusion when people think it is something new and different from blockchain. The term “blockchain” is bad and non-descriptive, just like the terms “machine learning” and “linear programming.” But, it is here to stay, just like them.
