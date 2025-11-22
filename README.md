# Blockchain Engineering Masterclass

**The complete source code for the "Engineering a Blockchain from Scratch" series.**

This repository contains the production-grade implementation of a custom blockchain, evolved from a TypeScript Monorepo (Phase 1) to a High-Performance Go Backend (Phase 2), and finally to a Rust-based System Architecture (Phase 3).

## The Grand Vision

We are not just building a toy blockchain. We are embarking on a comprehensive journey through the history and future of distributed systems. This course is designed to take you from a "User" of libraries to a **Protocol Architect**.

**Our Philosophy:**
*   **Chain Agnostic:** We learn **Architecture**, not just Syntax.
*   **Evolutionary Stack:** We don't just switch languages; we evolve the architecture based on the strengths of each stack (TS for Prototyping, Go for Concurrency, Rust for System Safety).
*   **Enterprise Grade:** We build with Monorepos, Docker, Kubernetes, and clean Domain-Driven Design from Day 1.

## What You Will Build & Understand

By the end of this masterclass, you will have engineered a system featuring:

1.  **Core Node (NestJS -> Go):** A modular blockchain node capable of mining, validating, and syncing blocks.
2.  **The Data Trinity:** A hybrid storage strategy using **LevelDB** (Ledger), **Redis** (Mempool), and **Postgres** (Indexer).
3.  **P2P Networking:** A decentralized gossip protocol using WebSockets and LibP2P.
4.  **Consensus Engines:**
    *   **Proof of Work (PoW):** Understanding Hashing, Difficulty, and Nonces.
    *   **Proof of Authority (PoA):** Implementing a basic "Authority Round" with trusted signers.
    *   **Proof of Stake (PoS):** Implementing Validators, Staking, and Slashing.
    *   **Delegated Proof of Stake (DPoS):** Voting mechanics and "Super Representatives" (BSC/EOS style).
    *   **BFT & Instant Finality:** Implementing Tendermint-style 3-phase commit (Cosmos).
    *   **Federated Byzantine Agreement (FBA):** Trust-based consensus (Stellar/XRP).
    *   **Hybrid Consensus:** Separating Block Production from Finality (Polkadot BABE/GRANDPA).
    *   **Avalanche:** Metastable consensus using random subsampling.
    *   **Proof of History (PoH):** Implementing Solana's verifiable delay function (VDF).
    *   **Non-Linear Consensus:** Building DAGs and Hashgraphs (Hedera/IOTA style).
5.  **The Explorer:** A professional dashboard using **Next.js 14** and **shadcn/ui** to visualize the ledger.
6.  **System Level Primitives (Rust):** Writing WASM modules and high-performance cryptographic primitives.

## Course Roadmap

### Phase 1: The Foundation (TypeScript Monorepo)
*   **Focus:** Architecture, Domain-Driven Design, and the basic "Bitcoin-like" mechanics.
*   **Tech:** NestJS, Docker, LevelDB.

### Phase 2: High Performance (The Go Migration)
*   **Focus:** Concurrency, handling 10k+ connections, and migrating to Proof-of-Stake (Delegated).
*   **Tech:** Go (Golang), Fiber, Goroutines.

### Phase 3: The System Level (Rust & WASM)
*   **Focus:** Memory safety, WebAssembly integration, and L2 Scaling (Rollups).
*   **Tech:** Rust, Arbitrum Stylus, Solana Architecture (PoH).

### Phase 4: The Frontier (Research & Beyond)
*   **Focus:** Zero-Knowledge Proofs, DAGs, Hashgraphs, and Account Abstraction.
*   **Tech:** Circom, SnarkJS, Graph Structures.

## Getting Started

### Prerequisites
- Node.js v20+
- Docker & Docker Compose
- pnpm (npm install -g pnpm)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/edsphinx/blockchain-engineering-masterclass.git
    cd blockchain-engineering-masterclass
    ```

2.  **Install dependencies:**
    ```bash
    pnpm install
    ```

3.  **Run the infrastructure:**
    ```bash
    docker-compose up -d
    ```

4.  **Start the development server:**
    ```bash
    pnpm dev
    ```

## Student?
If you are following the course, **DO NOT** clone this repository to start.
Use the **Starter Repository** or the **GitHub Classroom Link** provided in the lessons to build your own version from scratch.

*   [Start Here (Course Link)](https://paragraph.com/@edsphinx)
*   [Starter Repository](https://github.com/edsphinx/blockchain-engineering-masterclass-starter)

## License
MIT
