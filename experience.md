<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="logo-dark.svg">
    <img src="logo.svg" alt="Rubasankar logo" width="64">
  </picture>
</p>

<h1 align="center">💼 Experience</h1>
<p align="center">Professional history and detailed project contributions</p>

<p align="center">
  <a href="README.md">Profile</a> &nbsp;·&nbsp; <b>Experience</b> &nbsp;·&nbsp; <a href="projects.md">Projects</a> &nbsp;·&nbsp; <a href="education.md">Education</a> &nbsp;·&nbsp; <a href="certifications.md">Certifications</a>
</p>

---

## 🏢 Software Developer I · Queens Media Technologies Pvt Ltd

<table>
  <tr>
    <td><b>📍 Location</b></td>
    <td>Bangalore, India</td>
    <td><b>📅 Duration</b></td>
    <td>December 2024 - June 1, 2026 (~1.6 years)</td>
  </tr>
  <tr>
    <td><b>👥 Team</b></td>
    <td>Solo on internal tools, up to 8+ on larger engagements</td>
    <td><b>🧭 Reporting to</b></td>
    <td>CEO / Manager</td>
  </tr>
</table>

Queens Media Technologies is a development agency delivering full-stack web, mobile, and blockchain/Web3 engineering across multiple client engagements. Over the course of the role I worked on a client e-commerce platform (February - June 2026), an internal email-tracking tool (December 2025 - January 2026), and Infuex, a large Web3 platform spanning smart contracts, backend services, and a mobile wallet app (January - December 2025). In April 2026 I also handled the initial setup and handoff of a separate client project, TaskTracker.

### 📌 Responsibilities

- Built the user, cart, and order backend (Django, DRF) and the product endpoints (FastAPI) for a client e-commerce platform, with Razorpay payments and admin management, and contributed to its front-end migration from React to Next.js.
- Built an internal Django + React email-tracking tool with IMAP synchronisation as the sole developer.
- Used Docker, Docker Compose, and GitHub Actions for local environments and CI/CD.
- Proposed project plans and technical approaches, reviewed code for junior developers, and took part in client meetings.
- On the Web3 wallet platform, designed and built four components independently (the cross-chain EVM + Tron gasless token-transfer system, the wallet-auth profile API, the blockchain metadata API, and the `walletcore` native module in Kotlin/Swift) and worked with the team on WebRTC calling, signalling, and the React Native app.

### 🏆 Key Achievements

- Helped keep cached product browsing under **200 ms** and checkout under **500 ms** on the e-commerce platform.
- Designed and built, independently, a gasless transfer system validated on the **Sepolia (EVM)** and **Nile (Tron)** testnets.
- As part of the team, cleaned up the wallet app's React Native codebase: **3,000+ lines** of unused code removed and **15+ type-definition files** consolidated.

### 🧰 Tools and Technologies

<table>
  <tr>
    <td width="170"><b>Backend</b></td>
    <td><img src="https://skillicons.dev/icons?i=py,django,fastapi" alt="Python, Django, FastAPI"><br><sub>DRF · Celery · SQLAlchemy · Pydantic · structlog</sub></td>
  </tr>
  <tr>
    <td><b>Frontend &amp; Mobile</b></td>
    <td><img src="https://skillicons.dev/icons?i=nextjs,react,ts,kotlin,swift" alt="Next.js, React, TypeScript, Kotlin, Swift"><br><sub>React Native (Expo)</sub></td>
  </tr>
  <tr>
    <td><b>Data &amp; DevOps</b></td>
    <td><img src="https://skillicons.dev/icons?i=postgres,redis,sqlite,mysql,supabase,docker,githubactions" alt="PostgreSQL, Redis, SQLite, MySQL, Supabase, Docker, GitHub Actions"><br><sub>Docker Compose · black · flake8 · mypy · ruff · Git</sub></td>
  </tr>
  <tr>
    <td><b>Real-time</b></td>
    <td><sub>WebRTC · Socket.IO · JWT</sub></td>
  </tr>
  <tr>
    <td><b>Web3</b></td>
    <td><img src="https://skillicons.dev/icons?i=solidity" alt="Solidity"><br><sub>Truffle · Ethers.js · Web3.js · TronWeb · OpenZeppelin · EIP-712 · CREATE2</sub></td>
  </tr>
</table>

---

## 🔍 Project Spotlights

### 🛒 E-Commerce Platform (Client Project)

![Duration](https://img.shields.io/badge/Feb%202026%20--%20Jun%202026-1F2937?style=flat-square) ![Role](https://img.shields.io/badge/Role-Backend%20%26%20Front--end%20Migration-0A66C2?style=flat-square) ![Repository](https://img.shields.io/badge/Repository-Confidential-6B7280?style=flat-square)

A distributed e-commerce platform made up of a Next.js storefront, a FastAPI product-catalogue service, and a Django transactional backend, designed to replace a monolithic architecture with independent scalability, technology specialisation, and deployment isolation. I built the user, cart, and order backend on Django/DRF and the product endpoints in FastAPI, and contributed to moving the React front end to Next.js, using Docker and GitHub Actions for builds and deployment.

#### What I built

- Two-phase inventory reservation and commit
- Dual-verification payment model (provisional confirmation plus webhook)
- Idempotency on critical order and checkout operations

#### Architecture decisions

- Django as the sole database writer, with FastAPI serving as a read-only catalogue service (enforced at the database level)
- Redis split across five logical databases by domain
- Immutable product images with a one-year CDN cache TTL

**Outcome:** sub-200 ms cached product browsing, sub-500 ms checkout, and rate limiting on the API.

<img src="https://skillicons.dev/icons?i=nextjs,ts,tailwind,fastapi,django,postgres,redis,docker,githubactions" alt="Next.js, TypeScript, Tailwind CSS, FastAPI, Django, PostgreSQL, Redis, Docker, GitHub Actions"><br>
<sub>Also: SQLAlchemy · Pydantic · DRF · Celery · Razorpay · SendGrid</sub>

> **Note:** In April 2026, alongside this engagement, I set up the initial project structure for TaskTracker, a task and operations management platform for accounting teams, before handing it off to the client's own team.

### 📧 Email Response Management System

![Duration](https://img.shields.io/badge/Dec%202025%20--%20Jan%202026-1F2937?style=flat-square) ![Role](https://img.shields.io/badge/Role-Sole%20Developer-2EA44F?style=flat-square) ![Repository](https://img.shields.io/badge/Repository-Internal-6B7280?style=flat-square)

An internal web application that tracks incoming emails, monitors response times, and flags overdue follow-ups through IMAP integration, giving the team visibility into which emails needed a reply and whether responses were on time. I built the entire application from scratch: backend, frontend, and email-sync infrastructure.

#### What I built

- IMAP email synchronisation with progress tracking
- Email threading via RFC 5322 headers (`In-Reply-To`, `References`)
- Content parsing that separates original text from quoted and forwarded content
- HTML sanitisation with bleach
- A dashboard with response-time metrics, a skip/snooze workflow, ignore lists, and follow-up alerts for overdue responses

#### Architecture decisions

- Background threading for email sync so it never blocks API requests
- Original and quoted content stored separately for cleaner display
- A custom auth model with an Admin / Manager / Team Lead / Employee role hierarchy

**Outcome:** used internally for email workflow management.

<img src="https://skillicons.dev/icons?i=django,py,react,ts,vite,tailwind,sqlite,mysql" alt="Django, Python, React, TypeScript, Vite, Tailwind CSS, SQLite, MySQL"><br>
<sub>Also: DRF · JWT · Beautiful Soup 4 · Bleach · Axios</sub>

### ⛓️ Infuex: Web3 Wallet and Communication Platform

![Duration](https://img.shields.io/badge/Jan%202025%20--%20Dec%202025-1F2937?style=flat-square) ![Role](https://img.shields.io/badge/Role-Blockchain%2C%20Backend%20%26%20Mobile-0A66C2?style=flat-square) ![Repository](https://img.shields.io/badge/Repository-Confidential-6B7280?style=flat-square)

A mobile wallet for a crypto-focused client that combines secure multi-chain asset management with encrypted real-time communication, removing the need for separate wallet and messaging apps. The platform spanned smart contracts, backend services, and a mobile app, and was a team effort. I designed and built four components independently (the profile service, the blockchain metadata API, the gasless transfer system, and the native wallet module) and worked with the team on WebRTC calling, signalling, and the mobile app.

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🔐 Backend services (independent)</h4>
      <ul>
        <li><b>Blockchain metadata API</b> (FastAPI, SQLModel, SQLite): CRUD endpoints with pagination for blockchain and asset metadata, hash-based authentication for writes, a small HTML dashboard, and dependency-injected DB sessions.</li>
        <li><b>Profile service</b> (DRF, Supabase): wallet-signature authentication instead of passwords, JWT obtain/refresh tied to EVM signatures, profile-picture storage in Supabase buckets, multi-chain wallet addresses as a JSON field, and a custom <code>WalletAuthPermission</code> class.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h4>📡 WebRTC signalling server (team)</h4>
      <ul>
        <li>Node.js, TypeScript, and Socket.IO server for voice, video, and screen-share calls.</li>
        <li>JWT authentication during the WebSocket handshake, call-session management (initiate, accept, reject, end), and relaying of offers, answers, and ICE candidates.</li>
        <li>Mic/camera state sharing, automatic cleanup on disconnect, in-memory state with Socket.IO rooms for direct routing, and four iterations (v0.1 to v0.4).</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>📱 Mobile app</h4>
      <ul>
        <li><b>Independent:</b> the <code>walletcore</code> native module (Kotlin/Swift) for Ethereum/Tron transaction signing, wallet creation, mnemonic restoration, and address generation.</li>
        <li><b>With the team:</b> WebRTC video/audio calling with Socket.IO signalling, encrypted peer-to-peer chat, and the seed-phrase onboarding, backup, and restore flow.</li>
        <li>Codebase cleanup: 3,000+ lines of unused code removed and 15+ type-definition files consolidated across 90+ files.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h4>⛽ Gasless transfers (independent)</h4>
      <ul>
        <li>Token transfers without holding native gas currency (ETH/TRX), using EIP-712 permit signatures for gas subsidies.</li>
        <li><code>SmartContractAccount</code> contracts for permit-based ERC20/TRC20 transfers, and a <code>SmartContractAccountFactory</code> using CREATE2 for deterministic addresses.</li>
        <li>EIP-712 domain separator and struct-hash computation, signature recovery for EVM (<code>ecrecover</code>) and Tron, and nonce-based replay protection, validated on Sepolia and Nile.</li>
      </ul>
    </td>
  </tr>
</table>

<img src="https://skillicons.dev/icons?i=react,ts,kotlin,swift,nodejs,fastapi,django,supabase,sqlite,solidity" alt="React Native, TypeScript, Kotlin, Swift, Node.js, FastAPI, Django, Supabase, SQLite, Solidity"><br>
<sub>Also: Expo · WebRTC · Socket.IO · bitcoinjs-lib · ethers · elliptic · Truffle · Web3.js · TronWeb · OpenZeppelin · EIP-712</sub>

---

<p align="center">
  <a href="README.md"><b>Back to profile</b></a> &nbsp;·&nbsp; <a href="projects.md">Personal projects</a>
</p>
