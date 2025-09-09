# AI Apartment

AI Apartment is a virtual city where Web3 users can turn their wallets into **living digital identities**.  
Each user can rent an apartment that automatically syncs their **tokens and NFTs**,  
and an AI assistant helps analyze, explain, and showcase assets.

This repo serves as the starting point for documentation and community feedback.  
Demo 👉 [AI Apartment](https://aiapartment.app/)

⚠️ Note: AI Apartment is currently in **Proof of Concept (PoC)** stage.  
All data may be reset or deleted at any time during development. Please don’t store anything critical.

![Image](https://github.com/Tomoyouki-Lai/ai-apartment/raw/main/ai-apartment-9m.gif)

---

## ✨ Why AI Apartment?

Web3 users face common challenges:
- Assets are scattered across multiple chains and wallets  
- No easy way to selectively showcase tokens or NFTs  
- Wallets are hard to understand for newcomers  
- Assets are static numbers, lacking insights or context  

**AI Apartment reimagines this as a social + AI-powered experience**.

---

## 🏙 Core Concept: Virtual Apartment. Real Social Life.

- **Apartments** → Your Web3 profile & identity card  
- **Assets on display** → Choose which tokens/NFTs to showcase  
- **AI Assistant** → Explains assets, trends, and gives insights  
- **Visitors** → Friends can explore, comment, and connect  

Think of it as a **cross-chain, AI-enhanced Web3 portfolio** that feels social.

---

## 🕹 How to Play

1. **Login with your wallet** → Get **1000 ATT** starter credits  
2. **Pick an apartment** → Rent the one you like as your Web3 home  
3. **Visit neighbors** → Explore their assets, NFTs, and collections  
4. **Use AI Assistant** → Analyze and understand more about assets  
5. **Social (coming soon)** → Give likes & leave comments  
6. **Draw cards & upgrade** → Earn cards to level up your apartment

---

## 🔧 Tech Overview

**Architecture (current MVP):**
- **Wallet Login**: MetaMask, WalletConnect  
- **Data Layer**: Aggregated via APIs (Covalent/Moralis/Alchemy)  
- **Database**: Off-chain storage for apartments + user settings  
- **AI Layer**: LLM (fine-tuned) to provide explanations & insights  
- **Frontend**: Web app, apartments are rendered as 3D cubes  

**Future Roadmap:**
- Layer-2 support (Optimism, Polygon)  
- Zero-knowledge proofs for selective asset sharing  
- AI autonomous agents for asset strategy  

---

## 💰 In-Game Currency (ATT)

- Internal currency = **AI Apartment Token (ATT)**  
- Purchased with **USDC / credit card**  
- Stored **only in platform DB** (closed-loop)  
- Used for:
  - Apartment rent & upgrades
  - Marketplace fees
  - AI premium features  

_(Note: Not tradable outside platform. Future ERC-20 launch TBD.)_

---

## 🎮 Game Design (Cards + Stats)

⚠️ Note: The card system is still in **planning / prototype stage**.  
Rules, effects, and balancing are **subject to major changes** during development.  
Current card examples are only for **demonstration and community feedback**.

Each player has:
- **LV (Level)** → Progression indicator  
- **ATT (AI Apartment Token)** → In-game currency  
- **⚡️ Energy** → Actions per turn  
- **❤️ Health** → Survival in events  
- **🧠 Knowledge** → Boosts quests and AI interactions  
- **✨ Charisma** → Social influence and negotiation power  

### Card Types
- **Quest** → Missions that grant rewards  
- **Support** → Boost stats or recover resources  
- **Life** → Slice-of-life experiences, random outcomes  
- **Event** → Global or random triggers affecting all players  
- **Ad** → Watch ads / visit links to earn ATT  

### Example Card Pool (PoC, 20+ cards)

```json
[
  { "id":"q1","type":"quest","title":"Hackathon Night","text":"Join a Web3 hackathon in your apartment.","effect":"🧠+2, ⚡️-1, ATT+10" },
  { "id":"q2","type":"quest","title":"NFT Exhibition","text":"Host an NFT exhibition for visitors.","effect":"✨+2, ATT+8" },
  { "id":"q3","type":"quest","title":"DeFi Farming","text":"Experiment with yield farming.","effect":"🧠+1, ❤️-1, ATT+12" },

  { "id":"s1","type":"support","title":"Energy Drink","text":"A quick boost for late-night grinding.","effect":"⚡️+3" },
  { "id":"s2","type":"support","title":"Meditation","text":"Clear your mind and restore balance.","effect":"❤️+2, 🧠+1" },
  { "id":"s3","type":"support","title":"Networking Event","text":"Meet builders and investors.","effect":"✨+3, ⚡️-1" },

  { "id":"l1","type":"life","title":"Pizza Night","text":"Friends bring pizza to your apartment.","effect":"❤️+1, ⚡️+1" },
  { "id":"l2","type":"life","title":"All-Nighter","text":"Coded until sunrise.","effect":"🧠+2, ❤️-2" },
  { "id":"l3","type":"life","title":"Casual Streaming","text":"Chill stream with your cat.","effect":"✨+1, ATT+5" },

  { "id":"e1","type":"event","title":"Market Crash","text":"Crypto market dips 20%.","effect":"ATT-10 for all players" },
  { "id":"e2","type":"event","title":"Bull Run","text":"Tokens pump overnight!","effect":"ATT+15 for all players" },
  { "id":"e3","type":"event","title":"AI Upgrade","text":"New AI patch boosts analysis.","effect":"🧠+2 for all players" },

  { "id":"a1","type":"ad","title":"Watch DeFi Ad","text":"View a short DeFi promo video.","effect":"ATT+5" },
  { "id":"a2","type":"ad","title":"Visit Partner DApp","text":"Click to explore a sponsored DApp.","effect":"ATT+7" },
  { "id":"a3","type":"ad","title":"NFT Marketplace Promo","text":"Check out featured NFTs.","effect":"ATT+10" }
]
```

---

## 🚀 Roadmap

- **2025 Q3**: MVP launch (apartments + AI assistant)  
- **2025 Q4**: Cross-chain expansion + social tools  
- **2026 Q1**: Marketplace beta + advanced AI analytics  
- **2026 Q2**: Community governance + potential token launch  

---

## 🙋 Feedback Wanted

We’re especially looking for input on:
- Best practices for cross-chain asset indexing  
- Privacy vs. transparency in asset sharing  
- Ideas for AI use cases in Web3 portfolios  

Open an issue, or reach out: **tomoyoukilai@gmail.com**  

---

## 📜 Disclaimer

This repo contains documentation and early-stage concepts.  
Not investment advice. AI Apartment is an experimental project.  
