# Phoenix Paw 🟠🟣 Web3 Ecosystem on TON

**Phoenix Paw** is a modular Web3 gaming, social and impact ecosystem on **TON**, built as a **single Telegram Mini App / super-bot**.

No hype theatre, no mystery boxes of nothing.
**We don’t promise. We build.**



## 🔗 Quick Links

* Website: `phoenixpaw.io`
* Telegram: `@PHXPW`
* Token: `PHXPW` (TON Jetton) EQABtSLSzrAOISWPfIjBl2VmeStkM1eHaPrUxRTj8mY-9h43
* NFT Marketplace: Getgems (official collections)
* Docs / This repo: architecture, routes, APIs, models

> This repository documents the **product & tech model** of Phoenix Paw: routes, backend map, tokenomics model, staking integration, game modules & anti-abuse systems.



## 🧩 What is Phoenix Paw?

Phoenix Paw is not “one more token”, it’s a **hub**:

* One **Telegram Mini App** → tasks, games, staking, NFTs, Tigrit Village, raffles, Good Deeds Map, clans, future DAO.
* One **unified profile** → XP, Trust, Faith, Feathers, NFTs, access levels.
* One **transparent on-chain economy** → verifiable wallets, burns, staking, prize pools.

Everything is **modular**: screens, microservices, game modes and events can be rolled out and wired in step-by-step.



## 🪙 Core Asset: PHXPW

**PHXPW** — main ecosystem token on TON.

* Standard: Jetton
* Total Supply: `1,000,000,000` PHXPW
* Model: **deflationary via on-chain burns (BORN events)**
* Public:

  * Official contract & wallets
  * Burn address
  * Distribution segments that strictly sum to 1B, verifiable on-chain

On-chain = PHXPW & official NFTs.
Progression = **off-chain points**:

* `SCARLET` — base feathers (tasks, activity, referrals)
* `ICAR` — advanced feathers (hard modes, tournaments)
* `BROKEN` — penalty/special mechanics
* `Faith Points` — confirmed good deeds & honest, long-term behaviour

Feathers & Faith are **not tradable tokens**, only in-system reputation & utility.



## 🧬 Identity, Progression & Trust

Every user has a **living profile** shared across all modules:

* `XP` & `Level` — global progression
* `Trust Level (0–100)` — behaviour, abuse checks, on-chain history
* `Faith Points` — real impact, charity, eco-actions, honest play
* `NFT Power` — utility NFTs & access roles
* Badges, items, clans, factions → unified rank/permission model

High Trust / Faith unlock:

* boosted rewards
* private quests & pools
* smart events & tournaments
* future **governance hooks (DAO)**



## 🎮 Games & Mechanics

Phoenix Paw is a **game stack**, not one mini-game.

### 🌳 Tree(3): Flagship Mode

Hardcore logic / structure game:

* Sequence: `T1, T2, T3, ...`
* Exact node counts, parent rules, color limits (R/G/B)
* No repeats, no forbidden substructures
* Timer + 3 strikes system
* Leaderboards, tournaments, combo bonuses
* Fully integrated with profile, feathers, Trust/Faith

### Other Modes (progressive rollout)

* **Last Move** — discipline & timing
* **Minority** — social/choice game
* **Gift Battle** — event mode + rewards + charity
* **Phoenix GamePool** — check-in pools (off-chain & PHXPW)
* **Phoenix Gwent (concept)** — card game based on Phoenix Paw lore

All modes plug into shared:

* rewards system,
* anti-abuse service,
* events & raffles engine.



## 🐯 Tigrit Village & Lore

**Tigrit Village** — MMO-style chat world inside the Mini App:

* Locations, NPCs, AI-agents (phased)
* Quests and events bound to your:

  * profile
  * NFTs
  * Trust / Faith
* Based on the evolving **Tigrit Book** lore

Lore is **functional**: it drives access, buffs, cosmetics, events & narrative seasons.



## 🎁 NFTs, Loot & Merch

NFTs = **utility & status**, tightly wired into systems.

* **Genesis NFTs** — boosts, gated content, partial DAO access
* **PHXPW Hoodie — Access Token #001**

  * Limited supply
  * Right to claim real premium hoodie
  * Future perks & recognition
* Planned: `88 Gods`, `24 Zodiac`, seasonal sets

Loot & inventory:

* Eggs / lootboxes (with transparent RNG model)
* Utility items, tickets, buffs, cosmetic & physical rewards
* Strong linking between on-chain ownership and in-app rights



## 🌍 Good Deeds & Transparent Charity

Phoenix Paw ties gaming & DeFi with **real-world good**.

**Good Deeds Map**:

* Submit real actions (eco, charity, social impact)
* Provide media/on-chain proof
* Reviewed via hybrid moderation
* Get Faith Points, feathers, badges, rare rewards

Part of ecosystem revenue flows to:

* verified charity wallets
* eco & social initiatives

Where possible:

* tracked and auditable on-chain
* summarized in public reports



## 📈 Staking & Pools

Staking is implemented as a **separate service**, embeddable into the Mini App UI.

Key points:

* Aggregation of external, verifiable pools (e.g. Tonraffles, DeDust, jVault, etc.)
* In-app:

  * list of pools
  * conditions, APR (informational)
  * user stakes, unlock dates, status
* Data source of truth: **on-chain / official pool contracts**
* Off-chain storage only as cache
* No fixed-return promises, only transparent mechanics

This microservice approach allows integrating staking into current app safely & modularly.



## 🏆 Tasks, Raffles & Volume Flame

**Unified engine** for:

* Social / content / ads / on-chain / in-game / IRL tasks
* Quizzes on lore & tokenomics
* Raffles for:

  * tech
  * merch
  * NFTs
  * PHXPW rewards
* **Daily Riddles** for holders (with on-chain conditions)
* **Volume Flame**:

  * incentivizes organic PHXPW activity & liquidity
  * filters wash-trade, self-trade & fake volume

Everything is guarded by:

* eligibility rules,
* anti-abuse service,
* transparent public logic.



## 🛡 Clans, Factions & Future DAO

Social & governance layer on top of the ecosystem:

* Player **clans** with treasuries, quests & rankings
* **Factions** & seasonal wars/events
* DAO direction:

  * voting power via **key NFTs + Faith Points**
  * focus on reputation & contribution, not pure capital
  * decisions: prize pools, campaigns, lore/season parameters, etc.

Design is **opt-in, incremental, transparent**.



## ⚙️ Architecture & Stack (High-Level)

**Frontend**

* Telegram Mini App
* React + TypeScript
* TailwindCSS
* Modular UI, dark neon theme

**Backend**

* API Gateway (`/api`)
* Modular services:

  * auth, users, profile, wallet, tasks, quiz, games, gamepool
  * NFT & loot
  * good deeds, events & raffles
  * referrals, Tigrit, lore/content
  * clans/factions, DAO, mini-exchange, token tools
  * notifications, settings, smart-events
  * anti-abuse, analytics, admin

**Blockchain**

* Network: **TON mainnet**
* PHXPW Jetton
* Utility/NFT collections
* Official wallets & burn address
* Direct explorer & DEX integrations

**Security & Principles**

* No private keys / seed phrases. Ever.
* Only TonConnect / official wallets.
* Anti-abuse across tasks, games, raffles, trading campaigns.
* Admin actions fully logged (audit logs, role model, 2FA/IP recommended).


## 🧱 Why Phoenix Paw

Phoenix Paw is built as:

* A **long-term hub** for players, builders, and partners on TON.
* A system where:

  * smart play > blind degen,
  * reputation > pure volume,
  * real actions & honest activity are rewarded.
* A product-first ecosystem designed to be verifiable, forkable, integratable.

**Phoenix = transparency, discipline, longevity.**
If you build with the same values — welcome in. 🚀
