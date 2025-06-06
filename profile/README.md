# 🐮 OpenHerd

**OpenHerd** is a decentralized, anonymous, and location-based communication platform. It’s built for people who want to talk without being tracked, post without an account, and speak locally, even when centralized services are down, blocked, or untrustworthy.

No servers. No sign-ups. No surveillance.

## ✨ What It Does

- 📍 **Hyperlocal posts** — Messages are tied to coordinates, like an anonymous Yik Yak over mesh or Wi-Fi.
- 🔒 **End-to-end anonymous** — Each post uses a fresh PGP key, with no persistent identity.
- 📡 **P2P-first** — Uses [libp2p](https://libp2p.io) for decentralized pubsub and direct connections.
- 📁 **Relays and Dead Drops** — Lightweight HTTP-only nodes (relays) can store posts without needing libp2p.
- 🌐 **Beacon Network** — Relays can optionally register to a global directory for discoverability.
- 🔄 **Offline-first sync** — Devices can sync messages directly or through relays, even without internet.


## 🧩 Components

| 🧩 **Project**                                   | 📝 **Description**                                                                                                                                             |
| ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`pasture`](https://github.com/openherd/pasture) | **Full-featured OpenHerd client** written in Node.js. Handles post creation, syncing, libp2p comms, and more. Think of it as the Swiss Army knife of the herd. |
| [`relay`](https://github.com/openherd/relay)     | **Minimal HTTP relay server** for low-resource deployments. Great for Raspberry Pis, dead drops, or public mesh networks. No libp2p required.                  |
| [`beacon`](https://github.com/openherd/beacon)   | **Public directory for relays.** Relays can advertise themselves here (with optional PoW) for global discovery and indexing.                                   |
| [`meadow`](https://github.com/openherd/meadow)   | **A full PWA OpenHerd client** that runs entirely in the browser. No install, no backend, just one pure decentralized application.                                       |
| [`sprout`](https://github.com/openherd/sprout) | **MicroPython version of `relay`** designed for very constrained devices. It works and makes necessary compromises, but it's currently in **alpha** and not ready for production. |
| [`spec`](https://github.com/openherd/spec)       | 📜 **The full protocol specification.** Covers everything from message formats to chunking, PGP signing, and sync logic. The source of truth.                  |


## 🏴 Our Mission

> **To create a censorship-resistant, identity-optional, and geographically local communication layer that anyone can deploy and trust, even in hostile or disconnected environments.**

We believe in freedom of expression, anonymity by default, and communication systems that don’t depend on trust in corporate gatekeepers.

## 👩‍💻 Contribute

Pull requests are welcome across all repos!  
You can also open issues, propose enhancements, or help build out reference clients and interfaces.

## 🐾 Join the Herd

OpenHerd is still early and experimental, but that’s what makes it fun. Come help us build the future of offline-first, decentralized communication.
