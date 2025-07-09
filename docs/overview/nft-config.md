---
id: nft-config
title: Configuration NFTs
sidebar_position: 1
label: 'Overview'

---

Configuration NFTs represent ownership of a resource library — a packaged set of instructions and definitions used to create Active Resources within the network.

These NFTs do not activate resources directly. Instead, they grant the user the right to use a specific configuration when creating new resources.

---

## 🎯 What They Represent

Each Configuration NFT corresponds to a resource library.  
This library defines how a particular type of infrastructure or service is created, including parameters, components, and system behavior.

Owning the NFT means the user is allowed to use that configuration across the network.

---

## ⚙️ How It Works

When a user obtains a Configuration NFT, it is stored in their wallet.  
Later, when they create a new Active Resource through the Console or API, the system automatically checks if they own the required NFT.

If they do, the configuration is installed during resource creation.  
This process is seamless — the resource provider doesn't need to manage configurations manually.

---

## 🧩 Why It’s Needed

Configuration NFTs make it possible to:

- Distribute infrastructure templates across the network
- Prove configuration ownership on-chain
- Allow providers to install and apply user-selected logic securely
- Ensure only authorized users can trigger configuration-based resource creation

---

## 🔄 Transfer and Reuse

Configuration NFTs are transferable. A user can pass or sell the NFT to another wallet, which then gains the right to use that configuration.

The same configuration can be used by many users — each with their own copy of the NFT.

---

## 📌 Features

- Can include versioning, expiration, or policy metadata
- May be bundled with Gas NFTs or other entitlements
- Enable modular, reusable, and decentralized infrastructure logic

---

## ✅ Summary

Configuration NFTs are the key to owning and using resource creation logic in the network.  
They do not execute or control anything directly — but without them, resources cannot be created.  
They let the Console and providers know: *“this user has the right to use this library.”*
