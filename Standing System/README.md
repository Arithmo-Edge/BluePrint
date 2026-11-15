<div align="center">

<img src="https://images.pexels.com/photos/373543/pexels-photo-373543.jpeg?auto=compress&cs=tinysrgb&w=1600&h=420&fit=crop" alt="Arithmo-Edge Standings Portal Banner" width="100%" />

# 🏆 Arithmo-Edge Standings Portal — 14 Real-Time Global Leaderboards

*Subsite #7 (`rayaantasnim.github.io/Arithmo-Standings/`) • Zero-Login Public Access • 14 Live Leaderboards • Monotonic HQ Roster & Honorary Council • Wall of Patrons*

<p>
  <img src="https://img.shields.io/badge/Portal-Subsite_%237_Standings_Portal-00F0FF?style=for-the-badge" alt="Portal Badge" />
  <img src="https://img.shields.io/badge/Public_Access-Zero--Login_Guest_Browsing-10B981?style=for-the-badge" alt="Public Access Badge" />
  <img src="https://img.shields.io/badge/Leaderboards-14_Real--Time_Categorized_Boards-8B5CF6?style=for-the-badge" alt="Leaderboards Badge" />
  <img src="https://img.shields.io/badge/HQ_Governance-All_Members_%E2%80%A2_Positional_Chronology-F59E0B?style=for-the-badge" alt="HQ Governance Badge" />
  <img src="https://img.shields.io/badge/Patrons-Live_Firestore_'donors'_Wall_of_Patrons-F43F5E?style=for-the-badge" alt="Patrons Badge" />
  <img src="https://img.shields.io/badge/Scaling-60s_Edge_Cache_%2B_getCountFromServer()-3B82F6?style=for-the-badge" alt="Scaling Badge" />
</p>

</div>

---

## 🌐 Public Access Architecture & 14-Board Drill-Down Topology

**Subsite #7 (`rayaantasnim.github.io/Arithmo-Standings/`)** serves as the high-velocity telemetry and global ranking engine of **Arithmo-Edge** (*Powered by Olympiad Edge*). Built on **Codeforces-Style Transparency**, the entire competitive ecosystem is open to public inspection without authentication barriers, while seamlessly elevating authenticated `@handle` accounts with personalized $O(1)$ rank pinning and social filtering.

* **Zero-Login Public Guest Access (Codeforces-Style Transparency):**
  * Any spectator, coach, or prospective competitor worldwide can visit **Subsite #7** with zero authentication friction.
  * Unauthenticated guests receive unrestricted read access to all **14 Real-Time Leaderboards**, multi-dimensional **Country**, **Organization**, and **Academy** filters, specialized **HQ Standing Tabs**, live match scoreboards, and the **Wall of Patrons**.
* **Authenticated `@handle` User Perks:**
  * Signing in via verified Gmail `@handle` activates **Pinned Personal Standing**, dynamically pinning the user's exact global rank and rating delta at the top viewport of every board—even if they currently sit outside the paginated Top 100.
  * Unlocks the **`★ My Friends`** social filter toggle to isolate rival and teammate standings across any active board.
* **5-Category Drill-Down Architecture (`14 Total Leaderboards`):**
  * Navigating from `Homepage` -> **`Explore Real Time Leaderboard`** exposes **5 Master Category Buttons** (`Headquarters`, `Core Arenas`, `Academy`, `Contributors`, `All Rounders`), which deterministically route into **14 Distinct Live Leaderboards**.

### Architectural Access & Routing Flowchart

<div class="mermaid">
flowchart TD
    Visitor([Global Visitor / Spectator]) --> Entry[Subsite #7: Standings Portal<br/>rayaantasnim.github.io/Arithmo-Standings/]
    Entry --> AuthCheck{Session State?}

    AuthCheck -->|Unauthenticated Guest| GuestMode[Zero-Login Public Access<br/>Full 14 Boards + Country/Org/Academy Filters + Wall of Patrons]
    AuthCheck -->|Authenticated @handle| AuthMode[Verified Competitor Mode<br/>O(1) Pinned Personal Standing + ★ My Friends Filter]

    GuestMode --> Hub[Explore Real Time Leaderboard<br/>5 Master Category Router]
    AuthMode --> Hub

    Hub --> Cat1[1. Headquarters<br/>1 Complete Governance Board]
    Hub --> Cat2[2. Core Arenas<br/>5 Topics × 2 Modes = 10 Isolated Boards]
    Hub --> Cat3[3. Academy<br/>1 Institutional ELO Board]
    Hub --> Cat4[4. Contributors<br/>1 Unified Stewardship Board]
    Hub --> Cat5[5. All Rounders<br/>1 Composite Multi-Arena Board]

    Cat1 --> HQDetails[All HQ Members • Non-Decreasing ELO • Positional Chronology<br/>2 Tabs + 6 Position Filters]
    Cat2 --> ArenaSplit[Strict No-Mixed ELO Policy<br/>General vs. Expert Isolation]
    Cat3 --> AcadSync[Syncs with Subsite #9 Academy Arena<br/>Dual-Rank Member Views]
    Cat4 --> ContribRule[Guidebook +2 • Blog-to-Lab +5 • AoPS Leak +3]
    Cat5 --> AllRoundRule[Unified Cross-Arena Performance Rating]

    Entry -.-> Patrons[Live Wall of Patrons<br/>Firestore 'donors' Collection • ☕ Patron Badge • Zero ELO Boost]
</div>

### Complete 14-Leaderboard Navigation & Drill-Down Tree

<pre>
Subsite #7: Arithmo-Edge Standings Portal (rayaantasnim.github.io/Arithmo-Standings/)
├── [Public Overlay] Live Wall of Patrons (Firestore 'donors' Sync • ☕ Patron Badges • Zero ELO Impact)
├── [Auth Overlay]   Pinned Personal Standing (O(1) getCountFromServer) + ★ My Friends Toggle
└── Homepage ──▶ Explore Real Time Leaderboard (5 Master Categories ──▶ 14 Live Leaderboards)
    │
    ├── [Category 01] Headquarters (1 Complete Governance Board — Uncapped Full Roster)
    │   ├── Tab 01: All HQ Roster (Prime Sovereign 1000 ──▶ Chief Arbiter 750 ──▶ Round Coordinator 500 ──▶ Problem Architect 300 ──▶ Core Sentinel 100)
    │   ├── Tab 02: Sovereign Council & Honorary Architects (Founding Prime Sovereigns + 👑 Honorary Prime Sovereigns)
    │   └── 6-Button Position Filter: [All Positions] | [Prime Sovereign & Honorary] | [Chief Arbiter] | [Round Coordinator] | [Problem Architect] | [Core Sentinel]
    │
    ├── [Category 02] Core Arenas (10 Isolated Leaderboards — Strict No-Mixed ELO Policy)
    │   ├── Arena 01: Prime Factors
    │   │   ├── Leaderboard #02: Prime Factors — General Mode
    │   │   └── Leaderboard #03: Prime Factors — Expert Mode
    │   ├── Arena 02: GCD-LCM
    │   │   ├── Leaderboard #04: GCD-LCM — General Mode
    │   │   └── Leaderboard #05: GCD-LCM — Expert Mode
    │   ├── Arena 03: Number of Divisors τ(N)
    │   │   ├── Leaderboard #06: Number of Divisors τ(N) — General Mode
    │   │   └── Leaderboard #07: Number of Divisors τ(N) — Expert Mode
    │   ├── Arena 04: Square Root
    │   │   ├── Leaderboard #08: Square Root — General Mode
    │   │   └── Leaderboard #09: Square Root — Expert Mode
    │   └── Arena 05: Sum of Divisors σ(N)
    │       ├── Leaderboard #10: Sum of Divisors σ(N) — General Mode
    │       └── Leaderboard #11: Sum of Divisors σ(N) — Expert Mode
    │
    ├── [Category 03] Academy (1 Institutional Board)
    │   └── Leaderboard #12: Global Institutions (Ranked by Indivisible Academy ELO • Syncs with Subsite #9)
    │
    ├── [Category 04] Contributors (1 Unified Global Board — No Arena Division)
    │   └── Leaderboard #13: Ecosystem Stewards (Ranked by Contribution ELO: +2 / +5 / +3)
    │
    └── [Category 05] All Rounders (1 Composite Multi-Arena Board)
        └── Leaderboard #14: Unified Multi-Arena Champions (Synthesized Overall All-Rounder Rating)
</pre>

---

## 🔍 Deep-Dive Architectural Specifications

<details open>
<summary><strong>1. Complete Breakdown of All 14 Real-Time Leaderboards (5 Master Categories)</strong></summary>

<br />

The Standings Portal partitions competitive telemetry into **14 strictly isolated leaderboards** across **5 Master Categories**, preventing rating inflation across divisions while honoring distinct forms of mathematical and architectural excellence:

* **Category 1 — Headquarters (`Leaderboard #01`: `1 Complete Governance Board`):**
  * **Uncapped Full Roster:** Unlike public competitive boards paginated to Top 100 snapshots, the Headquarters board renders **ALL Headquarters members** simultaneously without rank truncation.
  * **Monotonic Non-Decreasing HQ ELO (`never drops`):** HQ ELO acts as an immutable governance ledger of administrative, editorial, and architectural service—it only increments or holds steady and can never decrease.
  * **Strict Positional Chronology:** Rank ordering is governed first by hierarchical tier and induction chronology, and secondarily by HQ ELO. A lower-ranked HQ member **never passes** a higher-ranked senior member on the board, even if their raw HQ ELO numerically surpasses the senior member's score.
  * **Specialized Governance Controls:** Equipped with **2 Dedicated Tabs** and **6 Interactive Position Filters** (fully detailed in Section 2 below).

* **Category 2 — 5 Core Topic Arenas (`Leaderboards #02–#11`: `10 Isolated Boards` = `5 Arenas × 2 Modes`):**
  * Selecting **Core Arenas** prompts the visitor to pick one of the **5 Core Number Theory Arenas** and then select either **`General`** or **`Expert`** mode:
    * **Prime Factors:**
      * `Leaderboard #02` — *Prime Factors (`General`)*
      * `Leaderboard #03` — *Prime Factors (`Expert`)*
    * **GCD-LCM:**
      * `Leaderboard #04` — *GCD-LCM (`General`)*
      * `Leaderboard #05` — *GCD-LCM (`Expert`)*
    * **Number of Divisors $\tau(N)$:**
      * `Leaderboard #06` — *Number of Divisors $\tau(N)$ (`General`)*
      * `Leaderboard #07` — *Number of Divisors $\tau(N)$ (`Expert`)*
    * **Square Root:**
      * `Leaderboard #08` — *Square Root (`General`)*
      * `Leaderboard #09` — *Square Root (`Expert`)*
    * **Sum of Divisors $\sigma(N)$:**
      * `Leaderboard #10` — *Sum of Divisors $\sigma(N)$ (`General`)*
      * `Leaderboard #11` — *Sum of Divisors $\sigma(N)$ (`Expert`)*
  * **Strict No-Mixed ELO Policy:** Ratings earned in `General` rounds never bleed into `Expert` standings, and topic ratings remain completely decoupled across arenas.
  * **Forward Architecture (`V11.0+`):** Designed with modular arena schema keys to scale cleanly into the **4 Core IMO Hubs** in `V11.0+` without schema migration overhead.

* **Category 3 — Academy (`Leaderboard #12`: `1 Institutional Board`):**
  * Ranks registered schools, colleges, coaching centers, and universities worldwide by a single indivisible **`Academy ELO`**.
  * **`Academy ELO` Synthesis:** Computed dynamically from official inter-academy team contest outcomes combined with weighted average match performance across active verified institutional roster members.

* **Category 4 — Contributors (`Leaderboard #13`: `1 Unified Global Board — No Arena Division`):**
  * A single unified worldwide leaderboard—intentionally unsplit by topic arena or difficulty mode—ranking community stewards and problem curators by **`Contribution ELO`**:
    * **HQ-Approved Guidebook Math Entries:** **`+2 ELO`** per verified theorem breakdown, lemma proof, or canonical solution guide.
    * **AI-Curated `Blog-to-Lab` Modules:** **`+5 ELO`** per validated interactive mathematical laboratory transformed from research blog posts.
    * **First Valid AoPS Leak Reports:** **`+3 ELO`** awarded to the first contributor flagging an unoriginal or leaked contest problem prior to round lock.

* **Category 5 — All Rounders (`Leaderboard #14`: `1 Composite Multi-Arena Board`):**
  * Global prestige leaderboard ranking versatile competitors by their unified **Overall All-Rounder Performance Rating**, synthesized via weighted multi-arena aggregation across all core mathematical domains.

</details>

---

<details>
<summary><strong>2. Headquarters Standing Tabs, Position Filters & <code>Honorary Prime Sovereign</code> Showcase</strong></summary>

<br />

The **Headquarters Standing** view (`Leaderboard #01`) implements custom governance UI controls tailored to organizational transparency and historical preservation:

* **2 Dedicated Navigation Tabs:**
  * **Tab 01 — `All HQ Roster`:**
    * Renders the complete chronological command roster across all **5 Governance Tiers**:
      1. **Prime Sovereign (`1000` HQ ELO Tier)** — Supreme architectural and mathematical governance.
      2. **Chief Arbiter (`750` HQ ELO Tier)** — Final contest adjudication, anti-cheat tribunal authority, and rejudge sign-off.
      3. **Round Coordinator (`500` HQ ELO Tier)** — Contest scheduling, problemset balancing, and live round operations.
      4. **Problem Architect (`300` HQ ELO Tier)** — Original Olympiad problem authorship, test-case verification, and editorial drafting.
      5. **Core Sentinel (`100` HQ ELO Tier)** — Queue moderation, AoPS leak triage, and community integrity enforcement.
  * **Tab 02 — `Sovereign Council & Honorary Architects`:**
    * Permanent hall of honor showcasing the **Founding Prime Sovereigns** (*Founder & Chief System Architect* and *Co-Founder & Chief Mathematical Architect*) alongside every inducted **`👑 Honorary Prime Sovereign`**.
    * Displays each inductee's custom architectural title (such as *Principal Olympiad Architect*, *Principal AI Engineer*, or *Master Theorem Curator*) alongside a permanent ledger of their documented system and mathematical contributions.

* **6-Button Interactive Position Filter Bar:**
  * Provides instantaneous client-side filtering across the full HQ roster without triggering extra database reads:
    * **`All Positions`** — Displays the entire unedited HQ hierarchy.
    * **`Prime Sovereign & Honorary`** — Isolates Founding Prime Sovereigns and `👑 Honorary Prime Sovereigns`.
    * **`Chief Arbiter`** — Filters exclusively to `750`-tier Chief Arbiters.
    * **`Round Coordinator`** — Filters exclusively to `500`-tier Round Coordinators.
    * **`Problem Architect`** — Filters exclusively to `300`-tier Problem Architects.
    * **`Core Sentinel`** — Filters exclusively to `100`-tier Core Sentinels.
  * **Guest & HQ Member Parity:** Fully interactive for unauthenticated guests without login, while automatically displaying **Pinned Personal Standing** at the top of the roster when a verified HQ member is signed in.

</details>

---

<details>
<summary><strong>3. Dual-Rank <code>Members Standing</code> Inside <code>Academy Arena</code> (<code>Subsite #9</code>)</strong></summary>

<br />

Institutional telemetry bridges **Subsite #7 (`Standings Portal`)** and **Subsite #9 (`Arithmo Academy Arena`)** through synchronized dual-view institutional standings:

* **1. `Academy Standing` Tab:**
  * Mirrors the global inter-academy ranking (`Leaderboard #12` — ranked by indivisible `Academy ELO`).
  * Automatically highlights and anchors the logged-in student's or mentor's own institution within the global institutional hierarchy.

* **2. `Members Standing` Tab (Simultaneous Dual-Rank Display):**
  * Renders every verified student, captain, and mentor belonging to the institution alongside **two real-time ranks displayed side-by-side**:
    * **Internal Academy Rank:** The member's exact intra-institutional standing within their own school, college, or club roster (e.g., `#3 in Academy`).
    * **Global Arithmo-Edge Rank:** The member's exact worldwide standing across the entire global Arithmo-Edge userbase (e.g., `#142 Globally`).

</details>

---

<details>
<summary><strong>4. Live Match Scoreboards, <code>Virtual Gym</code> Ghost Badges, <code>Golden Crowns (👑)</code> & <code>Wall of Patrons</code></strong></summary>

<br />

Beyond static rating tables, **Subsite #7** powers live contest telemetry, historical ghost simulations, championship insignia, and community patronage recognition:

* **Live Match & 6-Hour Hacking Scoreboards:**
  * **Real-Time Contest Telemetry:** Streams live problem solve ratios (e.g., `12/72`), time-and-wrong-attempt submission penalties, and dynamic rank shifts throughout active rounds.
  * **Post-Contest Hacking Window (`6-Hour` Daily / `2-Hour` Sunday Mega):** Opens accepted submission steps for room-based peer hacking; successful hacks trigger immediate **Global Rejudge** recalculations across affected scoreboard rows.
  * **Deterministic ELO Publication Pipeline:** Official ELO deltas remain provisional until completion of the **`1-hour` post-hacking MBTS Telemetry Clustering** anti-cheat audit—publishing strictly at **`T+7h`** for daily Expert rounds and **`T+3h`** for Sunday Mega rounds.

* **`Virtual Gym` Ghost Leaderboard Simulation:**
  * Allows competitors to enter historical contests asynchronously and injects their live run as a ghost entry directly onto the original historical scoreboard.
  * Ghost rows are distinguished by an explicit **`#` / `Virtual`** badge alongside their unrated **Simulated ELO Delta** (e.g., `+45` / `-20`), preserving historical leaderboard integrity while giving accurate rating feedback.

* **Annual World Cup `Golden Crowns (👑)`:**
  * Permanently renders rotating **Golden Crowns (`👑`)** adjacent to the `@handles` of **`Top 128` Annual World Cup** champions across all 14 leaderboards and live match scoreboards.

* **Live `Wall of Patrons` (`☕ Patron` Badges):**
  * Connects directly to the Firestore `donors` collection populated in real time via **"☕ Support the 13-Year-Old System Architect / Buy Me a Coffee"** webhooks.
  * Recognizes generous community supporters on the dedicated **Wall of Patrons** and appends prestigious **`☕ Patron`** badges next to their `@handles` across standings.
  * **Strict Competitive Integrity Firewall:** Patronage grants **strictly zero ELO bonus, zero tie-breaker priority, and zero ranking boost** across any of the 14 leaderboards.

</details>

---

<details>
<summary><strong>5. Zero-Cost Firestore Read-Shield & High-Traffic Caching Engineering</strong></summary>

<br />

To sustain viral tournament spectator spikes (**`10,000+` concurrent viewers**) on a **`$0/month` GitHub Pages + Firebase Spark** architecture without exhausting daily Firestore read quotas, **Subsite #7** enforces a three-layer read-shield pipeline:

* **1. `60-Second` Cloudflare Worker Edge Cache + Browser `LocalStorage` SWR:**
  * Public leaderboard requests route through a Cloudflare Worker edge proxy serving pre-serialized JSON snapshots with a **`60-second` TTL**, paired with client-side `LocalStorage` **Stale-While-Revalidate (SWR)** caching.
  * Collapses **`100,000+` spectator page loads and refreshes** down to just a few hundred origin Firestore document reads per 24-hour cycle.

* **2. Exact $O(1)$ Pinned Personal Rank via `getCountFromServer()`:**
  * Rather than downloading thousands of user profile documents to compute where an authenticated competitor sits globally, the client dispatches a single lightweight Firestore **`getCountFromServer()`** aggregation query (`count where elo > user.elo`).
  * Pins the user's exact global rank at the top of any leaderboard in $O(1)$ aggregation cost (charged as 1 index read per 1,000 matched index entries—orders of magnitude cheaper than full document fetches).

* **3. Top-100 Paginated Public Boards (Except Full HQ Roster):**
  * All standard public boards (*10 Core Arena boards*, *Academy*, *Contributors*, and *All Rounders*) load compact, pre-indexed **Top-100 paginated JSON snapshots** backed by composite **Country**, **Organization**, and **Academy** filter indices.
  * **Headquarters Exception:** Because HQ governance requires complete organizational visibility and strict positional chronology, `Leaderboard #01` (`Headquarters`) bypasses the Top-100 cap to render the complete HQ roster in a single cached payload.

</details>

---

<div align="center">

### 🛡️ Arithmo-Edge Standings Portal • Built for Mathematical Transparency & Zero-Cost Scale
**Subsite #7 (`rayaantasnim.github.io/Arithmo-Standings/`)** • *Powered by Olympiad Edge*

</div>