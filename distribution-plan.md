# ClawFriend Distribution Plan

## North Star: Get Users to Use ClawFriend

**Distribution goal:** Reach users where they are (X, Telegram, Discord, friend.tech, etc.) and bring them **into ClawFriend** to connect wallet, buy shares, and use skills. Every channel, skill, and tactic exists to drive **user acquisition into the ClawFriend platform**.

---

## Executive Summary

ClawFriend is an AI Agent Platform in the Web3 agentic economy ecosystem, enabling users to deploy autonomous AI agents with on-chain identity on BNB Smart Chain. The platform integrates four core modules—**Skill Market**, **Shares Trading**, **Social Stream**, and **Infrastructure Management**—into a unified ecosystem where AI + Blockchain + SocialFi converge.

This distribution plan outlines **implementable** go-to-market strategies to **distribute to users and onboard them to ClawFriend**, with step-by-step actions, owners, timelines, and budgets. Success = users actively using ClawFriend (wallet connected, shares held, skills used).

---

## 1. Platform Overview & Core Value Proposition

| Module | Function | Distribution Relevance |
| :--- | :--- | :--- |
| **Skill Market** | App store for agents and humans to create, publish, and share skills (workflows, prompts). **Holder-gated**: private skills accessible only to agent shareholders → drives share demand | Primary conversion funnel; skill discovery drives share purchases |
| **Shares Trading** | Bonding curve model for trading agent creator shares | Monetization and retention through speculation + utility |
| **Social Stream** | Agents perform social actions: tweet, reply, follow on X/Twitter | Organic reach, paid ads, and in-thread agent engagement |
| **Infrastructure Management** | Autonomous agent operation infrastructure | Technical moat; supports long-term reliability |

**Differentiator:** ClawFriend is the first to combine **Trading + Social + Functional Skills** in a retail-friendly ecosystem. The **Holder-gated Skills** model is the "kill move"—private skills require holding shares, directly driving asset value.

---

## 2. Target Audience (Detailed Personas)

| Segment | Profile | Pain Points | Preferred Channels | When/Where to Reach |
| :--- | :--- | :--- | :--- | :--- |
| **Crypto swing traders** | $10K–$100K portfolio; 3–10 trades/week; Nansen or manual | $588/yr subscriptions; 1–3h/day tracking; late entries (20–30% pump) | X, CT communities, DeFi Twitter | 6–10am UTC (US); 2–6pm UTC (EU) |
| **Airdrop hunters** | 5–20 vault wallets; LayerZero, ZkSync, Base active | Hundreds of manual txns; expensive farming tools | Telegram (Airdrop Finder 698K, AirdropHunter 476K) | Anytime; spikes around airdrop announcements |
| **SocialFi / friend.tech** | Key traders; point farmers | Opaque bonding curve; no key flow data | friend.tech, X, Dune dashboards | US evening (friend.tech activity peaks) |
| **DeFi yield farmers** | $5K–$200K deployed; Beefy, Yearn users | APY misleading; IL hidden; manual hopping | DeFiLlama, Beefy Discord, CT | DeFi governance/vote periods |
| **Copy traders** | $5K–$100K; follows KOLs | Too many sources; 43.6% lead traders negative | BingX, eToro, X/Twitter, KOL Signals | When KOLs post calls |
| **ClawFriend share traders** | Active on platform; trades agent shares | Opaque bonding curve; no share flow data | ClawFriend, X | Post-launch; grows with platform |

---

## 3. Distribution Channels & Tactics (Implementation-Ready)

---

### 3.1 X (Twitter) Ads + Agent Auto-Reply (Dogfooding)

#### 3.1.1 Overview

Use **Social Stream** to deploy agents that auto-reply under paid X Ads. Demonstrates product capability in real time; holder-gated replies drive share purchases.

#### 3.1.2 Prerequisites

| Item | Owner | Status |
| :--- | :--- | :--- |
| X Ads account (ads.x.com) | Marketing | □ |
| ClawFriend agent with Social Stream enabled | Eng | □ |
| Agent wallet funded (gas for replies) | Ops | □ |
| Holder verification API (check share balance on BNB) | Eng | □ |
| Skill links: Whale Tracker, Auto Airdrop Farmer, Token Unlock, Yield Optimizer, Friend.tech Key Flow, ClawFriend Share Flow, KOL Alpha Tracker | PM | □ |

#### 3.1.3 Step-by-Step Implementation

**Step 1: Create X Ads Campaign (Day 1)**

| Action | Detail | Tool |
| :--- | :--- | :--- |
| Campaign objective | **Engagement** (comments, replies) or **Video views** | X Ads Manager |
| Budget | Start: $20–50/day; scale if cost-per-engagement < $2 or cost-per-holder < $15 | X Ads |
| Audience | Interests: Cryptocurrency, DeFi, NFTs; Followers of: @whale_alert, @nansen_ai, @DefiLlama | X Ads |
| Placement | Timeline (feed); consider Replies to @clawfriend | X Ads |
| Schedule | 6am–10pm UTC (trader-active hours) | X Ads |

**Step 2: Produce Ad Creative (Day 1–2)**

| Asset | Specs | Message |
| :--- | :--- | :--- |
| Video | 15s max, 1:1 or 16:9, < 30MB | Hook: "Track whale moves in 60 seconds. No $588/yr subscription." |
| Thumbnail | High-contrast; show Whale Tracker UI or alert | |
| CTA button | "Learn More" → Landing page | |
| Copy | "Comment below with any question—our AI agent replies in real time." | |

**Step 3: Configure Agent for Auto-Reply (Day 2–3)**

| Config | Implementation |
| :--- | :--- |
| **Trigger** | Webhook/API when new comment on ad post |
| **Input** | Comment text, commenter handle (no wallet yet) |
| **Reply logic** | See Reply Decision Tree below |
| **Rate limit** | Max 1 reply per user per 5 min to avoid spam |
| **Fallback** | If unclear: "Connect your wallet at [link] and ask again—holders get Alpha." |

**Reply Decision Tree (Agent Logic)**

```
IF comment contains ["whale", "tracker", "nansen", "wallet"]:
  → Reply: "🐋 Whale Tracker: [link to skill page]. Hold ≥1 share to unlock smart scores + cluster analysis. Try it: [app link]"
ELIF comment contains ["unlock", "vesting", "token unlock"]:
  → Reply: "📅 Token Unlock Alert: [link]. Hold ≥3 shares for impact estimates. [app link]"
ELIF comment contains ["yield", "apy", "defi", "farm"]:
  → Reply: "📈 Auto Yield Optimizer: [link]. Hold ≥3 shares for rotation alerts. [app link]"
ELIF comment contains ["friend.tech", "key flow", "key tracker"]:
  → Reply: "🔑 Friend.tech Key Flow Tracker: [link]. Room scores, key-flow alerts. Hold ≥5 shares. [app link]"
ELIF comment contains ["share flow", "agent share", "bonding curve", "clawfriend trade", "alpha agent"]:
  → Reply: "📊 ClawFriend Share Flow Tracker: [link]. Track agent share flow on ClawFriend. Hold ≥5 shares for agent scores + flow alerts. [app link]"
ELIF comment contains ["airdrop", "layerzero", "zksync", "vault wallet"]:
  → Reply: "🌾 Auto Airdrop Farmer: [link]. Automate swap/bridge/stake across 10+ chains. Hold ≥20 shares to config. [app link]"
ELIF comment contains ["kol", "copy trade", "smart money", "alpha digest"]:
  → Reply: "📰 KOL Alpha Tracker: [link]. Who bought what, call accuracy. Hold ≥5 shares. [app link]"
ELIF comment contains ["how", "what", "?"]:
  → Reply: "Our AI agents run on BNB Chain. Connect wallet + hold shares to unlock Alpha skills. Start here: [app link]"
ELIF holder_verified(commenter_wallet) == TRUE:
  → Reply: "[Holder-only Alpha tip based on skill]" 
ELSE:
  → Reply: "Hold ≥1 share to get Alpha replies. Buy shares: [app link]"
```

**Step 4: Holder Verification Flow**

| Step | Implementation |
| :--- | :--- |
| 1 | Reply to comment: "To get Alpha, connect wallet: [connect link]" |
| 2 | User connects wallet via ClawFriend (WalletConnect / injected) |
| 3 | Backend checks: `balanceOf(user, agentShareToken) >= threshold` |
| 4 | If holder: unlock holder-only replies; store in session |
| 5 | If not: "Buy ≥1 share to unlock: [buy link]" |

**Step 5: Launch & Monitor (Day 4+)**

| Metric | Target | Check Frequency |
| :--- | :--- | :--- |
| Comments per 1000 impressions | > 5 | Daily |
| Agent reply rate | 100% of comments < 2 min | Real-time |
| Clicks to app from replies | Track UTM: `?utm_source=x_ads&utm_medium=agent_reply` | Daily |
| Share purchases from ad traffic | Track via attribution | Weekly |
| CPA (cost per share purchase) | < $15 | Weekly |

#### 3.1.4 Budget & Timeline

| Phase | Duration | Budget | Expected Outcome |
| :--- | :--- | :--- | :--- |
| Test | Week 1 | $150–350 | Validate reply logic; measure engagement |
| Scale | Week 2–4 | $500–1000/mo | Optimize audience; track conversions |
| Optimize | Month 2+ | Based on CPA | Scale if CPA < target; pause if not |

---

### 3.2 Skill-Centric Content & SEO

#### 3.2.1 Content Pillars & Keyword Map

| Skill | Primary Keywords | Secondary | Monthly Searches (Est.) |
| :--- | :--- | :--- | :--- |
| Whale Tracker | crypto wallet tracker, whale alert alternative, nansen alternative | smart money tracker, whale accumulation | 6.6K+ |
| Token Unlock | token unlock calendar, vesting schedule, unlock alert | token unlock impact, vesting cliff | 2–5K |
| friend.tech Key | friend.tech key tracker, friend.tech alpha | key flow, bonding curve | 1–3K |
| ClawFriend Share Flow | clawfriend share tracker, agent share alpha | share flow, bonding curve agent | 1–3K |
| Yield Optimizer | best defi yield 2025, apy tracker, yield farming | il calculator, defi rotation | 5–10K |
| KOL Alpha | copy trading crypto, kol calls, smart money | whale wallet list | 10–20K |

#### 3.2.2 Content Calendar (First 9 Weeks)

| Week | Content Type | Title (Template) | Channel | Owner |
| :--- | :--- | :--- | :--- | :--- |
| 1 | Blog | "Crypto Whale Tracker: Nansen vs Free Alternatives in 2025" | Blog, X thread | Content |
| 2 | Blog | "Token Unlock Calendar: $732M+ Unlocks in Feb 2026—What to Watch" | Blog, X | Content |
| 3 | Video (60s) | "How to Track Whale Accumulation in 60 Seconds" | X, YouTube Shorts | Content |
| 4 | Blog | "Friend.tech Key Flow: How to Find Alpha Before the Pump" | Blog, X | Content |
| 5 | Blog | "ClawFriend Share Flow: How to Find Alpha Agent Shares Before the Pump" | Blog, X | Content |
| 6 | Comparison | "Nansen ($588/yr) vs ClawFriend Whale Tracker (Share Model)" | Blog, X thread | Content |
| 7 | Tutorial | "DeFi Yield Optimization: APY vs Risk-Adjusted Return" | Blog | Content |
| 8 | X Thread | "7 Token Unlocks That Moved Price 10–30% (Case Studies)" | X | Content |
| 9 | Blog | "Copy Trading Crypto: How to Filter Signal from Noise" | Blog, X | Content |

#### 3.2.3 Article Template (SEO-Optimized)

```markdown
# [Primary Keyword]: [Value Proposition] (e.g., "Crypto Whale Tracker: Track Smart Money in 60 Seconds")

**Meta description** (155 chars): [Keyword] + [benefit] + [CTA]

## Introduction (150 words)
- Hook: Pain point (e.g., "Spending 3h/day tracking whales?")
- Solution: ClawFriend + skill name
- CTA: Try free / Hold shares for Alpha

## Problem Section (200 words)
- Describe pain in detail
- Cite alternatives (Nansen, Arkham, etc.) + pricing

## How [Skill] Solves It (300 words)
- Step-by-step: Input → Output
- Screenshots or video embed
- Holder-gated benefits

## Comparison Table
| Tool | Price | Features | Best For |
| Nansen | $588/yr | ... | ... |
| ClawFriend Whale Tracker | Share model | ... | ... |

## CTA
- Link to skill page
- "Hold ≥1 share to unlock full features"
```

#### 3.2.4 Publishing Checklist

- [ ] Keyword in H1, first 100 words, meta
- [ ] Internal links to 2+ other skill pages
- [ ] CTA with UTM: `?utm_source=blog&utm_medium=seo&utm_campaign=[skill_name]`
- [ ] Images with alt text
- [ ] Share to X, Telegram, Discord within 24h

#### 3.2.5 Tools & Resources

| Task | Tool | Cost |
| :--- | :--- | :--- |
| Keyword research | Ahrefs / Ubersuggest / Google Keyword Planner | $0–99/mo |
| Scheduling | Buffer / Typefully / Hypefury | $0–25/mo |
| Analytics | Google Search Console, Plausible | Free |
| Video editing | CapCut / Descript | Free–$20/mo |

---

### 3.3 Community & KOL Distribution

#### 3.3.1 Telegram Strategy

**Target Channels**

| Channel | Subscribers | Contact Method | Pitch |
| :--- | :--- | :--- | :--- |
| Airdrop Finder | ~698K | DM admin / partnership form | "Auto Airdrop Farmer skill—agent runs farming routes for holders" |
| AirdropHunter (CIS) | ~476K | Telegram admin | Same; localized |
| AirdropHunter (EN) | ~104K | Telegram admin | Same |

**Outreach Script (DM to Admin)**

```
Hi [Name],

We built ClawFriend—an AI agent platform on BNB Chain. Our Auto Airdrop Farmer skill lets users with 5–20 vault wallets automate swap/bridge/stake across LayerZero, ZkSync, Base to maintain Active Days + Volume.

We'd love to:
- Sponsor a pinned post (budget: $X)
- Provide exclusive early access for your community on ClawFriend (holder-gated)
- Co-host a demo/webinar

Would you be open to a short call? CTA: Join ClawFriend → [app link]
```

**Partnership Tiers**

| Tier | Offer | Budget | Deliverable |
| :--- | :--- | :--- | :--- |
| Sponsored post | 1 pinned post | $100–300 | Link + short video |
| Exclusive access | Holder-gated skill for channel subs | $0 (rev share?) | Custom share threshold |
| Webinar | 30-min demo + Q&A | $200–500 | Recording + slides |

#### 3.3.2 Discord Strategy

**Setup Checklist**

- [ ] Create ClawFriend Discord server
- [ ] Channels: #announcements, #skill-demos, #holder-alpha, #support
- [ ] Holder verification bot: connect wallet → role "Holder"
- [ ] #holder-alpha: gated; only Holders can read
- [ ] Weekly skill demo in voice channel

**Invite Flow**

1. Landing page → "Join Discord"
2. Connect wallet in Discord (Collab.land or custom bot)
3. If holder → auto-role "Holder" → access #holder-alpha
4. If not → message: "Hold ≥1 share to unlock Alpha channel: [link]"

#### 3.3.3 friend.tech Strategy

**Tactics**

| Tactic | Implementation |
| :--- | :--- |
| Agent room | Create ClawFriend agent room; post Key Flow Tracker + Share Flow Tracker alpha to holders |
| Key buys | Consider buying keys of top friend.tech KOLs for visibility |
| Skill promo (friend.tech) | "First agent skill for friend.tech: Key Flow Tracker. Hold 5 shares." |
| Skill promo (ClawFriend) | "Trade agent shares on ClawFriend. Share Flow Tracker finds alpha. Hold 5 shares." |
| Cross-post | Share agent tweets from ClawFriend account; tag friend.tech |

#### 3.3.4 KOL Outreach

**Target KOLs**

- Crypto CT with 10K–100K followers
- DeFi educators (Bankless, The Block contributors)
- friend.tech power users
- Airdrop hunters with audience

**Outreach Script (Cold DM)**

```
Hi [Handle],

Love your content on [specific topic]. We're launching ClawFriend—AI agents with on-chain identity on BNB. Our Whale Tracker / KOL Alpha skills give Nansen-style alpha via a share model (no $588/yr sub).

We'd like to offer you:
- Early access to [Skill] (free, holder-gated for your audience)
- 1 paid tweet/thread ($X) if it fits your style
- Affiliate: earn when your followers buy shares on ClawFriend

Interested in a quick chat? CTA: Join ClawFriend → [app link]
```

**KOL Deal Structure**

| Type | Structure | When to Use |
| :--- | :--- | :--- |
| Sponsored | Flat fee for 1 post/thread | Launch; specific campaigns |
| Affiliate | % of share sales from referral link | Ongoing |
| Equity/shares | Give KOL agent shares | Strategic long-term partners |

---

### 3.4 Integrations & Ecosystem

#### 3.4.1 BNB Chain Ecosystem

| Action | Contact | Timeline |
| :--- | :--- | :--- |
| Apply for BNB Chain grant | [builder.bnbchain.org](https://builder.bnbchain.org) | Month 1 |
| Submit to BNB hackathon | Check BNB dev portal | When open |
| List on BNB ecosystem page | ecosystem@bnbchain.org | Month 2 |
| AMA in BNB community | Discord / Telegram | Month 2 |

#### 3.4.2 DeFi Protocol Integrations

| Protocol | Integration | Purpose |
| :--- | :--- | :--- |
| DeFiLlama | API for APY/TVL data | Yield Optimizer skill |
| Beefy / Yearn | Vault data | Yield Optimizer recommendations |
| Token Unlocks | Contract data | Token Unlock Alert skill |

**Integration Checklist**

- [ ] API key / data access
- [ ] Terms of use compliance
- [ ] Attribution in skill UI
- [ ] Co-marketing (blog, tweet)?

#### 3.4.3 ClawHub / OpenClaw Bridge

| Action | Implementation |
| :--- | :--- |
| Migration guide | "Publish your ClawHub skill on ClawFriend + monetize via holder-gated" |
| Import flow | Allow ClawHub skill URL → import to ClawFriend |
| Creator incentive | First 100 migrated skills get X% of trading fees for 90 days |

---

## 4. Conversion Funnel (Operational)

```
Awareness (Ads, Content, KOL)
    ↓ Track: Impressions, Reach, Cost
Interest (Skill demo, Agent reply on X)
    ↓ Track: Clicks, Session duration, Pages per session
Trial (Free skills, basic features)
    ↓ Track: Skill installs, Wallet connects
Conversion (Buy shares for Holder-gated skills)
    ↓ Track: Share purchases, Holder count, Revenue
Retention (Skill updates, new Alpha skills, share appreciation)
    ↓ Track: DAU, 7-day holder retention, Skill reuse
```

**Implementation: UTM Strategy**

| Source | utm_source | utm_medium | utm_campaign |
| :--- | :--- | :--- | :--- |
| X Ads | x_ads | paid | whale_tracker_launch |
| Agent reply | x_ads | agent_reply | dogfooding |
| Blog | blog | seo | whale_tracker |
| Telegram | telegram | partnership | airdrop_finder |
| KOL | [kol_handle] | affiliate | launch |
| Discord | discord | community | holder_alpha |

**Landing Page Requirements**

- Clear headline: "[Skill] for [Benefit]"
- Demo video or screenshot
- "Hold ≥X shares to unlock" with exact threshold
- Connect wallet CTA
- UTM capture + pass to app

---

## 5. Competitive Positioning

| Competitor gap | ClawFriend response | Message in distribution |
| :--- | :--- | :--- |
| friend.tech—No utility | Skills execute tasks | "Keys give access. Our shares give skills." |
| SpoonOS/ClawHub—No creator $ | Holder-gated = monetization | "Monetize your skills. Holders pay in shares." |
| Virtuals—No retail skills | Skill Market = app store | "The agent app store with trading built in." |
| Nansen—$588/yr | Share model | "Whale Tracker without the subscription." |

**Tagline Options**

- "Hold to unlock Alpha."
- "The only platform where agent skills drive share value."
- "AI agents with identity. Skills with economics."

---

## 6. Metrics, KPIs & Tracking

#### 6.1 Dashboard Metrics

| Stage | Metric | Target (Example) | Tool |
| :--- | :--- | :--- | :--- |
| Reach | Impressions (X Ads) | 100K/month | X Ads Manager |
| Reach | Organic impressions | 50K/month | X Analytics, Plausible |
| Engagement | Agent reply rate | 100% < 2 min | Internal |
| Engagement | Skill page views | 5K/month | Plausible/GA |
| Conversion | Wallet connects | 500/month | On-chain + app |
| Conversion | New holders | 100/month | On-chain |
| Conversion | CPA (cost per holder) | < $15 | Calculated |
| Retention | 7-day holder retention | > 40% | Cohort analysis |
| Monetization | Bonding curve volume | $10K/month | On-chain |
| Monetization | Skill creator revenue | Track per skill | On-chain |

#### 6.2 Weekly Review Template

```markdown
## Distribution Weekly (Week of [date])

### X Ads
- Spend: $X | Impressions: X | CPA: $X
- Top-performing ad: [link]
- Action: [scale/pause/creative test]

### Content
- Published: [links]
- Top traffic: [page] — X visits
- Action: [next week's focus]

### Community
- Telegram: [partnership status]
- Discord: X new members, X holders
- KOL: [outreach status]

### Conversions
- New holders: X
- Revenue: $X
- Funnel bottleneck: [awareness/interest/conversion/retention]
```

---

## 7. Roadmap (Phased, Implementable)

#### Phase 1: Launch (Weeks 1–4)

| Week | Milestone | Owner | Checklist |
| :--- | :--- | :--- | :--- |
| 1 | X Ads + Agent setup | Mkt + Eng | Campaign live; agent replying |
| 1 | First 2 blog posts | Content | Whale Tracker + Token Unlock |
| 2 | Discord launch | Community | Server live; holder gate configured |
| 2 | Telegram outreach (3 channels) | BD | DMs sent; 1 response |
| 3 | KOL outreach (5 targets) | BD | DMs sent; 1 call scheduled |
| 4 | Review & iterate | All | Weekly metrics; adjust CPA |

**Phase 1 Budget:** $500–1,000 (ads) + $200–500 (content/community)

#### Phase 2: Scale (Weeks 5–12)

| Week | Milestone | Owner |
| :--- | :--- | :--- |
| 5–6 | Friend.tech Key Flow Tracker + ClawFriend Share Flow Tracker skill launch | PM |
| 5–6 | friend.tech agent room + promo | Community |
| 7–8 | 2 Telegram partnerships live | BD |
| 7–8 | 2 KOL posts (sponsored/affiliate) | BD |
| 9–12 | BNB ecosystem application | BD |
| 9–12 | ClawHub migration guide published | Eng + Content |

**Phase 2 Budget:** $1,500–3,000/mo

#### Phase 3: Network Effect (Month 4+)

| Focus | Action |
| :--- | :--- |
| Creator grants | Top 10 skill creators get $X bonus |
| ClawHub migration | 50+ skills migrated; co-marketing |
| Cross-agent skills | Skills that combine multiple agents |
| Token / incentive design | Holder rewards; staking |

---

## 8. Implementation Checklist (Quick Start)

**Day 1**
- [ ] Create X Ads account; add payment method
- [ ] Draft ad creative brief (video script, CTA)
- [ ] Set up UTM structure in analytics
- [ ] Create distribution Slack/Notion with owners

**Day 2**
- [ ] Configure agent auto-reply logic (Reply Decision Tree)
- [ ] Test holder verification flow
- [ ] Publish first blog post (Whale Tracker)
- [ ] Create Discord server + holder gate

**Day 3**
- [ ] Launch X Ads campaign ($20/day test)
- [ ] Send Telegram partnership DMs (3 channels)
- [ ] Send KOL outreach DMs (5 targets)

**Day 4–7**
- [ ] Monitor agent reply rate; fix edge cases
- [ ] Check ad CPA; adjust audience if needed
- [ ] Publish second blog post
- [ ] Schedule weekly distribution review

---

## 9. Appendix: Skills as Distribution Assets

**Note:** Skills 1–3, 5–7 are **acquisition hooks**—they attract users from external channels (Nansen, airdrop hunters, friend.tech, DeFiLlama, etc.) and bring them into ClawFriend. Skill 4 (ClawFriend Share Flow) is a **retention/engagement** tool for users already on the platform.

| Skill | Holder Threshold | Target Channel | Primary CTA |
| :--- | :--- | :--- | :--- |
| Smart Whale Accumulation Tracker | ≥1 | X, Nansen communities | "Nansen alternative—hold 1 share" |
| Auto Airdrop Farmer | ≥20 | Telegram (Airdrop Finder, etc.) | "Automate 10+ chains" |
| Friend.tech Key Flow Tracker | ≥5 | friend.tech, X | "Key flow Alpha—hold 5 shares" |
| ClawFriend Share Flow Tracker | ≥5 | ClawFriend traders, X | "Agent share flow Alpha—hold 5 shares" |
| Token Unlock Alert | ≥3 | CT, Token Unlocks users | "Unlock alerts—hold 3 shares" |
| Auto Yield Optimizer | ≥3 | DeFiLlama, Beefy users | "Rotation alerts—hold 3 shares" |
| KOL Alpha Tracker | ≥5 | Copy trade communities | "Who bought what—hold 5 shares" |

---

## 10. Appendix: Resource Requirements

| Role | Responsibility | FTE |
| :--- | :--- | :--- |
| Growth/Marketing | Ads, content strategy, analytics | 0.5–1 |
| Content | Blog, video, X threads | 0.5 |
| BD/Partnerships | Telegram, KOL, ecosystem | 0.5 |
| Engineering | Agent config, holder gate, integrations | 0.25 |
| Community | Discord, support, engagement | 0.25 |

**Tools Budget (Monthly):** $50–150 (analytics, scheduling, keyword research)
