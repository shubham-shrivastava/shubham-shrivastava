<h1 align="center">Shubham Shrivastav</h1>

<h3 align="center">Founder &amp; Senior Full-Stack Engineer</h3>

<p align="center">
  <em>I build developer-facing products end to end.<br/>Currently building <a href="https://shipguarde.com">ShipGuarde</a>, a quality gate for every release.</em>
</p>

<p align="center">
  <a href="https://shubhamshrivastav.com" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-0F766E?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio"/>
  </a>
  <a href="https://shipguarde.com" target="_blank">
    <img src="https://img.shields.io/badge/ShipGuarde-0A0E14?style=for-the-badge&logoColor=5EEAD4" alt="ShipGuarde"/>
  </a>
  <a href="https://linkedin.com/in/shubhamshrivastav" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:shrivastava.shubham219@live.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</p>

<p align="center">
  <a href="#projects">Projects</a> •
  <a href="#writing">Writing</a> •
  <a href="#tech-stack">Tech Stack</a> •
  <a href="#impact">Impact</a> •
  <a href="#connect">Connect</a>
</p>

---

### About

Senior full-stack engineer, **9+ years**, building developer-facing products end to end across TypeScript, Next.js, React, Node.js, Python, and PostgreSQL.

- 🚢 **Founder &amp; Principal Engineer at [ShipGuarde](https://shipguarde.com)**. Took it from an empty repository to a live multi-tenant SaaS with paid plans, a public API, and a [GitHub Action](https://github.com/ShipGuarde/review-action) other teams install.
- 💼 **Eight years at [Luzmo](https://luzmo.com)** (formerly Cumul.io), a Belgian company. Backend first, then full-stack, on a multi-tenant analytics platform that thousands of customers build against.
- 🤖 **Production AI, not demos.** Multi-agent orchestration, RAG on pgvector, and evaluation harnesses that catch quality regressions before users do.
- 🌍 **Remote since 2018**, on European hours from India the whole time. Written and async by default, not as a fallback.
- 📍 Based in **Pune, India**.

I like the unglamorous half of the work: the retry that doesn't swallow a real failure, the error message that says what to actually do. Nobody thanks you for those. They just don't leave.

---

### Currently

**Founder &amp; Principal Engineer, ShipGuarde.** Building all of it solo: architecture, dashboard, API, infrastructure, billing, docs, and the customer conversations.

**Full Stack Developer, Luzmo.** Owning developer-facing analytics and AI features end to end on a multi-tenant platform.

**Open to senior and staff full-stack roles**, remote and global. I read everything and reply properly.

---

<a id="projects"></a>
### Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://shipguarde.com">ShipGuarde</a> <sub><em>Founder</em></sub></h4>
      <p><em>A quality gate for every release. Multi-agent checks on any URL and every pull request, ending in one plain-English verdict a non-engineer can act on.</em></p>
      <ul>
        <li>Isolated parallel workers behind a Fastify orchestrator, with per-agent timeouts and a retry policy that retries <strong>only</strong> infrastructure faults, never a real finding</li>
        <li>Billing built for correctness: provider-agnostic payment seam, signature-verified webhooks deduped by event id, idempotent application, usage meters derived from the source of truth so they can't drift</li>
        <li><strong>Precision / recall / F1 eval harness</strong> that regression-guards agent quality as models and prompts change</li>
        <li><strong>23-component</strong> shared UI package, so a verdict renders identically in the dashboard, the PR comment, and the public report</li>
      </ul>
      <p><strong>Stack:</strong> <code>Next.js 15</code> <code>TypeScript</code> <code>Fastify</code> <code>BullMQ</code> <code>Redis</code> <code>PostgreSQL</code> <code>Prisma</code> <code>Zod</code> <code>Playwright</code> <code>Turborepo</code></p>
      <p><a href="https://shipguarde.com"><strong>🔗 shipguarde.com</strong></a> | <a href="https://github.com/ShipGuarde/review-action"><strong>⚙️ GitHub Action</strong></a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://shipguarde.com">
        <img src="https://shubhamshrivastav.com/assets/shipguarde1.png" alt="ShipGuarde preview" />
      </a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/shubham-shrivastava/ocularis">Ocularis</a> <sub><em>Apache-2.0</em></sub></h4>
      <p><em>Autonomous browsing agent built around reliability, recovery, and structured reasoning.</em></p>
      <ul>
        <li>Goal planner, postcondition checks, and critic-loop supervision</li>
        <li>Stuck detection with <strong>MD5 + SSIM</strong>, multi-step recovery, circuit-breaker escalation, and human approval gates</li>
        <li>Vision model support with <strong>UI-TARS</strong> via <strong>OpenRouter</strong></li>
        <li>Built in the open: typed public API, live dashboard, docs, Docker setup, contribution-ready test suite</li>
      </ul>
      <p><strong>Stack:</strong> <code>Python</code> <code>FastAPI</code> <code>Playwright</code> <code>PostgreSQL</code> <code>pgvector</code> <code>Next.js</code> <code>Docker</code></p>
      <p><a href="https://github.com/shubham-shrivastava/ocularis"><strong>📦 GitHub</strong></a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/shubham-shrivastava/ocularis">
        <img src="https://shubhamshrivastav.com/assets/ocularis1.jpeg" alt="Ocularis preview" />
      </a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://nexdocs.in">NexDocs</a></h4>
      <p><em>AI knowledge platform with a production RAG pipeline, taken 0 to 1 solo.</em></p>
      <ul>
        <li>Retrieval on <strong>pgvector</strong>, with chunking and ranking tuned so a reader lands on the right passage, not just the right document</li>
        <li><strong>40+ tRPC endpoints</strong> with end-to-end type safety</li>
        <li>Five parallel generation workers cut generation time <strong>70%</strong>, with circuit breakers, retries, caching, and tracing behind them</li>
        <li>Three delivery modes over one core: hosted site with custom domains, embeddable widget, API</li>
      </ul>
      <p><strong>Stack:</strong> <code>Next.js</code> <code>TypeScript</code> <code>tRPC</code> <code>NestJS</code> <code>FastAPI</code> <code>PostgreSQL</code> <code>pgvector</code> <code>Redis</code></p>
      <p><a href="https://nexdocs.in"><strong>🔗 nexdocs.in</strong></a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://nexdocs.in">
        <img src="https://shubhamshrivastav.com/assets/nexdocs1.png" alt="NexDocs preview" />
      </a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://apps.apple.com/in/app/timedial/id6758935499?mt=12">TimeDial</a></h4>
      <p><em>Native macOS timezone companion for distributed teams. Shipped through App Store review.</em></p>
      <ul>
        <li>Compare up to 6 timezones at once with real-time sync</li>
        <li>Interactive analog clocks with drag-to-adjust behavior</li>
        <li>Lightweight menu bar footprint</li>
      </ul>
      <p><strong>Stack:</strong> <code>SwiftUI</code> <code>AppKit</code> <code>Combine</code> <code>macOS</code></p>
      <p><a href="https://apps.apple.com/in/app/timedial/id6758935499?mt=12"><strong>🍎 App Store</strong></a> | <a href="https://github.com/shubham-shrivastava/timedial"><strong>📦 GitHub</strong></a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://apps.apple.com/in/app/timedial/id6758935499?mt=12">
        <img src="https://shubhamshrivastav.com/assets/timedial1.png" alt="TimeDial preview" />
      </a>
    </td>
  </tr>
</table>

<details>
  <summary><strong>More projects</strong></summary>
  <br />

#### [Railway Control Center](https://railway-control-center-frontend.up.railway.app/)
> The scheduling and health features Railway's dashboard doesn't offer, built on their public GraphQL API.

- Cron-based service spin-up and spin-down, plus one-time delayed actions ("stop in five minutes")
- One-click redeploy and restart, and a unified health view across projects
- Every GraphQL operation typed against the public schema, so a breaking change surfaces at compile time instead of in production

**Stack:** `Next.js 14` `TypeScript` `TanStack Query` `NestJS` `GraphQL` `Prisma` `PostgreSQL` `Docker`

[**🔗 Live Demo**](https://railway-control-center-frontend.up.railway.app/) | [**📦 GitHub**](https://github.com/shubham-shrivastava/railway-control-center)

---

#### [AutoResearch](https://github.com/shubham-shrivastava/autoresearch), Android
> Research app that aggregates and analyzes structured information from multiple sources.

- Cut research time by up to **70%** for end users
- Automated PDF report generation saving roughly **5 hours per project**
- Drove a **25% increase** in daily engagement

**Stack:** `Flutter` `Dart` `Firebase` `REST APIs`

[**🎯 Product Hunt**](https://www.producthunt.com/products/autoresearch-research-expert) | [**📦 GitHub**](https://github.com/shubham-shrivastava/autoresearch)

</details>

---

<a id="writing"></a>
### Writing

I write about problems I actually hit building ShipGuarde.

- **[Pass, Fail, and the Third State Your QA Tool Is Missing](https://shipguarde.com/blog/pass-fail-and-the-third-state)**. We pointed our own QA agents at two dozen real websites in a day and found five ways they reported a failure to measure as a result. The one primitive that fixes most of them. *(Aug 2026)*
- **[Running Untrusted Code Safely: A Field Guide for AI and CI Pipelines](https://shipguarde.com/blog/running-untrusted-code-safely)**. Every bot that reads your pull requests is executing code it didn't write. Sandboxing, secret isolation, and least privilege. *(Jul 2026)*
- **[One Certificate for Code Review and Visual QA](https://shipguarde.com/blog/one-certificate-for-code-and-visual-qa)**. Reviewing the diff is half the job. The other half is the running app. *(Jun 2026)*

[**All posts →**](https://shipguarde.com/blog)

---

<a id="tech-stack"></a>
### Tech Stack

#### Languages
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

#### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Radix UI](https://img.shields.io/badge/Radix_UI-161618?style=for-the-badge&logo=radixui&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)

#### Backend &amp; Data
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

#### AI in Production
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/🦜_LangChain-1C3C3C?style=for-the-badge)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![UI-TARS](https://img.shields.io/badge/UI--TARS-Vision_Model-5B6CFF?style=for-the-badge)
![OpenRouter](https://img.shields.io/badge/OpenRouter-6B21A8?style=for-the-badge)

#### Quality &amp; Delivery
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)

---

<a id="impact"></a>
### Impact

- 🚢 Took **ShipGuarde** from an empty repository to a live multi-tenant SaaS with paid plans, a public API, and a distributed GitHub Action
- ⚡ **40% latency cut** on a production GPT-4 assistant, by reading traces first and fixing what they pointed at: tokenization, Redis caching, query optimization
- 🏗️ **60% faster builds** from an NX micro-frontend migration that made a large codebase safely divisible across teams
- 📈 **Test coverage 65% → 92%**, with layered Jest, Cypress, and Playwright suites wired into CI/CD
- 🔌 **99.9% uptime** on Node.js microservices, plus ingestion connectors for **5+ external data platforms** including BigQuery and Snowflake
- 👥 Mentored **5+ engineers** through code review, design discussion, and career conversations
- 🌍 **8 years remote**, on European hours, for a Belgian company

---

### Currently Learning

- **Go** and **Rust.** My depth is TypeScript and Python, and these are the two I keep meeting at the edges of infrastructure work. I want them in production, not just in reading.
- Durable workflow orchestration (Temporal), coming from BullMQ
- Agent evaluation methodology beyond precision and recall

---

<a id="connect"></a>
### Connect

Open to senior and staff full-stack roles, remote and global. I read everything and reply properly.

- 🌐 [shubhamshrivastav.com](https://shubhamshrivastav.com)
- 🚢 [shipguarde.com](https://shipguarde.com)
- 💼 [LinkedIn](https://linkedin.com/in/shubhamshrivastav)
- 📧 [shrivastava.shubham219@live.com](mailto:shrivastava.shubham219@live.com)

---

### Education

**Bachelor of Engineering, Information Technology**
Lakshmi Narain College of Technology, Bhopal
*2012 to 2016*
