---
title: a survey of blockchain-based technologies
date: 2022-06-16 15:11:15
tags:
---

A decentralized (p2p) timestamping technique was invented by Haber and Stornetta in 1994. The resulting data structure from application of this technique is called _distributed ledger_.

What are the properties of a distributed ledger?

As far as software used by clients is concerned, 

1. it is an exchange of block of data. These blocks are ordered(using various algorithms)& replicated(across nodes) & this ordering & replication makes the data in those blocks immutable(subject to conditions[^1]).

2. This exchange of data in the blocks is over a network of peers. This networking is done by each end-point for the _purpose of participation_ and not for the _purpose of production_, which is the default.

3. It is a data structure that secures its' purpose[^2].

Data structures are techniques to store and retrieve data; data which is stored on data _drives_. **If a blockchain is a data stucture, whose drive is it running on?** A generic blockchain data structures may be considered agnostic to the data they store, whereas a specific blockchain may be considered _secure_.

[^2]: This *security* is not data security which is the property of drive system(database), neither is this proof-of-work which secures structure of data; it is about the meaning of data. Bitcoin might say this data is transaction of bitcoin units, while ethereum might say this data is transaction of smart contract state changes caused by transaction of ethereum units. 

[^1]: Immutability has a degree of trust or a probability of failure, depending on the algorithm used.
