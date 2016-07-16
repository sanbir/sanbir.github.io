---
layout: post
title: Decentralized data marketplace
---

Hi everybody! I would like to discuss with you my idea about a new blockchain-based application. It may be not new, maybe I simply have not found it. Please let me know your thoughts, criticize me. Any feedback is welcome.

It is inspired by <a href="https://steem.io/">STEEM</a>. STEEM has proven that the distribution of monetary incentives can be well organized by using blockchain. For the first time in history, people directly received payments for their data of quality.

Internet of Things (IoT) is another massive trend nowadays. Numerous devices that belong to individuals, from a thermometer to an automobile, generate data streams, which may benefit many companies. As far as I know, currently there is no way for regular people to directly sell such data. The data is sometimes accumulated and then re-sold by a centralized authority (such as a manufacturer of the device or a cloud service provider). However, that sensing data must belong to the device owner. And, if there is a demand for this data, there should be a way for device owners to sell it.

Ideally, the process should be completely automated. Granted a certain set of permissions by the human owner only once, a device should be able to search for potential buyers of its data (which, in turn can be both humans or other devices that need exactly such data). And, when buyers and sellers agree on the price, the sale should proceed.

A possible algorithm:

1. Buyer sends a transaction to the contract with what kind of data it needs (e.g. geolocation, time interval, temperature) along with the money it is willing to pay.
2. Sellers send transactions to the contract with their data (possibly, hash or any other reference to the actual data) and the desired price.
3. If the agreement on the price is reached, the contract validates the quality of the data. (The quality validation can be done through a consensus among many sellers of similar data).
4. If the contract detects that there is data of the required quality (e.g. 95% of the sellers claim the temperature in the radius of 5 km from the Eiffel Tower is 23 C), those sellers receive the money the contract has from all the buyers agreed for that data at that price.
5. Contract sends the purchased data to the buyers.

Why blockchain? Because, if the entity bringing together buyers and sellers (broker, exchange) is implemented as a smart contract, it will never go offline and the market participants will trust it. Also, no complicated registration with revealing financial details would be required. A private/public key pair will be enough. So, devices can trade themselves without humans.

I understand that the implementation of a possible solution can be quite challenging. There should be a mechanism for validating the quality of the data. Also, the data itself cannot be stored directly on the blockchain for obvious reasons (1. the blockchain would quickly become too large; 2. if we believe the data has value, it should not be publicly exposed).

Could you please tell me if this is already implemented or is a complete bullshit? Do you know any projects working on something similar? What other challenges can you see? If it is too hard with IoT, what about a similar decentralized system, replacing, for example, Amazon Mechanical Turk?

Thank you very much for your comments!

### P.S.
I also published this post on <a href="https://steemit.com/@sanbir/decentralized-data-marketplace">Steemit</a>