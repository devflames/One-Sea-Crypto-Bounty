# 🏴‍☠️ One Sea Crypto Bounty — Master Project Document v2
### Heroic Adventure Edition | Updated from GDD + Whitepaper
**By Albert Camings (AC) & One Sea Crypto Bounty Interactive Studio**
> *"Sail. Conquer. Earn. Awaken."*

---

## 📋 What Changed from v1 → v2

| Area | v1 (Placeholder) | v2 (From Your GDD) |
|---|---|---|
| Tokens | `$BOUNTY` (1 token) | `$BERRY` (₿ɇ, 10B) + `$GLORY` (ɠł, 1B) |
| Combat | TBD (turn-based considered) | **Real-time skill-based** confirmed |
| Devil Fruit Types | 3 types | **4 types** (+ Mythical) |
| Factions | None defined | **4 Factions**: Pirate, Marine, Revolutionary, Celestial |
| Classes | 6 (names TBD) | **6 fully named + described** |
| Haki NFTs | Generic | **Haki Crystals** (mintable w/ ₿ɇ, random type) |
| Chain Strategy | OneSea Chain only | **Multi-chain**: OneSea (primary) + ETH/BNB/Polygon/Solana bridges |
| Levels | 1–250 confirmed | 1–250 confirmed |
| NFT Classes | 3 types | **5 types**: Ships, Crew, Devil Fruits, Weapons/Artifacts, Haki Crystals |

---

## 🎮 Game Systems — Full Reference

### Classes (GDD Section 5)

| Class | Role | Primary Stats | Specialty |
|---|---|---|---|
| **Warrior** | Frontline Tank | Strength + Defense | Balanced melee, high endurance |
| **Gunner** | Ranged/Sniper | Dexterity + Luck | Rifles & cannons, armor-piercing |
| **Navigator** | Support | Dexterity + Haki | Buffs team, masters storm terrain |
| **Elementalist** | Mage/AoE | Haki + Luck | Devil Fruit elemental powers |
| **Brawler** | Melee DPS | Strength + Haki | Bare-handed + Haki enhancements |
| **Beastmaster** | Hybrid | Strength + Dexterity | Zoan forms + creature commands |

### Factions (GDD Section 10)

| Faction | Playstyle | Special Perks |
|---|---|---|
| **Pirate** | Freedom/Aggression | +15% bounty gain, highest scaling |
| **Marine** | Law/Defense | Bounty hunter quests, defense bonus |
| **Revolutionary** | Stealth/Liberation | Stealth missions, anti-authority quests |
| **Celestial** | Noble/Economic | Exclusive lore access, economic privileges |

### Devil Fruits (GDD Section 4)

| Type | Description | Best Class | Acquisition |
|---|---|---|---|
| **Paramecia** | Body modification powers | Any | Loot drops, treasure maps |
| **Zoan** | Animal transformation | Beastmaster | Events, boss rewards |
| **Logia** | Elemental body control | Elementalist | Rare loot, special events |
| **Mythical** | Legendary powers | Any | Boss-only / ultra-rare events |

**Awakening**: High-level transformation — costs ₿ɇ + Haki Crystals. Massively boosts power and elemental traits.

### Haki System (GDD Section 4)

| Haki Type | Unlock Method | In-Game Effect | Crystal Drop Rate |
|---|---|---|---|
| **Observation** | Level milestone + quest | Dodge chance, enemy detection | 55% |
| **Armament** | Level milestone + quest | Bypass Logia immunity, damage/defense boost | 43% |
| **Conqueror's** | Innate (cannot be trained) | AoE fear, overwhelm NPCs, boss bonus damage | 2% |

**Haki Crystals**: Mintable as NFTs from the official site using ₿ɇ. More mints = higher power tier (Tier 1–5). Type is randomly assigned on mint.

### Bounty Ranks

| Rank | Threshold | Perks |
|---|---|---|
| Unknown | 0 ₿ɇ | Starter |
| Pirate | 1M ₿ɇ | Access to Grand Line |
| Supernova | 100M ₿ɇ | Crew leadership rights |
| Shichibukai | 500M ₿ɇ | Territory control eligible |
| Yonko | 1B ₿ɇ | Emperor candidacy, Grand Fleet |
| Pirate King | 5B ₿ɇ | Legendary status, DAO power boost |

---

## ⛓️ Token Architecture

### ₿ɇ Berry Token — Core Economy

```
Total Supply:  10,000,000,000 ₿ɇ

Distribution:
  40% ─── Player Rewards      (earned through gameplay)
  20% ─── Treasury & Ecosystem
  15% ─── Developer & Staff   (vested)
  10% ─── Staking & Farming
  10% ─── Advisors & Partners
   5% ─── Reserve

Uses:
  • Combat rewards & exploration loot
  • Crafting, upgrades, trading
  • Haki Crystal minting
  • NFT purchases & Devil Fruit awakening
  • Bridge to on-chain (₿ɇ off-chain → $BERRY ERC-20)
```

### ɠł Glory Token — Governance & Premium

```
Total Supply:  1,000,000,000 ɠł

Distribution:
  25% ─── Player Rewards      (high-tier, tournaments, Emperor rewards)
  25% ─── Treasury & Ecosystem
  20% ─── Staking & Farming Pools
  15% ─── Developer & Staff   (vested)
  10% ─── Advisors & Partners
   5% ─── Reserve

Uses:
  • DAO voting (1 staked ɠł = 1 vote)
  • Premium features & exclusive items
  • Staking for passive yield
  • Treasure map events
  • Profit-sharing from marketplace fees
```

### Team Vesting Schedule

| Role | Allocation | Cliff | Vest Period |
|---|---|---|---|
| Founders & Core Devs | 15% | 6 months | 18 months |
| Game Designers & Artists | 5% | 3 months | 12 months |
| Staff & Support | 5% | 1 month | 9 months |
| Marketing & Community | 3% | 0 months | Ongoing |
| Advisors | 2% | 3 months | 6 months |

---

## 🌐 Blockchain Strategy

### Primary Chain: OneSea Chain (Custom EVM via OP Stack)
- Our own branded L2 — all core game transactions live here
- Low fees, 2-second block time, fully EVM-compatible
- Native gas token: `$SEA`

### Multi-Chain Bridges (Whitepaper Section 7)
| Network | Role |
|---|---|
| Ethereum Mainnet | Settlement layer, high-value NFT trading |
| BNB Chain | Low-gas alternative for emerging markets |
| Polygon | Fast microtransactions |
| Solana | Speed bridge for competitive PvP events |

### Smart Contracts to Build

| Contract | Type | Purpose |
|---|---|---|
| `BerryToken.sol` | ERC-20 | Core economy token (₿ɇ) |
| `GloryToken.sol` | ERC-20 + ERC-20Votes | Governance token (ɠł) with staking |
| `HakiCrystal.sol` | ERC-1155 | 3 Haki types, mintable with ₿ɇ |
| `DevilFruitNFT.sol` | ERC-721 | Rare fruits (Paramecia/Zoan/Logia/Mythical) |
| `CharacterNFT.sol` | ERC-721 | Playable pirate characters |
| `ShipNFT.sol` | ERC-721 | 6 ship classes with stats |
| `WeaponNFT.sol` | ERC-1155 | Loot-based weapons & artifacts |
| `BountySystem.sol` | Custom | On-chain bounty registry + oracle |
| `TerritoryControl.sol` | Custom | Island/New World territory ownership |
| `Marketplace.sol` | Custom | P2P NFT trading + 2.5% ɠł fee |
| `OneSEADAO.sol` | Governor | ɠł-weighted DAO governance |
| `Treasury.sol` | Multi-sig | Community treasury |
| `BridgeRelay.sol` | Custom | Off-chain ₿ɇ → on-chain $BERRY bridge |

---

## 🗺️ Official Roadmap (from Whitepaper)

| Phase | Focus | Target |
|---|---|---|
| **Phase 1** | Concept Design, Core Lore, Token Deployment | ✅ Completed |
| **Phase 2** | Alpha Build, NFT Minting System | Q1 2026 |
| **Phase 3** | Mainnet Launch + Playable Closed Beta | Q3 2026 |
| **Phase 4** | DAO Governance Activation | Q1 2027 |
| **Phase 5** | Multi-Chain Expansion & Metaverse Hub | Q4 2027 |

### Our Development Milestones (Technical Breakdown)

```
NOW (Phase 2 Start)
  ├── Repo scaffold ✅
  ├── Deploy BerryToken + GloryToken to testnet
  ├── Deploy HakiCrystal + DevilFruitNFT to testnet
  ├── Unity: Core game loop prototype
  └── Backend: Player auth + bounty API

Q2 2026
  ├── OneSea Chain devnet live
  ├── NFT minting site (Haki Crystals)
  ├── Unity: Combat system + 2 classes playable
  └── Closed Alpha (internal testing)

Q3 2026 (Phase 3)
  ├── OneSea Chain mainnet launch
  ├── Token public launch (₿ɇ + ɠł)
  ├── Playable closed beta (Android)
  ├── Marketplace live
  └── First World Boss event

Q1 2027 (Phase 4)
  ├── DAO governance portal live
  ├── All 6 classes available
  ├── Grand Line + New World regions open
  └── Emperor System + Fleet Wars

Q4 2027 (Phase 5)
  ├── Multi-chain bridges (ETH, BNB, Polygon, Solana)
  ├── Metaverse hub integration
  └── Full open world launch
```

---

## 📁 Files Produced (This Session)

| File | Description |
|---|---|
| `BerryToken.sol` | ERC-20 with 10B supply, vesting, minter roles |
| `GloryToken.sol` | ERC-20Votes governance with staking + vesting |
| `HakiCrystal.sol` | ERC-1155 Haki minting with ₿ɇ, random type, power tiers |
| `GameEnums.cs` | All Unity enums: Classes, Factions, Regions, Fruit Types, Haki, Rarity |
| `CombatSystem.cs` | Real-time combat with stats, combos, Haki/Logia mechanics |
| `schema.prisma` | Full PostgreSQL schema: Players, Ships, Crews, Quests, Events |
| `ARCHITECTURE.md` | Full system blueprint (v1, update with this doc) |
| `setup-repo.sh` | Monorepo scaffolding script |

---

## 🎨 Brand Colors (Whitepaper Section 12)
```
Deep Blue  : #0D1B2A  (backgrounds, ocean)
Gold       : #D4AF37  (accents, tokens, legendary rarity)
Silver     : #C0C0C0  (UI elements, common rarity)
```

---

*© 2025 One Sea Crypto Bounty Interactive Studio. All rights reserved.*
*"AC" initials in gold script — Albert Camings, Founder & Visionary*
