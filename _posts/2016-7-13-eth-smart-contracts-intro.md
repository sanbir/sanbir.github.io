---
layout: post
title: Introduction to Ethereum smart contracts
description: "This post is about the very basics of Ethereum smart contracts."
tags: [ethereum, smart contracts, bitcoin, blockchain, solidity]
categories: [Cryptocurrencies]
---

The best source of information for understanding the concept of Ethereum so far for me is SURPRISE- SURPRISE… <a href="https://github.com/ethereum/wiki/wiki/White-Paper">Ethereum White Paper</a> by Vitalik Buterin, the inventor of Ethereum. It is written really good and worth every minute you spend reading it.

In my opinion, you don’t really need to read the original <a href="https://bitcoin.org/bitcoin.pdf">Bitcoin: A Peer-to-Peer Electronic Cash System</a> by Satoshi Nakamoto in order to understand all the Bitcoin background of Ethereum. Vitalik Buterin has clearly explained the main innovation of Bitcoin – <a href="https://github.com/ethereum/wiki/wiki/White-Paper#mining">decentralized consensus about the sequence in time, in which transactions take place</a>. 

Next, Vitalik shows that the decentralized consensus, not available before Bitcoin, has numerous potential real-world applications, far beyond cryptocurrencies and even finance. It can be decentralized domain name system, decentralized marketplaces, decentralized social networks just to name a few. However, the original Bitcoin protocol was not designed for general purpose programming. Its built-in scripting language has significant limitations. One of the most noticeable of them is a lack of loops. Pseudo-loops via conditional transfer of control are impractical from the performance standpoint since every iteration would be executed in a separate block, which takes 10 minutes to mine in Bitcoin.

![ETHEREUM Image]({{ site.url }}/images/ETHEREUM-ICON_Black.png)
{: .image-right}

Ethereum comes as a solution. It was designed specifically to run code of arbitrary complexity. It basically is a virtual machine, similar to Java’s JVM or .NET’s CLR. Like them, Ethereum virtual machine (EVM) executes commands in its own bytecode. A programmer can write code in a high-level language of choice, which is then compiled into the bytecode. There are 3 major such languages supported thus far: Solidity (similar to JavaScript), Serpent (similar to Python), and LLL (similar to Lisp). However, as it was explained in a <a href="https://medium.com/@ConsenSys/a-101-noob-intro-to-programming-smart-contracts-on-ethereum-695d15c1dab4">great article for beginners</a> (which I also highly recommend): “Just use Solidity. You prefer Python? Use Solidity.” Solidity receives the most of attention and support from developers.

So, what are smart contracts after all? Well, again, as Scott Driscoll said in <a href="https://app.pluralsight.com/library/courses/bitcoin-decentralized-technology">Introduction to Bitcoin and Decentralized Technology</a> they are neither smart nor contracts. They have nothing to do with artificial intelligence. Neither are they legal agreements. They are simply code that is executed on the Ethereum blockchain, by every blockchain node, every time a block with a transaction to its address (public key) gets validated.

Solidity code, dapps, and more are coming… Stay tuned!
