# ChainNode – AI-Based Blockchain Fraud Detection System

## Overview

ChainNode is a Python-based blockchain system developed to demonstrate a secure and practical blockchain network with integrated fraud detection capabilities.

The project combines blockchain fundamentals, cryptographic wallets, transaction verification, Proof-of-Work mining, peer-to-peer networking, persistent storage, and AI-assisted fraud detection into a single web-based platform.

## Key Features

- Blockchain creation and validation
- SHA-256 block hashing
- Previous-hash based block linking
- Proof-of-Work mining
- Configurable mining difficulty
- ECDSA SECP256K1 wallets
- Public/private key generation
- Digitally signed transactions
- Transaction verification
- Wallet balance management
- Manual wallet funding
- Transaction history
- Wallet name and wallet hash identification
- Mempool for pending transactions
- Persistent blockchain storage
- Peer-to-peer network communication
- Blockchain synchronization between nodes
- Fraud detection system
- Suspicious wallet detection and blacklisting
- AI/ML-assisted transaction risk analysis
- Web-based blockchain dashboard
- REST API
- Blockchain explorer
- Analytics and fraud monitoring

## System Architecture

The system is organized into several major components:

```text
                    ┌─────────────────────┐
                    │    Web Dashboard    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     REST API        │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              ▼                ▼                ▼
       ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
       │   Wallets   │  │ Transactions│  │ Fraud       │
       │             │  │             │  │ Detection   │
       └──────┬──────┘  └──────┬──────┘  └──────┬──────┘
              │                │                │
              └────────────────┼────────────────┘
                               ▼
                    ┌─────────────────────┐
                    │     Blockchain      │
                    └──────────┬──────────┘
                               │
                 ┌─────────────┴─────────────┐
                 ▼                           ▼
          ┌─────────────┐             ┌─────────────┐
          │   Mining    │             │ P2P Network │
          └─────────────┘             └─────────────┘
