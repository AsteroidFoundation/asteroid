<p align="center">
  <img src="logo.png" width="150" height="150" alt="ASTEROID (ASTRO)"/>
</p>

<h1 align="center">ASTEROID (ASTRO)</h1>

<p align="center">
  The first Shiba in space — now on its own blockchain. 42, 69, and a whole lot of luck.
</p>

---

## The Story Behind ASTEROID

Asteroid Shiba is the **first Shiba Inu to travel to space**, launched aboard a SpaceX rocket alongside the Polaris astronauts — traveling the farthest distance from Earth ever recorded in human history.

The story begins with **Liv Perrotto**, a passionate space enthusiast who can recount every rocket mission by heart. After surviving cancer in 2021, Liv was inspired by Hayley Arceneaux — a fellow cancer survivor turned astronaut. Liv was invited by the Polaris Program to design the **zero-gravity indicator**: a Shiba Inu plush named **Asteroid Shiba**, inspired by Elon Musk's own Shiba, Floki.

During SpaceX's live broadcast of the first-ever commercial spacewalk, Asteroid Shiba was featured prominently. The design and its story were shared with millions of viewers worldwide. Asteroid Shiba plushies are available for purchase at the official SpaceX and Polaris Program stores, with **all proceeds donated to St. Jude Children's Research Hospital**.

Liv's message to the world: *"If Asteroid Shiba can go to space, so can they. Everyone should chase their own dreams."*

**ASTEROID** carries that spirit forward — a blockchain born from the cosmos, where every block reward is **lucky**, because space is full of surprises.

---

## Key Specs

| Parameter | Value |
|-----------|-------|
| **Algorithm** | Scrypt |
| **Block Time** | 60 seconds |
| **Total Supply** | 42,069,000,000 ASTRO (42.069 billion, hard cap) |
| **Reward Type** | Lucky v2 (random per block + jackpot tiers via Mersenne Twister) |
| **Difficulty Adjustment** | Every 20 blocks (pre-Digishield) → every block after block 50,000 (Digishield) |
| **Merge Mining** | Supported (AuxPoW) |
| **Genesis** | 2026 |

## Lucky Block Rewards v2

Block rewards are **not fixed** — they're randomized within a range using the previous block's hash as a seed, ensuring deterministic but unpredictable rewards. Every block is a lucky draw, and special blocks hit **jackpots**.

### Emission Schedule

| Era | Block Range | Base Reward (ASTRO) | Lucky Range (ASTRO) | Blocks | Duration | Avg Emission | % |
|-----|-------------|---------------------|---------------------|--------|----------|-------------|---|
| 1 | 0 — 144,999 | 69,420 | 34,710 — 104,130 | 145K | ~101 days | 10.07B | 28.7% |
| 2 | 145,000 — 564,999 | 42,069 | 21,034 — 63,103 | 420K | ~292 days | 17.67B | 50.3% |
| 3 | 565,000 — 1,254,999 | 6,942 | 3,471 — 10,413 | 690K | ~479 days | 4.79B | 13.6% |
| 4 | 1,255,000 — 2,944,999 | 1,337 | 668 — 2,005 | 1,690K | ~1,174 days | 2.26B | 6.4% |
| 5 | 2,945,000 — 5,654,999 | 420 | 210 — 630 | 2,710K | ~1,882 days | 1.14B | 3.2% |
| 6 | 5,655,000 — 8,364,999 | 69 | 34 — 103 | 2,710K | ~1,882 days | 187M | 0.5% |
| 7 | 8,365,000 — 11,109,999 | 4 | 2 — 6 | 2,745K | ~1,906 days | 11M | 0.03% |
| 8 | 11,110,000+ | 0 | — | ∞ | perpetual | 0 | — |

**Total average emission: ~36.1B ASTRO** across ~11.1M blocks (~21 years).

### Jackpot Tiers

Special blocks receive multiplied rewards based on their block height:

| Tier | Trigger | Multiplier | Approx. Frequency |
|------|---------|------------|-------------------|
| **Mega Jackpot** | Every 69,420 blocks | ×69 | ~every 48 days |
| **Mini Jackpot** | Every 4,206 blocks | ×42 | ~every 3 days |
| **Lucky Strike** | Every 420 blocks | ×21 | ~every 7 hours |

Example: At Era 1 (base 69,420), a **Mega Jackpot** block yields **2.4M — 7.2M ASTRO** instead of the normal 34,710 — 104,130.

> Every number tells a story: **42**, **69**, **420**, **1,337**, **4,206**, **69,420** — meme math all the way down.

## Difficulty Adjustment

- **Block 0 — 49,999**: Retarget every 20 blocks (~20 minutes), standard Bitcoin-style
- **Block 50,000+**: Digishield activated — difficulty adjusts **every single block**, providing rapid response to hashrate changes and protection against attacks

## Network Ports

| Network | P2P Port | RPC Port |
|---------|----------|----------|
| Mainnet | 9333 | 9332 |
| Testnet | 19333 | 19332 |
| Regtest | 29333 | 29332 |

## Address Format

Mainnet addresses start with **`A`** (prefix byte 23), so your wallet address will look like `A...`

## Building from Source

See [INSTALL.md](INSTALL.md) for detailed build instructions.

### Quick Start (Linux)

```bash
# Dependencies
sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils python3 libboost-all-dev libminiupnpc-dev libzmq3-dev

# Build
./autogen.sh
./configure
make -j$(nproc)

# Run
./src/asteroidd
./src/asteroid-cli getblockchaininfo
```

## License

ASTEROID is released under the terms of the MIT license. See [COPYING](COPYING) for more information.

---

<p align="center">
  <strong>ASTEROID</strong> — If a Shiba can go to space, so can you. 🚀
</p>
