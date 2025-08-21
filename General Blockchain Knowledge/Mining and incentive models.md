
Mining is the process of adding transaction details to the Blockchain, like sender address, hash value, etc. The Blockchain contains all the history of the transactions that have taken place in the past for record purposes and it is stored in such a manner that, it can’t be manipulated.

An Incentive is basically a reward given to a Blockchain Miner for speeding up the transactions and making correct decisions while processing the complete transaction securely.

# Consensus mechanisms

The term 'consensus mechanism' is often used colloquially to refer to 'proof-of-stake', 'proof-of-work' or 'proof-of-authority' protocols. However, these are just components in consensus mechanisms that protect against Sybil attacks. Consensus mechanisms are the complete stack of ideas, protocols and incentives that enable a distributed set of nodes to agree on the state of a blockchain.

## What is consensus

By consensus, we mean that a general agreement has been reached. Consider a group of people going to the cinema. If there is no disagreement on a proposed choice of film, then a consensus is achieved. If there is disagreement, the group must have the means to decide which film to see. In extreme cases, the group will eventually split.

In regard to the Ethereum blockchain, the process is formalized, and reaching consensus means that at least 66% of the nodes on the network agree on the global state of the network.


## What is consensus mechanism?

The term consensus mechanism refers to the entire stack of protocols, incentives and ideas that allow a network of nodes to agree on the state of a blockchain.

Ethereum uses a proof-of-stake-based consensus mechanism that derives its crypto-economic security from a set of rewards and penalties applied to capital locked by stakers. This incentive structure encourages individual stakers to operate honest validators, punishes those who don't, and creates an extremely high cost to attack the network.

Then, there is a protocol that governs how honest validators are selected to propose or validate blocks, process transactions and vote for their view of the head of the chain. In the rare situations where multiple blocks are in the same position near the head of the chain, there is a fork-choice mechanism that selects blocks that make up the 'heaviest' chain, measured by the number of validators that voted for the blocks weighted by their staked ether balance.

Some concepts are important to consensus that are not explicitly defined in code, such as the additional security offered by potential out-of-band social coordination as a last line of defense against attacks on the network.

These components together form the consensus mechanism.

## Types of consensus mechanisms

### Proof-of-work based

Like Bitcoin, Ethereum once used a **proof-of-work (PoW)** based consensus protocol.

#### Block creation

Miners compete to create new blocks filled with processed transactions. The winner shares the new block with the rest of the network and earns some freshly minted ETH. The race is won by the computer which is able to solve a math puzzle fastest. This produces the cryptographic link between the current block and the block that went before. Solving this puzzle is the work in "proof-of-work". The canonical chain is then determined by a fork-choice rule that selects the set of blocks that have had the most work done to mine them.

#### Security

The network is kept secure by the fact that you'd need 51% of the network's computing power to defraud the chain. This would require such huge investments in equipment and energy; you're likely to spend more than you'd gain.

### Proof-of-stake based
Ethereum now uses a **proof-of-stake (PoS)** based consensus protocol.

#### Block creation

Validators create blocks. One validator is randomly selected in each slot to be the block proposer. Their consensus client requests a bundle of transactions as an 'execution payload' from their paired execution client. They wrap this in consensus data to form a block, which they send to other nodes on the Ethereum network. This block production is rewarded in ETH. In rare cases when multiple possible blocks exist for a single slot, or nodes hear about blocks at different times, the fork choice algorithm picks the block that forms the chain with the greatest weight of attestations (where weight is the number of validators attesting scaled by their ETH balance).

#### Security

A proof-of-stake system is secure crypto-economically because an attacker attempting to take control of the chain must destroy a massive amount of ETH. A system of rewards incentivizes individual stakers to behave honestly, and penalties disincentivize stakers from acting maliciously.

[[output (3).png]]


