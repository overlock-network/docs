---
id: intro
slug: /
title: Welcome to Overlock Network
sidebar_position: 0
sidebar_label: 'Introduction'
---

# 🌐 Welcome to Overlock Network

**Overlock Network** is a decentralized system for managing external infrastructure through distributed execution.  
It is built with the [**Cosmos SDK**](https://cosmos.network/appchains/) and extends the control plane model using [**Crossplane**](https://crossplane.io) .

In Overlock Network, Active Resources are on-chain definitions that tell provider-hosted controllers how to create and manage infrastructure in cloud and edge environments.
As a result, Overlock Network can coordinate infrastructure on platforms such as GCP, AWS, Azure, Akash, DigitalOcean, and others.

---

## 🧱 Core Concepts

The network is centered around a small number of composable, on-chain objects:

- **Active Resources**  
  Describe the infrastructure or services to be created and managed externally.

- [**Configuration NFTs**](./overview/nft-config)  
  Represent access to reusable infrastructure definitions (similar to a configuration library). 

- [**Gas NFTs**](./overview/nft-gas)
  Store a balance of execution tokens, which are gradually consumed as infrastructure operations are performed. 

---


## 🌍 Distributed Providers

Overlock does not run infrastructure itself.  
Instead, it relies on an open set of **independent providers** who run trusted execution environments and Crossplane-based controllers.  
These providers process on-chain requests, access cloud APIs, and consume gas as work is completed.

Each interaction is tied to ownership:  
- users retain control through NFTs and token balances  
- providers receive compensation through gas consumption

---

## 🧩 Modularity and Extensibility

Overlock is designed to support many use cases:
- cloud automation
- edge orchestration
- multi-provider workflows
- agent-based infrastructure management

Its primitives — Active Resources, Configuration NFTs, and Gas NFTs — can be extended or composed to support increasingly complex systems and tooling.

---

Overlock Network provides a programmable and verifiable way to control external infrastructure — with ownership and automation at its core.