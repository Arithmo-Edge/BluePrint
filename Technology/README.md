<div align="center">
  <img src="https://images.pexels.com/photos/1181244/pexels-photo-1181244.jpeg?auto=compress&cs=tinysrgb&w=1600&h=420&fit=crop" alt="Arithmo-Edge Hero Banner" width="100%" style="border-radius: 8px;" />
  
  # ⚙️ Arithmo-Edge Technology Stack & Zero-Cost Distributed Architecture
  
  *13 Federated Portals on Free Forever GitHub Pages • Centralized `Arithmo-Core-SDK` • `Hot Firebase + Cold 24h GitHub Data Lake` • `Cloudflare Workers` Edge Proxy • `Three.js`, `GSAP`, `Tailwind` & `Web Audio API`*
  
  <p>
    <img src="https://img.shields.io/badge/Hosting-Free_Forever_GitHub_Pages_%2B_Actions-00F0FF?style=for-the-badge&logo=github&logoColor=black" alt="Hosting" />
    <img src="https://img.shields.io/badge/Frontend-Vite_%E2%80%A2_Tailwind_%E2%80%A2_Three.js_%E2%80%A2_GSAP_%E2%80%A2_Framer-8B5CF6?style=for-the-badge&logo=react&logoColor=white" alt="Frontend" />
    <img src="https://img.shields.io/badge/Core_SDK-1--Click_Centralized_Arithmo--Core--SDK-10B981?style=for-the-badge&logo=javascript&logoColor=white" alt="Core SDK" />
    <img src="https://img.shields.io/badge/Storage-Hot_Cloud_Firestore_%2B_Cold_24h_GitHub_Lake-F59E0B?style=for-the-badge&logo=firebase&logoColor=white" alt="Storage" />
    <img src="https://img.shields.io/badge/Edge_Proxy-Cloudflare_Workers_(100k_Free_Reqs%2FDay)-F43F5E?style=for-the-badge&logo=cloudflare&logoColor=white" alt="Edge Proxy" />
    <img src="https://img.shields.io/badge/Client_Compute-Brent--Pollard_Rho_%2B_MediaPipe_Module_7-3B82F6?style=for-the-badge&logo=python&logoColor=white" alt="Client Compute" />
  </p>
</div>

---

## End-to-End System Infrastructure Topology

<div class="mermaid">
graph TD
    subgraph Client Tier ["Client Browser (Zero-Server Compute)"]
        Browser["Vite + React / ES6+ UI"]
        Three["Three.js 3D Manifolds"]
        Audio["Web Audio API Synthesizer"]
        Mod7["Module 7: MediaPipe & WebRTC Proctoring"]
        Math["Brent-Pollard's Rho & Miller-Rabin Engine"]
    end

    subgraph Hosting Tier ["Free Forever Infrastructure"]
        GH["13 GitHub Pages Repositories (rayaantasnim.github.io)"]
        CoreSDK["Centralized Arithmo-Core-SDK (engine.js)"]
    end

    subgraph Edge Tier ["Cloudflare Edge Gateway"]
        CF["Cloudflare Workers (100k Free Req/Day)"]
        Sec["Atomic UTC Clocks & Rate Limiter"]
    end

    subgraph Intelligence Tier ["AI & Verification Sandboxes"]
        Gemini["Gemini Pro/Flash + Qwen-Math"]
        SymPy["Python + SymPy Verification Sandboxes"]
    end

    subgraph Storage Tier ["Hybrid Hot/Cold Data Lake"]
        Firestore["Hot Cloud Firestore (Live ELOs & Wallets)"]
        GHData["Cold 24h GitHub Data Lake (Anonymized JSONL)"]
    end

    Browser --> GH
    GH --> CoreSDK
    Browser --> CF
    CF --> Sec
    CF --> Gemini
    CF --> Firestore
    Firestore --> GHData
    Browser --> Mod7
    Browser --> Math
</div>

* **Zero-Cost Hyper-Scaling Architecture:** Engineered to serve thousands of concurrent Olympiad competitors with zero VPS bills by offloading mathematical computation, UI rendering, and optical/audio proctoring (`Module 7`) to the client browser while securing API secrets and payment webhooks at the Cloudflare Edge.

---

## Technical Specifications & Architecture Deep-Dive

<details>
<summary><b>Dropdown 1: Frontend UI/UX Stack, 3D Graphics & Procedural Audio Engine</b></summary>

* **1. Core Build & Styling (`Vite` + `React` / `Vanilla ES6+` + `Tailwind CSS`):**
  * Ultra-fast sub-`50ms` Vite bundling paired with utility-first **Tailwind CSS** and custom **Cyber-Olympiad Glassmorphism UI** (`backdrop-filter: blur`, translucent neon borders, and fixed per-arena dark palettes: `#00F0FF` Cyan, `#10B981` Emerald, `#8B5CF6` Violet, `#F59E0B` Amber, `#F43F5E` Rose).
* **2. 3D WebGL & Choreographed Motion (`Three.js` + `GSAP` + `Framer Motion`):**
  * **`Three.js` (WebGL):** Renders interactive 3D prime number constellations, divisor lattices, and geometric manifolds in the hero workspace.
  * **`GSAP` (GreenSock Animation Platform):** Drives ultra-smooth `60fps` countdown timers, live ELO delta counters, and high-stakes `T-1 Minute` urgency animations.
  * **`Framer Motion`:** Powers tactile spring transitions for expandable 4-segment contest cards, `Toph.co`-style 3-column Expert panels, and in-chat dual-AI model selector pop-ups.
* **3. Mathematical Typesetting (`KaTeX` & `MathJax`):**
  * Instantaneous client-side rendering of Olympiad equations, modular congruences, $\sigma(N)$ / $\tau(N)$ series, and multi-step proofs across arenas, blogs, and dual guidebooks.
* **4. Zero-Asset `Web Audio API` Tactile Synthesizer:**
  * Synthesizes mechanical keystroke clicks, ascending harmonic combo chimes (`Combo x4`), and alert tones mathematically in real time via the browser's native **Web Audio API**—requiring zero external `.mp3` downloads.
* **5. Offline-First `PWA` & `IndexedDB` Resilience Vault:**
  * Installable **Progressive Web App (`Service Workers` + `Manifest`)** featuring `T-15 minute` contest push notifications and an encrypted **`IndexedDB` Offline Local Vault** that caches live contest questions and seals offline submissions with cryptographic millisecond timestamps during network drops.

</details>

<details>
<summary><b>Dropdown 2: Client-Side Deterministic Math & `Module 7` Edge Proctoring Engines</b></summary>

* **1. Sub-Millisecond Number Theory Engine (`Brent-Pollard's Rho` & `Miller-Rabin`):**
  * Deterministic primality testing and ultra-fast prime factorization implemented directly in client-side ES6+ JavaScript—handling massive integers instantaneously with zero server round-trips.
* **2. Client-Side `Module 7` Optical & Neural Audio Proctoring (`WebRTC` + `MediaPipe` / `TensorFlow.js`):**
  * Executes `100%` inside the competitor's browser; raw camera video and microphone audio are **never uploaded or saved to any server** (`Zero-PII` & `COPPA/GDPR-K` compliant).
  * Powers the **`4.5s` Context-Aware Adaptive Gaze Guard**, **3-Axis Neural Audio Collusion Trap**, and browser **Device/Canvas/WebGL Hardware Fingerprinting**.

</details>

<details>
<summary><b>Dropdown 3: Centralized `Arithmo-Core-SDK` (`1-Click` Global Maintenance Engine)</b></summary>

* **1. Single-Source Master SDK (`rayaantasnim.github.io/Arithmo-Core-SDK/engine.js`):**
  * Houses unified Firebase Authentication initialization, **Strict No-Handle Auto-Redirect** enforcement, **Dual-Handle Context Routing** (loading personal `@handle` on 12 sites vs. Cryptographic Academy Handle on `Subsite #9`), **Module 7** anti-cheat rules, and `Arithmo Wallet` / `Academy Wallet` state readers.
* **2. `30-Second` Global Hot-Patching:**
  * Every one of the 13 GitHub Pages repositories imports `engine.js` via a single script tag. Updating anti-cheat thresholds, security guards, or routing logic requires pushing to **only `1` repository**—automatically propagating across all 13 websites within `30 seconds`.

</details>

<details>
<summary><b>Dropdown 4: Unified Firebase, `Hot Firebase + Cold 24h GitHub Data Lake` & Read-Shield Caching</b></summary>

* **1. Unified `Firebase Auth` (Google OAuth 2.0) & `Cloud Firestore` (`Hot Operational DB`):**
  * Single Firebase UID shared across all 13 portals storing live running ELOs (`15` dimensions), `Arithmo Wallet` & `Academy Wallet` balances, active subscriptions, `donors` collection (`Wall of Patrons`), and active/recent matches.
  * Protected by strict **Firestore Security Rules** blocking client-side writes to `elo`, `hqElo`, `walletBalance`, and `isHqMember`.
* **2. `24-Hour` Automated Private GitHub Data Lake (`Cold Telemetry & Archive Repo`):**
  * Every `24 hours`, a scheduled **GitHub Actions** Python pipeline (`Arithmo ChronoVault AI` + `ComplianceGuard AI`) extracts completed match histories, solve-time latencies, backspace entropy, and `Zero-PII` cognitive vectors from Firestore, strips all personal identifiers, and executes an automated `git push` into a private **GitHub Data Archive Repository** (`JSONL` format) while pruning stale logs from Firestore.
* **3. Edge Read-Shield (`60s` Cloudflare Cache + `LocalStorage` SWR + `getCountFromServer()`):**
  * `Subsite #7 (Standings)` serves `60-second` cached snapshots at the Cloudflare Edge and browser `LocalStorage`, and uses lightweight **`getCountFromServer()`** aggregation queries to pin a user's exact global rank at near-zero read cost.

</details>

<details>
<summary><b>Dropdown 5: `Cloudflare Workers` Edge Proxy, `GitHub Actions` CI/CD & Payment Webhooks</b></summary>

* **1. `Cloudflare Workers` Secure API & Private GitHub Gateway (`100,000` Free Requests/Day):**
  * Keeps `GEMINI_API_KEY`, `QWEN_API_KEY`, `LEMON_SQUEEZY_WEBHOOK_SECRET`, and scoped `Contents: Read-only` **GitHub Fine-Grained Personal Access Tokens (`PAT`)** completely hidden from frontend code.
  * Enforces **Atomic UTC Server Clocks** (`X-Edge-Server-Time`), `15s` exponential hacking cooldowns, and dynamic semantic token routing (`General 1x` vs. `Premium 2x`).
* **2. `GitHub Actions` Automated Pipelines & `Python + SymPy` Verification Sandboxes:**
  * Runs continuous deployment (`CI/CD`) across all 13 `rayaantasnim.github.io` portals, executes overnight **Python + SymPy** mathematical verification sandboxes (`Arithmo AxiomCheck AI` & `SymPyVeritas AI`), runs post-contest **`MBTS` telemetry clustering**, and powers the `24h` Data Lake sync.
* **3. Lemon Squeezy / Paddle Merchant-of-Record Webhooks:**
  * Zero monthly fee cryptographic webhooks that credit subscriptions, +10% bonus wallet top-ups, @handle pass gifts, and ☕ Patron badges while handling global VAT/taxes automatically.

</details>

<details>
<summary><b>Dropdown 6: Local Development & Deployment Commands</b></summary>

<pre>
# 1. Clone the Centralized Core SDK & Subsites
git clone https://github.com/rayaantasnim/Arithmo-Core-SDK.git
cd Arithmo-Core-SDK

# 2. Install Dependencies across Workspaces
npm install

# 3. Configure Local Environment Variables (.env.local)
cp .env.example .env.local
# Set VITE_FIREBASE_API_KEY, VITE_CF_WORKER_ENDPOINT, etc.

# 4. Run Vite Development Server Locally
npm run dev

# 5. Deploy Cloudflare Worker Edge Proxy
npx wrangler publish

# 6. Push changes to trigger GitHub Actions CI/CD Pipeline
git add .
git commit -m "feat: upgrade edge proctoring and math engines"
git push origin main
</pre>

</details>

---

<hr>
<center>Authorized by Rayaan Tasnim 
<br>© All Rights Reserved 
<br>© Arithmo-Edge 
<br>Powered by Olympiad Edge
</center>