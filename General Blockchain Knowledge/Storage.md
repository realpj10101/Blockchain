 
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


### How IPFS represents and addresses data

IPFS represents data as content-addressed blocks, and operates on those data blocks using the following subsystems:

- Content Identifier (CID)
- InterPlanetary Linked Data (IPLD)
- Content Addressable aRchive (CAR) files

#### Content Identifier (CID)

In IPFS, data is chunked into blocks, which are assigned a unique identifier called a Content Identifier (CID). In general, the CID is computed by combining the hash of the data with its codec. The codec is generated using Multiformats.

CIDs are unique to the data from which they were computed, which provides IPFS with the following benefits:

- Data can be fetched based on its content, rather than its location.
- The CID of the data received can be computed and compared to the CID requested, to verify that the data is what was requested.

Codec -> Specifies what type the data is (JSON, image, vidoe )

**CID = Hash + Codec**

##### Features and benefits of (CID)

1- Content-based addressing 
* On regular on internet: File calls by location address (URL)
* On IPFS: File calls by **CID** -> Its not important where the file is, You can find it wherever it is

2- Verification
* When you get the file -> hash of that data computes again
* If CID = Wanted hash -> data is not changed

####  InterPlanetary Linked Data (IPLD)

IPFS uses InterPlanetary Linked Data (IPLD) to work with CIDs and content-addressed data. IPFS uses IPLD to represent relationships between content-addressed data, such as file directories and other hierarchical structures, using a Directed Acyclic Graph (DAG) called a Merkle DAG. Using IPLD for the general functionality, IPFS is able provide a more tailored, specific mechanism for representing and addressing files, directories, and their symlinks, called [UnixFS](https://docs.ipfs.tech/concepts/file-systems/#unix-file-system-unixfs). With UnixFS, IPFS can chunk and link data too big to fit in a single block, and use the chunked representation to store and manage the data.

IPLD provides IPFS with the following benefits:

- The ability to represent and work with arbitrary data, whether that data is standard files and directories, linked data, a Merkle DAG, or another data type.
- Base functionality to structure, serialize, traverse and link content-addressed data, which can be leveraged by abstractions like UnixFS for more specific use cases.
- Interoperable protocols.
- Easy upgradeability.
- Backwards compatibility.

#### Content Addressable aRchive (CAR) files

IPFS uses Content Addressable aRchive (CAR) files to store and transfer a serialized archive of IPLD content-addressed data. CAR files are similar to TAR files, in that they that are designed for storing collections of content addressed data.

### How content routing works in IPFS

_Content routing_ refers to the way in which IPFS determines where to find a given CID on the network; specifically, which network peers are providing the CIDs you are requesting. In other words, a node cannot simply find data in the network with a CID alone; it requires information about the IP addresses and ports of its peers on the network. To route content, IPFS uses the following subsystems:

- Kademlia Distributed Hash Table (DHT)
- Bitswap
- mDNS
- Delegated routing over HTTP

#### Kademlia Distributed Hash Table

IPFS uses Kademlia, a Distributed Hash Table (DHT) designed for decentralized peer-to-peer networks. Kademlia helps you find peers in the IPFS network storing the data you are seeking. The Kademlia DHT can be thought of as a large table distributed across many nodes that stores information about which peers (IPs) have which data (CIDs). Kademlia provides a highly efficient, self-organizing system that withstands node churn. Kademlia uses [libp2p](https://docs.ipfs.tech/concepts/libp2p/) to establish connectivity.

#### Bitswap (for content routing)

IPFS nodes use Bitswap, a message-based, peer-to-peer network protocol for the transfer of data, that is _also_ used for routing data. With Bitswap, an IPFS node can ask any of the peers that it is connected to if they have any of the CIDs that node is looking for, all without traversing the [Kademlia DHT](https://docs.ipfs.tech/concepts/how-ipfs-works/#kademlia-distributed-hash-table-dht). Peers also store wantlists, so that if a peer receives the requested data at a later time, it can then send it to the node that originally requested. Like Kademlia, Bitswap uses [libp2p](https://docs.ipfs.tech/concepts/libp2p/) to establish connectivity.

#### Delegated routing over HTTP

Delegated content routing is a mechanism for IPFS implementations to use for offloading content routing to another process/server using an HTTP API. For example, if an IPFS node does not implement the DHT, a delegated router can search the DHT for peers on its behalf. The main benefit of delegated routing is that nodes are not required to implement routing functionality themselves if they do not have the computing resources to do so, or wish to build an IPFS system with a custom backend for routing. So, delegated routing over HTTPS provides IPFS nodes with a standard interface that allows more flexibility in terms of how content routing works.

#### mDNS

To quickly and efficiently discover peers in local networks, IPFS uses Multicast Domain Name System (mDNS), a type of DNS protocol that resolves human-readable internet domain names to IP names without the use of a name server.

The use of mDNS enables quick and efficient discovery of IPFS nodes in local networks without any coordination, e.g., without internet connectivity or access to [bootstrap nodes](https://docs.ipfs.tech/concepts/nodes/#bootstrap).

### How IPFS transfers data

In addition to [routing data](https://docs.ipfs.tech/concepts/how-ipfs-works/#how-content-routing-works-in-ipfs), nodes in the IPFS network must efficiently distribute and deliver the content addressed data, taking into account that there are some nodes in the network who already have a copy of the data, and other nodes who do not have a copy of the data, but want one. To handle the transfer of data, IPFS uses the following subsystems:

- [Bitswap](https://docs.ipfs.tech/concepts/how-ipfs-works/#bitswap-for-data-transfer)
- [IPFS HTTP Gateways](https://docs.ipfs.tech/concepts/how-ipfs-works/#ipfs-http-gateways)
- [Sneakernet](https://docs.ipfs.tech/concepts/how-ipfs-works/#sneakernet)

#### Bitswap (for data transfer)

As discussed in [How content routing works in IPFS](https://docs.ipfs.tech/concepts/how-ipfs-works/#bitswap-for-content-routing), IPFS nodes use Bitswap, a message-based, peer-to-peer network protocol for both content routing and the transfer of data. With Bitswap, any peers that an IPFS node is connected to can transfer requested blocks directly to that node without needing to traverse the [DHT](https://docs.ipfs.tech/concepts/how-ipfs-works/#kademlia-distributed-hash-table-dht). Peers also store wantlists, so that if a peer receives requested data at a later time, it can then transfer it to the node that originally requested.

####  IPFS HTTP Gateways

HTTP Gateways allow applications that do not support or implement all IPFS subsystems to fetch data from the IPFS network using an HTTP interface. In its simplest form, a gateway is an IPFS Node that also exposes an [HTTP Gateway API (opens new window)](https://github.com/ipfs/specs/blob/main/http-gateways/README.md).

####  Sneakernet

For use cases where transfer of data over a network connection is not an option, IPFS supports the use of sneakernet to transfer content-addressed data between IPFS nodes. Using IPFS, CAR files (discussed in [How IPFS represents and addresses data](https://docs.ipfs.tech/concepts/how-ipfs-works/#content-addressable-archive-car-files)) can be transferred between two network drives without any network connectivity. Because of IPFS, the data is [verifiable](https://docs.ipfs.tech/concepts/what-is-ipfs/#verifiability) and will have the same CID on both sides of the air gap.


## Data Locations - Storage, Memory and Calldata (Solidity Code Example)

### Storage

*  Data saves on blockchain
* Permanent as long as contract stands
* It has a higher gas cost because the change is made on blockchain

```solidity
	pragma solidity ^0.8.0;
	
	contract Example {
	    uint public number; // storage (state variable)
	
	    function setNumber(uint _num) public {
	        number = _num; // نوشته شدن در storage → ذخیره روی بلاکچین
	    }
	}

```

### Memory

* The data is temporary and only exist when the function is executed
* It is destroyed after the function ends
* Low gas cost than storage

``` solidity
pragma solidity ^0.8.0;

contract Example {
    function processData(uint[] memory _data) public pure returns (uint) {
        return _data[0]; // فقط تو حافظه RAM استفاده میشه
    }
}
```


### Calldata

* Specific type of ROM for function parameters
* Data comes from out of function it cannot be change
* In term of gas more optimal than memory for parameters

```solidity
pragma solidity ^0.8.0;

contract Example {
    function getFirstElement(uint[] calldata _data) public pure returns (uint) {
        return _data[0]; // فقط خواندن از calldata، تغییر داده نمیشه
    }
}
```









