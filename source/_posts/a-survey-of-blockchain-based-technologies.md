---
title: a survey of blockchain-based technologies
date: 2022-06-16 15:11:15
tags:
---

# Introduction

This article is being written in 2022, more than a decade later than invention of bitcoin.  In 2013, I spent a few months studying the technology behind bitcoin, just a couple years after graduating as a bachelor of engineering in computer science. Since then I have been working in the domain & here are a few things I learnt, that are not yet published.

## Distributed Ledgers of what?

A timestamping technique was invented by Haber and Stornetta in 1994.
Satoshi Nakamoto used it to create a p2p timestamp of transactions.

Blockchain is a collection of blocks of data, each of which contains a hash of the previous block, and block of data. _If the data in the blocks are not transactions, they are still chained blocks & this information structure of this data is still a "blockchain"_. This is important because in case of ethereum, the data is the state of the ethereum virtual machine.

**Blockchains are generic ledgers**, bitcoin & ethereum etc. are specific ledgers.

## Is blockchain a data structure?

The data structure, where every node contains the hash of the previous node, may be considered a blockchain? 
It must be noted that traditionally in data structures, we would use "node" to refer to a _location in computer's memory_, but in case of blockchains, a node is a _location in the network's memory_ & that node uses any _data structure_ to hold this information structure, ing away information from the data.

**Blockchains are information structures**, not data structures.

## Properties of a distributed ledger

As far as software used by the users of this technique is concerned, 

1. it is a p2p exchange of _data_. The discrete files of this data are called _blocks_. All participants replicate the construction of continous stream of **information** by orderering these blocks(using various algorithms)& this ordering & replication makes the information immutable(subject to conditions[^1]).

2. This exchange of data in the blocks is over a network of peers. This networking is done by each end-point for the _purpose of participation in securing the immutability_ of the stream of information and not for the _purpose of production_, which is the default.

3. It is a data structure that secures its' purpose[^2].

## Life of a blockchain

Last bitcoin will be mined around 2140.
The life of a blockchain is the life of the network of nodes, but not the life of the data in the blocks. The data in the blocks is an immutable record of the transactions that were made in the network. Dead ledgers are frozen in time records of activity.

[^2]: This *security* is not data security which is the property of drive system(database), neither is this proof-of-work which secures structure of data; it is about the meaning of data. Bitcoin might say this data is transaction of bitcoin units, while ethereum might say this data is transaction of smart contract state changes caused by transaction of ethereum units. 

[^1]: Immutability has a degree of trust or a probability of failure, depending on the algorithm used.
