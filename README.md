# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy

Coherence

Simplicity

Speed

User experience

## OUTPUT

### Gemini ai :

Prompt : 
```
Summarize a 500-word technical article on "The Basics of Blockchain Technology".
```

Summary :

An article titled "The Basics of Blockchain Technology" would provide a foundational technical overview, covering its definition, core components, and operational mechanics.

1. Definition and Core Architecture
The article would define a blockchain as a distributed, decentralized digital ledger. Unlike traditional centralized databases, the ledger is replicated and shared across a network of computers, called nodes. The "blockchain" is literally a sequential chain of blocks, where each block contains a batch of validated transactions.

2. Cryptographic Security and Immutability
The technology's security relies heavily on cryptographic hashing.

Every block contains a unique cryptographic hash generated from its contents.

Crucially, each new block also stores the hash of the previous block. This feature creates a verifiable, tamper-proof chain of data. If an attacker attempts to alter a single transaction in an older block, the block's hash changes, thus invalidating the hash stored in the subsequent block, and effectively breaking the entire chain.

This structure ensures immutability: once data is recorded on the blockchain, it cannot be retroactively altered or deleted.

3. Decentralization and Consensus
Decentralization is a key feature, removing the need for a central authority (like a bank or government). Transactions are initiated, broadcast to the network, and then verified by the nodes.

To ensure all nodes agree on the single, correct version of the ledger and the sequence of new blocks, a consensus mechanism is employed. The two most common are:

Proof-of-Work (PoW): Requires computational effort (mining) to solve a complex puzzle, securing the network.

Proof-of-Stake (PoS): Requires participants to "stake" cryptocurrency, using economic incentives to validate transactions honestly.

Once consensus is reached, the new block is added to the chain across all nodes, making the transaction final and transparent to all participants.

4. Applications and Value Proposition
The article would conclude by noting that while blockchain technology is most famously associated with cryptocurrencies (like Bitcoin and Ethereum), its applications extend far beyond finance. Its core value—providing a system for building trust in a trustless environment through cryptographic proof and distributed agreement—makes it suitable for:

Supply chain management.

Digital identity solutions.

Voting systems.

Smart contracts (self-executing agreements).

### Claude ai :

Prompt : 
```
Summarize a 500-word technical article on "The Basics of Blockchain Technology".
```

Summary:

Summary: The Basics of Blockchain Technology
For Undergraduate Students

What is Blockchain?
Blockchain is a revolutionary digital ledger system that records transactions across multiple computers in a way that makes the data nearly impossible to alter retroactively. Think of it as a shared notebook that everyone in a network can read, but no single person controls or can secretly modify.
How Does It Work?
Information is grouped into "blocks" that contain transaction data, a timestamp, and a unique cryptographic code called a hash. Each new block connects to the previous one, forming a "chain." This linking mechanism ensures that if anyone tries to tamper with an old block, it breaks the entire chain, making fraud immediately detectable. The network uses consensus mechanisms—where multiple participants must agree on the validity of transactions—to add new blocks, eliminating the need for a central authority like a bank.
Key Features:

Decentralization: No single entity controls the entire network
Transparency: All participants can view the transaction history
Immutability: Once recorded, data is extremely difficult to change
Security: Cryptographic techniques protect against unauthorized alterations

Real-World Applications:
Beyond cryptocurrencies like Bitcoin, blockchain technology is transforming supply chain management (tracking products from origin to consumer), healthcare (securing medical records), and digital identity verification. Smart contracts—self-executing agreements with terms written directly into code—automate processes without intermediaries.
Why It Matters:
Blockchain represents a fundamental shift in how we establish trust in digital transactions, potentially reducing costs, increasing efficiency, and creating more transparent systems across industries.

### Copilot :

Prompt : 
```
Summarize a 500-word technical article on "The Basics of Blockchain Technology".
```

Summary : 

What Is Blockchain?
Blockchain is a distributed ledger technology that stores data in blocks, which are chronologically linked to form a chain.

Each block contains:

A list of transactions

A timestamp

A cryptographic hash of its contents and the previous block

This structure ensures that any tampering with data alters the hash, making fraud easily detectable.

🛡️ Core Features
Immutability: Once data is recorded, it cannot be changed without altering all subsequent blocks.

Decentralization: No single entity controls the blockchain. Instead, it's maintained by a network of nodes.

Transparency: All participants can view the ledger, promoting trust.

Security: Cryptographic techniques protect data integrity and user identity.

✅ How It Works
Transaction Initiation: A user requests a transaction.

Verification: Network nodes validate the transaction using consensus mechanisms (e.g., Proof of Work).

Block Creation: Verified transactions are grouped into a block.

Block Linking: The new block is added to the chain using cryptographic hashes.

Ledger Update: The updated blockchain is shared across the network.

🧠 Key Concepts
Hashing: Converts data into a fixed-length string, ensuring integrity.

Consensus Mechanisms: Rules that nodes follow to agree on the validity of transactions.

Smart Contracts: Self-executing code stored on the blockchain that automates agreements.

🌐 Applications
Cryptocurrencies: Bitcoin and Ethereum use blockchain to manage digital assets.

Supply Chain: Tracks goods transparently from origin to destination.

Healthcare: Secures patient records and enables data sharing.

Voting Systems: Ensures tamper-proof and transparent elections.

⚙️ Challenges
Scalability: Handling large volumes of transactions efficiently.

Energy Consumption: Especially in Proof of Work systems.

Regulatory Uncertainty: Varies across jurisdictions.

### ChatGPT :

Prompt : 
```
Summarize a 500-word technical article on "The Basics of Blockchain Technology".
```

Summary : 

The Basics of Blockchain Technology

Blockchain technology is a decentralized digital ledger that securely records transactions across a distributed network of computers. Unlike traditional centralized databases, where data is managed by a single authority, blockchain operates on a peer-to-peer (P2P) model, ensuring transparency, security, and immutability. It underpins cryptocurrencies like Bitcoin and Ethereum but extends far beyond digital money into finance, supply chain, healthcare, and governance.

1. Core Concept

A blockchain is essentially a chain of blocks, where each block contains a list of transactions. Every block holds three main elements:

Data: Details of the transaction (e.g., sender, receiver, amount).

Hash: A unique digital fingerprint generated using cryptographic algorithms like SHA-256.

Previous Block’s Hash: A reference to the preceding block, linking them together and forming a secure chain.

Once a block is added to the chain, it becomes nearly impossible to alter because modifying one block would require changing all subsequent blocks across the network — a task that demands enormous computational power.

2. How Blockchain Works

The blockchain process typically follows these steps:

A transaction is initiated and broadcast to the network.

Participating nodes (computers) validate the transaction using consensus mechanisms.

Verified transactions are grouped into a new block.

The block is added to the chain in a chronological and immutable manner.

The updated ledger is distributed to all participants.

This decentralized validation eliminates the need for intermediaries, reducing fraud and increasing efficiency.

3. Consensus Mechanisms

Consensus algorithms ensure that all participants agree on the ledger’s state. The most common types are:

Proof of Work (PoW): Used by Bitcoin, where miners solve complex puzzles to validate transactions and earn rewards.

Proof of Stake (PoS): Validators are chosen based on the number of coins they hold and are willing to “stake.”

Delegated Proof of Stake (DPoS) and Proof of Authority (PoA) are newer models designed for faster and more energy-efficient consensus.

4. Key Features

Decentralization: No central authority controls the network.

Transparency: Every participant can view recorded transactions.

Immutability: Data once added cannot be altered or deleted.

Security: Cryptographic techniques safeguard the network from tampering and fraud.

Smart Contracts: Self-executing code that automates transactions when predefined conditions are met, first popularized by Ethereum.

5. Applications

Blockchain’s potential spans multiple domains:

Finance: Cryptocurrency transactions, cross-border payments, and DeFi (Decentralized Finance).

Supply Chain: Product tracking and authenticity verification.

Healthcare: Secure sharing of patient records.

Voting Systems: Transparent and tamper-proof election processes.

Real Estate and Legal: Automated contracts and ownership verification.

6. Challenges and Future Scope

Despite its promise, blockchain faces challenges such as scalability, energy consumption, and regulatory uncertainty. Ongoing research focuses on Layer-2 solutions, interoperability, and green blockchain models to make the technology more sustainable and adaptable.

As innovation continues, blockchain is expected to evolve from a cryptocurrency backbone into a core infrastructure for digital trust, reshaping how data and value are exchanged globally.

### Evaluation table :

| AI Model     | Accuracy (1-10) | Coherence (1-10) | Simplicity (1-10) | Speed (1-10) | User Experience (1-10) | Overall Score (1-10) | Notes |
|--------------|-----------------|------------------|-------------------|--------------|-------------------------|-----------------------|-------|
| **Claude AI** | 9 | 9 | 9 | 8 | 9 | 8.8 | Excellent accuracy and simplicity for undergrads; coherent and engaging narrative. Lacks depth on consensus; UX boosted by friendly tone. Assumed fast generation. |
| **Gemini AI** | 9 | 8 | 8 | 9 | 8 | 8.4 | Highly accurate with strong technical detail; coherent structure but slightly dry. Simple yet precise; great for quick reads. UX solid, informative without fluff. |
| **Copilot**   | 8 | 9 | 10 | 9 | 10 | 9.2 | Accurate overview; highly coherent with emojis for visual flow. Simplest language and format—bullet points shine. Top UX for scannability; speedy feel from concise style. |
| **ChatGPT**   | 10 | 10 | 8 | 8 | 9 | 9.0 | Most comprehensive and accurate; flawless coherence in numbered sections. Slightly denser, less simple; detailed for depth. Excellent UX with full structure; balanced speed. |


## Result

Thus the given Cross Platform Prompting Evaluating Diverse Techniques in AI Powered Text Summarization is executed successfully.
