<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="logo-dark.svg">
    <img src="logo.svg" alt="Rubasankar logo" width="64">
  </picture>
</p>

<h1 align="center">🚀 Personal Projects</h1>
<p align="center">Independent projects, designed, built, and maintained as the sole developer</p>

<p align="center">
  <a href="README.md">Profile</a> &nbsp;·&nbsp; <a href="experience.md">Experience</a> &nbsp;·&nbsp; <b>Projects</b> &nbsp;·&nbsp; <a href="education.md">Education</a> &nbsp;·&nbsp; <a href="certifications.md">Certifications</a>
</p>

---

These are personal projects with no company involvement. Client work completed at Queens Media Technologies is covered on the [Experience](experience.md) page.

<a name="digits"></a>

## 🛒 Digits

![Status](https://img.shields.io/badge/Live%20demo-coming%20soon-6B7280?style=flat-square) ![Role](https://img.shields.io/badge/Role-Sole%20Developer-2EA44F?style=flat-square) ![Typed](https://img.shields.io/badge/mypy-strict-1F5082?style=flat-square)

A self-hosted e-commerce platform for small and medium businesses, covering the complete order lifecycle from catalogue to returns and refunds (inventory, orders, payments, and shipping) without vendor lock-in or recurring SaaS fees.

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>✨ Key features</h4>
      <ul>
        <li>16 domain-bound Django apps: accounts, catalogue, pricing, inventory, shopping, checkout, orders, payments, delivery, customers/staff, promotions, and reviews</li>
        <li>Immutable stock-movement ledger</li>
        <li>Order and item snapshots that preserve historical pricing and addresses</li>
        <li>Return-lifecycle state machine: PENDING → APPROVED → RETURN_SHIPPED → RECEIVED → COMPLETED</li>
        <li>Category-scoped EAV attribute system for flexible product variants</li>
        <li>Twilio-based phone verification</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h4>🏗️ Architecture</h4>
      <ul>
        <li>Domain-driven design across 16 bounded contexts</li>
        <li>Service-layer architecture that keeps business logic out of views and models</li>
        <li>Apps communicate only through service calls, never through direct model access</li>
        <li>Database-level constraints that enforce accounting formulas and prevent negative stock</li>
      </ul>
      <h4>📈 Status</h4>
      <p>Fully typed (mypy strict) and lint-clean, with pre-commit-enforced secrets detection. Not yet in production.</p>
    </td>
  </tr>
</table>

<img src="https://skillicons.dev/icons?i=py,django,postgres,redis,tailwind" alt="Python, Django, PostgreSQL, Redis, Tailwind CSS"><br>
<sub>Also: Celery · django-allauth (MFA, social login) · Argon2 · django-unfold · django-cotton / labbui · daisyUI · ruff · mypy strict · pytest · factory-boy</sub>

---

<a name="chess-clock"></a>

## ♟️ Chess Clock (Schach Clock)

![Status](https://img.shields.io/badge/Live%20demo-coming%20soon-6B7280?style=flat-square) ![Role](https://img.shields.io/badge/Role-Sole%20Developer-2EA44F?style=flat-square) ![Platform](https://img.shields.io/badge/Platform-Mobile%20%26%20Web-000020?style=flat-square)

A modern chess clock for mobile and web that supports the Fischer, Bronstein, and Simple Delay increment formats used in tournament play. It provides accurate timing, audio cues, and haptic feedback suited to both casual club matches and timed tournaments. Designed, built, and shipped end-to-end.

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>✨ Key features</h4>
      <ul>
        <li>Real-time two-player clock with pause, reset, and turn-based timing logic</li>
        <li>Three increment formats: Fischer, Bronstein, and Simple Delay</li>
        <li>11 FIDE-standard time-control presets plus a custom builder</li>
        <li>Four clock-face themes and two table orientations for face-to-face or physical-clock play</li>
        <li>Audio and haptic feedback, with low-time alerts at 30 seconds</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h4>🏗️ Architecture</h4>
      <ul>
        <li>Persisted app state (presets, theme, sound and haptics preferences) via Zustand</li>
        <li>Worklet-based animation for smooth, performance-critical UI updates</li>
        <li>Codebase organised into <code>clock/</code>, <code>settings/</code>, and <code>time-control/</code> feature modules</li>
      </ul>
      <h4>📈 Delivery</h4>
      <p>Full CI/CD pipeline with linting, type-checking, formatting, automated EAS builds on tagged releases, and PR preview builds via EAS Update. Private repository, published under <code>rubasankar-dev</code> on Expo.</p>
    </td>
  </tr>
</table>

<img src="https://skillicons.dev/icons?i=react,ts" alt="React, TypeScript"><br>
<sub>Also: React 19 · React Native · Expo SDK 57 · Expo Router · Zustand · expo-audio · expo-haptics · React Native Reanimated</sub>

---

<p align="center">
  <a href="README.md"><b>Back to profile</b></a> &nbsp;·&nbsp; <a href="experience.md">Experience</a>
</p>
