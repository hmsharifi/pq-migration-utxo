# pq-migration-utxo
Implementation of the post-quantum wallet migration protocol for UTXO blockchains without address change (ML-DSA, SNARKs).
# PQ Migration UTXO

Implementation of the post-quantum wallet migration protocol for UTXO blockchains without address change.

## Paper

This repository contains the reference implementation for the paper:  
**"A Post-Quantum Wallet Migration Protocol for UTXO Blockchains without Address Change"**  
(S. L. Hosseini, H. Sharifi – Shahed University, Iran)

## Protocol Overview

The protocol enables users to migrate UTXO-based cryptocurrency funds (e.g., Bitcoin) from legacy ECDSA keys to post-quantum ML-DSA (CRYSTALS-Dilithium) keys without changing their wallet address. It combines:

- **Commit-reveal mechanism** to prevent mempool race attacks
- **Hash-based SNARK** (Poseidon + Spartan) for zero-knowledge proof of ownership
- **ML-DSA** (FIPS 204) for post-quantum signatures

## Repository Structure

## Requirements

- Rust 1.85+
- liboqs 0.12.0
- arkworks 0.4.0

## License

Apache 2.0
