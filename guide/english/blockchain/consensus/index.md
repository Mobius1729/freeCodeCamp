---
title: Consensus
---

## Consensus
Most discussions of consensus begin with Byzantine Fault Tolerance (BFT). BFT is derived from the Byzantine Generals' Problem, and understanding how it relates to decentralized systems allows for the implementation of other consensus algorithms used today.

As explained on Wikipedia (https://en.wikipedia.org/wiki/Byzantine_fault_tolerance):

>A group of generals, each commanding a portion of the Byzantine army, encircle a city. These generals wish to formulate a plan for attacking the city. In its simplest form, the generals must decide only whether to attack or retreat. Some generals may prefer to attack, while others prefer to retreat. The important thing is that every general agree on a common decision, for a halfhearted attack by a few generals would become a rout, and would be worse than either a coordinated attack or a coordinated retreat.


## Types of Consensus Algorithms 
(See for more: https://hackernoon.com/a-hitchhikers-guide-to-consensus-algorithms-d81aae3eb0e3)

- Proof of Work
- Proof of Stake
- Proof of Authority 

## Proof of Work
Proof of work is a consensus mechanism which uses computational power to achieve consensus in the network. In Proof of Work there are designated nodes, dubbed 'miners', who are attempting to solve a computationally-difficult problem in order to add *their* blocks to the network. 
Miners are tasked with verifying transactions and including them in a block. They then hash the block's header with a random number, called the *nonce* in order to achieve a hash that meets the difficulty of the network. The difficulty is how many 0s a hash should begin with. For instance, if the difficulty was 5, then the block's hash should look like 00000f16...
The only way to find the right hash is via testing out multiple nonce values. This takes up significant computing power and is a 'proof of the miners work'. Due to the massive amount of computation required to verify a block, it becomes very very difficult very fast to attempt to alter the contents of a block. Proof of work is the only consensus mechanism known to be Sybil attack resistant.
