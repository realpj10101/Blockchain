 
Unlike a centralized server operated by a single company or organization, decentralized storage systems consist of a peer-to-peer network of user-operators who hold a portion of the overall data, creating a resilient file storage sharing system.

## Blockchain storage

### What is blockchain storage

Blockchain storage is a way of saving data in a decentralized network, which utilizes the unused hard disk space of users across the world to store files. The decentralized [infrastructure](https://www.techtarget.com/searchdatacenter/definition/infrastructure) is an alternative to centralized [cloud storage](https://www.techtarget.com/searchstorage/definition/cloud-storage) and can solve many problems found in a centralized system.

### How blockchain storage works

[Blockchain] relies on distributed ledger technology ([DLT](https://www.techtarget.com/searchcio/definition/distributed-ledger)). The DLT acts as a decentralized database of information about transactions between various parties. Operations fill the DLT in chronological order and are stored in the ledger as a series of blocks. An interconnected chain is formed between blocks with each one referring to the block before it, thus creating a blockchain.

In blockchain storage, files are first broken apart in a process called [sharding](https://www.techtarget.com/searchoracle/definition/sharding). Each shard is copied to [prevent loss of data](https://www.techtarget.com/searchcio/tip/8-blockchain-security-risks-to-weigh-before-adoption) should an error occur during transmission. The files are also [encrypted](https://www.techtarget.com/searchsecurity/definition/encryption) with a private key that makes it impossible for it to be viewed by other nodes in the network. The replicated shards are distributed among decentralized nodes all over the world. The interactions are recorded in the blockchain ledger, allowing the system to confirm and synchronize the transactions across the nodes in the blockchain. Blockchain storage is designed to save these interactions forever and the data can never be changed.

1- **Sharding**: Files divided to smaller sections

2- **Replication**: Each shard has a copy so if one the them breaks or been lost on transaction - it restores 

3- **Distribution**: This encrypted shards distributed between thousands of nodes 

4- **Ledger Recording**: All of this exchanges(who saves which shard) registers on blockchain 

5- **Immutability**: When data registered. saves forever and it cannot be change


### Blockchain storage vs. cloud storage 

Blockchain storage is a potentially cheaper, more secure and more reliable alternative to centralized cloud storage.

Providers of centralized cloud storage prevent data loss by making copies of the data and storing it in different data centers. The large amount of data that is duplicated in this process can create excessive amounts of surplus information. Also, cloud storage requires enterprise-grade hardware for its [data centers](https://www.techtarget.com/searchdatacenter/definition/data-center). These factors can make centralized data storage significantly more expensive than blockchain storage.

By taking advantage of the empty space on users' devices across the world, blockchain storage can cut up to 90% of the cost of centralized cloud storage, proponents claim. [Individuals and businesses can profit](https://www.techtarget.com/searchcio/tip/5-tips-to-successfully-implement-blockchain-for-businesses) by renting out the unused space on their hard disks for others to use.

### Advantages of blockchain storage 

In addition to the advantages explained above, having data stored across dozens of individual nodes also gives [blockchain storage security benefits](https://www.techtarget.com/searchcio/tip/Permissioned-vs-permissionless-blockchains-Key-differences). Encrypting the files and distributing them across the decentralized network makes it harder for [hackers](https://www.techtarget.com/searchsecurity/definition/hacker) to access the data. There is no central entity controlling access to files or possessing the keys needed to decrypt the files. The private keys are controlled entirely by the user, making it theoretically impossible for a third party to access the files. Sharding also promotes security and privacy.

Blockchain storage could also allow faster and more customizable storage systems because [users are able to manipulate settings](https://www.techtarget.com/searchcio/feature/Todays-blockchain-use-cases-and-industry-applications), such as the speed of retrieval and redundancy.


###  Decentralized Storage

Unlike a centralized server operated by a single company or organization, decentralized storage systems consist of a peer-to-peer network of user-operators who hold a portion of the overall data, creating a resilient file storage sharing system. These can be in a blockchain-based application or any peer-to-peer-based network.

Ethereum itself can be used as a decentralized storage system, and it is when it comes to code storage in all the smart contracts. However, when it comes to large amounts of data, that isn't what Ethereum was designed for. The chain is steadily growing, but at the time of writing, the Ethereum chain is around 500GB - 1TB ([depending on the clientopens in a new tab](https://etherscan.io/chartsync/chaindefault)), and every node on the network needs to be able to store all of the data. If the chain were to expand to large amounts of data (say 5TBs) it wouldn't be feasible for all nodes to continue to run. Also, the cost of deploying this much data to Mainnet would be prohibitively expensive due to [gas](https://ethereum.org/en/developers/docs/gas/) fees.

Due to these constraints, we need a different chain or methodology to store large amounts of data in a decentralized way.

#### Why Ethereum has problem is having problem in its own?

1- Each node has to save many data
	When you say "full-node" means it contains all blocks and transactions.
	For now it is about 1TB. which if we want put videos and datasets easily reaches to several TB.
	In this case only large companies  can run nodes -> network is not decentralized any more

2- Gas Fee its going to be very expensive 
	 saving 1KB data on Ethereum might worth several dollars, now imagine you want to put 1GB  file on it -> the cost is millions of dollars

#### Solutions
Here blockchain combines with other networks.

1- User uploads a file 
- File divides to smaller parts (Shards/Chunks).
- This pieces distributed among P2P networks  like Storj, Arweave, Filecoin, IPFS.
- This data encrypts, so nodes which have the files cannot see the content of files.

2- Store Hash (CID)
- All the files convert to CID with an hash algorithm (like SHA-256).
- If one bite changes, all the hash changes.

3- Only hash saves on Ethereum 
- Only hash or pointer saves on ethereum blockchain.
- In this way data is immutable cause data registered on blockchain forever.

4- File backup
- Anyone wants to receive file get hash from ethereum.
	- Then asks form P2P(IPFS, Filecoin) network.
	- Network uses the hash, collect the correct peaces of file and gives it to user.

[[output (7).png]]

When looking at decentralized storage (dStorage) options, there are a few things a user must keep in mind.

- Persistence mechanism / incentive structure
- Data retention enforcement
- Decentrality
- Consensus


1- Persistence mechanism / incentive structure
- In dStorage there is no centralized company for give a promise to save your file
- It has to be motivated system to so that nodes can rent out part of their space
	for example:
		Filecoin -> get FIL token for saving files.
		Storj/ Sia -> users pay, nodes get reward for saving data.

*  Without this mechanism, there is no reason for node to save your data -> data might be lost

2- Data retention enforcement
 * Only motivation is not enough. it has to be mechanism to confirm that node really saves the file 
 * Usually it done with cryptographic proofs:
	 * Proof-of-replication -> Node has to proof copy exists
	 *  Proof-of-Spacetime -> node has to show within certain time period  data is still stored
* In this case if node wants to cheat and erase the file, blockchain gets it and punishes that node.

3- Decentrality 
*  The more nodes in different geographical locations hold the file, the more secure and reliable the network is.
* Decentralization prevents a single provider's dominance, data censorship, and and DDos attacks.
	* ex: 
		* If there is only 10 servers for saving data and all of them are in one country -> government can easily cut the access
		* But if there is thousands of node on different countries - possibility of censorship is almost zero 

4- Consensus 
* Infrastructure blockchain has have mechanism to all nodes agree who save which data.
* Consensus prevents cheating.
	* example: 
		* In file coin PoST(Proof-of-Spacetime) and consensus of all network guarantees to everyone data is really saves.
			* This part is important cause if consensus do not works correctly, nodes can claim "we save data" while they not.



### What is IPFS(InterPlanetary File System)
IPFS is a set of building blocks for a better web. Open protocols to make your data smarter: content-addressed, verifiable, and unstoppable.

#### Main features of IPFS

1- Content-address
* In current internet files known by (URL/Domain) -> `https://example.com/file.png`
* In IPFS files known by their contents(Hash) -> `QmXyz...`

2- Verifiable:
* Cause address is the hash of content -> when you download a file you are sure the content its not change

3- Unstoppable
* Cause data does not saves on specific server, it distributed among thousands of nodes
* Even one server or some countries censored the data, it still exists on another nodes


#### IPFS has 3 main layers

1- Addressing: data get address by hash not location.
2- Routing: P2P network knows each data saves on which node.
3- Transferring: Data directly exchanges between nodes without need any centralize server

[[output (8).png]]

