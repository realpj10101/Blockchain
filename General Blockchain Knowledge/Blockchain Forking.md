
## Fork(blockchain)

In [blockchain](https://en.wikipedia.org/wiki/Blockchain "Blockchain"), a **fork** is defined variously as:

- "What happens when a [blockchain](https://en.wikipedia.org/wiki/Blockchain "Blockchain") diverges into two potential paths forward",
- "A change in protocol", or
- A situation that "occurs when two or more blocks have the same block height".[[1]](https://en.wikipedia.org/wiki/Fork_\(blockchain\)#cite_note-mastering-1): glossary [[a]](https://en.wikipedia.org/wiki/Fork_\(blockchain\)#cite_note-4)

Forks are related to the fact that different parties need to use common rules to maintain the history of the blockchain. When parties are not in agreement, alternative chains may emerge. While most forks are short-lived some are permanent. Short-lived forks are due to the difficulty of reaching fast [consensus](https://en.wikipedia.org/wiki/Consensus_\(computer_science\) "Consensus (computer science)") in a distributed system. Whereas permanent forks (in the sense of protocol changes) have been used to add new [features](https://en.wikipedia.org/wiki/Software_feature "Software feature") to a blockchain, they can also be used to reverse the effects of [hacking](https://en.wikipedia.org/wiki/Computer_hacking "Computer hacking") such as the case with [Ethereum](https://en.wikipedia.org/wiki/Ethereum "Ethereum") and [Ethereum Classic](https://en.wikipedia.org/wiki/Ethereum_Classic "Ethereum Classic"), or avert catastrophic [bugs](https://en.wikipedia.org/wiki/Software_bug "Software bug") on a blockchain as was the case with the [bitcoin](https://en.wikipedia.org/wiki/Bitcoin "Bitcoin") fork on 6 August 2010.[_[citation needed](https://en.wikipedia.org/wiki/Wikipedia:Citation_needed "Wikipedia:Citation needed")_] The concept of blockchain technology was first introduced in 2008 by an unknown person or group of people using the pseudonym “Satoshi Nakamoto” in a white paper describing the design of a decentralized digital currency called Bitcoin. Blockchain forks have been widely discussed in the context of the [bitcoin scalability problem](https://en.wikipedia.org/wiki/Bitcoin_scalability_problem "Bitcoin scalability problem").

## Types of forks

### Accidental Fork

* When two or more miners find a valid block almost simultaneously
* So for a moment there are two parallel chains 
* Network solve it by  longest chain law
	* Each miner continues with one of the chains 
	* Finally, one of the chains is goes longer than others -> It will be valid
	* Short chain blocks will be orphaned blocks and they will left aside

##### Features 

* Temporary and short-term
* Usually happens because of network latency or concurrency in mining  
* It does not threaten the security of blockchain because it is resolved quickly


### Intentional Fork

* When society or developers change the protocol rules intentionally
* This cause network splits in two sections:
	* Who continue with the new rules
	* Who stay on old rules

##### Features 
* long-term or permanently
* In two shapes
	* Soft Fork -> compatible with the previous version
	* Hard Fork -> incompatible change(cause two separate chain) 

### Hard Fork

A _hard fork_ is a change to the blockchain protocol that is not backward compatible and requires all users to upgrade their software in order to continue participating in the network. In a hard fork, the network splits into two separate versions: one that follows the new rules and one that follows the old rules.

For example, Ethereum was hard forked in 2016 to "make whole" the investors in [The DAO](https://en.wikipedia.org/wiki/The_DAO_\(organization\) "The DAO (organization)"), which had been hacked by exploiting a vulnerability in its code. In this case, the fork resulted in a split creating Ethereum and [Ethereum Classic](https://en.wikipedia.org/wiki/Ethereum_Classic "Ethereum Classic") chains. In 2014, the [Nxt](https://en.wikipedia.org/wiki/Nxt "Nxt") community was asked to consider a hard fork that would have led to a rollback of the blockchain records to mitigate the effects of a theft of 50 million NXT from a major [cryptocurrency exchange](https://en.wikipedia.org/wiki/Cryptocurrency_exchange "Cryptocurrency exchange"). The hard fork proposal was rejected, and some of the funds were recovered after negotiations and ransom payment. Alternatively, to prevent a permanent split, a majority of nodes using the new software may return to the old rules, as was the case with Bitcoin split on 12 March 2013.[[7]](https://en.wikipedia.org/wiki/Fork_\(blockchain\)#cite_note-ArsFork-8)

A more recent hard-fork example is of Bitcoin in 2017, which resulted in a split creating [Bitcoin Cash](https://en.wikipedia.org/wiki/Bitcoin_Cash "Bitcoin Cash").[[8]](https://en.wikipedia.org/wiki/Fork_\(blockchain\)#cite_note-bpr-9) The network split was mainly due to a disagreement in how to increase the transactions per second to accommodate for demand.[[9]](https://en.wikipedia.org/wiki/Fork_\(blockchain\)#cite_note-CNN_2017-08-01-10)

### Soft Fork

A _soft fork_ is a backward-compatible change to the blockchain protocol that allows new rules to be introduced without requiring all users to upgrade their software. In a soft fork, a majority of the network’s miners implement the new rules and begin following the updated version of the blockchain. The rest of the network can continue to follow the blockchain, but they will be unable to validate that new blocks follow the updated rules. Because a soft fork is backward-compatible, it does not result in the creation of a new blockchain or the splitting of the network. Instead, it allows the network to gradually transition to the new rules while still maintaining compatibility with the old rules.

### Source code fork

A _source code fork_ or _project fork_ is when developers take a copy of source code from one cryptocurrency project and start **independent** development on it, creating a separate and new piece of blockchain. Such examples are; [Litecoin](https://en.wikipedia.org/wiki/Litecoin "Litecoin") a source code fork of [Bitcoin](https://en.wikipedia.org/wiki/Bitcoin "Bitcoin"), [Monero](https://en.wikipedia.org/wiki/Monero "Monero") fork of Bytecoin and [Dogecoin](https://en.wikipedia.org/wiki/Dogecoin "Dogecoin") fork of Litecoin.



