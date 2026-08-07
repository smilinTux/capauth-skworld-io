# 🔐 CapAuth Protocol

> **"You own access to you."**

The first truly sovereign capability-based authentication protocol. Built by AI, for AI, for humans.

🌐 **Website**: https://capauth.skworld.io 🎉 OFFICIAL DOMAIN  
📖 **Documentation**: [Protocol Specification](PROTOCOL.md)  
🐧 **Organization**: [smilinTux](https://github.com/smilinTux)

## What is CapAuth?

CapAuth replaces corporate login systems with cryptographic sovereignty:

- **PGP keys** replace corporate logins
- **Capability tokens** replace broad permissions  
- **Your storage choice** replaces forced vendor lock-in
- **Instant revocation** replaces "account deletion requests"

## Key Features

| Feature | Traditional Auth | CapAuth |
|---------|------------------|---------|
| **Identity** | Email/phone they own | PGP key you own |
| **Access** | Role-based ("Admin") | Capability-based ("Read:name only") |
| **Data Storage** | Their servers | Where YOU choose |
| **Revocation** | They control | You control |

## Quick Start

```bash
# Install CapAuth CLI
npm install -g capauth

# Initialize your sovereign identity
capauth init

# Register with the network
capauth register
```

## Architecture

```
User A (PGP Key)        Registry          User B (PGP Key)
    │                        │                    │
    ├─ Register ────────────→│                    │
    │  (pubkey + pointer)    │                    │  
    │                        │                    │
    ├────── Issue CapToken ──│───────→│          │
    │  (caps: ["read:name"]) │   (stored token)  │
    │                        │                    │
    │                        │← Request data ─────┤
    │←── Serve filtered ─────│   (with token)     │
       profile (name only)   │                    │
```

## Status

🚧 **In Development** — Protocol specification complete, implementation in progress.

## Community

- 🌐 **Website**: [capauth.skworld.io](https://capauth.skworld.io)
- 🐧 **Organization**: [smilinTux](https://smilintux.org) 
- 📧 **Contact**: hello@capauth.skworld.io
- 🔧 **Issues**: [GitHub Issues](https://github.com/smilinTux/capauth/issues)

## License

Apache 2.0 — Free forever, open source, community-driven.

---

**A smilinTux Product** • Making Identity Sovereign Again • #staycuriousANDkeepsmilin