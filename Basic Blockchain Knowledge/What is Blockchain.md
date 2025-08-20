A blockchain is a distributed database or ledger shared across a computer network's nodes. They are best known for their crucial role in cryptocurrency systems, maintaining a secure and decentralized record of transactions, but they are not limited to cryptocurrency uses. Blockchains can be used to make data in any industry immutable—meaning it cannot  be altered.

## How Does a Blockchain Work

You might be familiar with spreadsheets or databases. A blockchain is somewhat similar because it is a database where information is entered and stored. The key difference between a traditional database or spreadsheet and a blockchain is how the data is structured and accessed.

[[output (1).png]]


The Bitcoin blockchain collects transaction information and enters it into a 4MB file called a [block](https://www.investopedia.com/terms/b/block-bitcoin-block.asp) (different blockchains have different size blocks). Once the block is full, the block data is run through a cryptographic hash function, which creates a hexadecimal number called the [block header](https://www.investopedia.com/terms/b/block-header-cryptocurrency.asp) hash.

The hash is then entered into the following block header and encrypted with the other information in that block's header, creating a chain of blocks, hence the name “blockchain.”

## Transaction Process

Transactions follow a specific process, depending on the blockchain. For example, on Bitcoin's blockchain, if you initiate a transaction using your [cryptocurrency wallet](https://www.investopedia.com/terms/b/bitcoin-wallet.asp)—the application that provides an interface for the blockchain—it starts a sequence of events.

In Bitcoin, your transaction is sent to a memory pool, where it is stored and queued until a miner picks it up. Once it is entered into a block and the block fills up with transactions, it is closed, and the mining begins.

Mempool(Memory Poll): 
	Means a waiting room for transactions
	When add a transaction. First, goes to Mempool  
	Miners choose transaction from here to put them in a block(Transaction with higher fees are have more priority)


Proof of Work(PoW):
	Means solving a hard mathematic puzzle for create a new block
	Miners trying billions time to found a new valid hash
	any miner who founds a correct hash, creates a new block and receive a reward

Nonce(Number used once): 
	Means a variable number in block 
	Miners changes the nonce to get the hash block which contains the network conditions
	Find the correct nonce => solving the PoW puzzle

Not all blockchains follow this process. For instance, the [Ethereum](https://www.investopedia.com/terms/e/ethereum.asp#:~:text=23-,The%20Bottom%20Line,deploy%20applications%20and%20smart%20contracts.) network randomly chooses one validator from all users with ether staked to validate blocks, which are then confirmed by the network. This is much faster and less energy intensive than Bitcoin's process.

Proof of Stake(PoS): after Ethereum 2.0
	Instead of  miners, There are users which stake their own Ethereum.(put lock on network)
	Network choose a random validator, this validator creates a new block. other validators check that block and approve it. if validator do the correct work it earns a reward if it doesn't
	it slashed


## Blockchain Decentralization

A blockchain allows the data in a database to be spread out among several network nodes—computers or devices running software for the blockchain—at various locations. This creates redundancy and maintains the fidelity of the data. For example, if someone tries to alter a record on one node, the other nodes would prevent it from happening by comparing block hashes. This way, no single node can alter information within the chain.

Because of this distribution—and the encrypted proof that work was done—the blockchain data, such as transaction history, becomes irreversible. Such a record could be a list of transactions, but private blockchains can also hold a variety of other information like legal contracts, state identifications, or a company's inventory. Most blockchains wouldn't "store" these items directly; they would likely be sent through a hashing algorithm and represented on the blockchain by a token.

## Blockchain Transparency

Because of the decentralized nature of the Bitcoin blockchain, all transactions can be transparently viewed by downloading and inspecting them or by using [blockchain explorers](https://www.blockchain.com/explorer?utm_campaign=dcomnav_explorer) that allow anyone to see transactions occurring live. Each node has its own copy of the chain that gets updated as fresh blocks are confirmed and added. This means that if you wanted to, you could track a bitcoin wherever it goes.

## Is Blockchain Secure?

Blockchain technology achieves decentralized security and trust in several ways. To begin, new blocks are always stored linearly and chronologically. That is, they are always added to the "end" of the blockchain. After a block has been added to the end of the blockchain, previous blocks cannot be altered.

A change in any data changes the hash of the block it was in. Because each block contains the previous block's hash, a change in one would change the following blocks. The network would generally reject an altered block because the hashes would not match. However, a change can be accomplished on smaller blockchain networks.

## Bitcoin vs. Blockchain 

Blockchain technology was first outlined in 1991 by Stuart Haber and W. Scott Stornetta, two researchers who wanted to implement a system where document timestamps could not be tampered with.4 But it wasn’t until almost two decades later, with the launch of Bitcoin in January 2009, that [blockchain had its first real-world application](https://www.investopedia.com/news/what-genesis-block-bitcoin-terms/).

## Blockchain vs. Banks
  
Blockchains have been heralded as a disruptive force in the finance sector, especially with the functions of payments and banking. However, banks and decentralized blockchains are vastly different.
