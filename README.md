<!-- Banner -->
![header](https://capsule-render.vercel.app/api?type=waving&color=0:0052CC,100:6D28D9&height=230&section=header&text=Dhanesh%20M&fontSize=55&fontAlignY=28&desc=Full-Stack%20Engineer%20%E2%80%A2%20Solo%20SaaS%20Founder%20%E2%80%A2%20Open%20Source%20Builder&descSize=16&descAlignY=52&fontColor=FFFFFF)

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3000&pause=1200&color=A78BFA&center=true&vCenter=true&multiline=true&width=650&height=80&lines=Building+ECODrIx+%E2%80%94+Multi-tenant+SaaS+for+Indian+SMBs;WhatsApp+CRM+%C2%B7+AI+Lead+Gen+%C2%B7+Booking+%C2%B7+Payments+%C2%B7+All+in+One+API" alt="Typing SVG" />

<br/>

[![Portfolio](https://img.shields.io/badge/portfolio.ecodrix.com-0052CC?style=for-the-badge&logo=googlechrome&logoColor=white)](https://portfolio.ecodrix.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhanesh-mekalthuru-5baa9323b/)
[![npm](https://img.shields.io/badge/@ecodrix-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/~ecodrix)
[![Buy Me Coffee](https://img.shields.io/badge/Support_My_Work-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/dhanesh1232)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=dhanesh1232&color=6D28D9&style=flat-square&label=Profile+Views)
&nbsp;
![GitHub followers](https://img.shields.io/github/followers/dhanesh1232?style=flat-square&color=0052CC&label=Followers)
&nbsp;
![GitHub stars](https://img.shields.io/github/stars/dhanesh1232?style=flat-square&color=FFDD00&label=Total+Stars)

</div>

---

## 👋 Who I Am

Self-taught full-stack engineer from India 🇮🇳 building production SaaS systems solo.

I design **multi-tenant architectures**, ship **published npm packages**, build **AI-powered automation engines**, and deploy to production every day. My work spans from low-level job queue systems to polished React component libraries.

**Not just coding — building a business.** ECODrIx is a real product serving real clients, handling real WhatsApp messages, processing real payments.

<details>
<summary>💬 <b>Ask me about</b></summary>
<br/>

- Multi-tenant SaaS architecture (dual-database strategy, tenant isolation)
- WhatsApp Cloud API integration (webhooks, templates, bulk messaging)
- Building custom job queue systems without Redis
- AI-powered lead generation and scoring pipelines
- Publishing and maintaining npm packages (SDK generation from OpenAPI)
- Event-driven automation engines with variable resolution
- Browser automation at scale (Playwright, proxy rotation, session isolation)
- Scaling a solo SaaS from 0 → paying clients

</details>

---

## 🔥 Currently Shipping

```diff
+ 🚀 LAIE v2 — AI lead scoring with multi-model fallback (Claude → GPT-4 → Gemini)
+ 📦 @ecodrix/erix-react v0.2.3 — CRM + Analytics + WhatsApp React components
+ 🌐 Public API docs — OpenAPI 3.1 spec with auto-generated SDK
+ 🧪 Browser automation actors — Playwright + proxy rotation + session isolation
! 🎯 Next: Client self-serve dashboard with no-code automation builder
```

---

## 🏗️ Flagship: ECODrIx Platform

> **Multi-tenant business automation platform** — WhatsApp CRM, AI lead generation, booking, payments, and email marketing through a single API.


<!-- 
  📸 DEMO GIF PLACEHOLDER
  To add: Record a 15-second screen capture of your admin panel or WhatsApp CRM,
  convert to GIF using https://gifcap.dev or CloudConvert,
  upload to your repo, and uncomment the line below:
-->
<!-- <div align="center"><img src="./assets/demo.gif" width="80%" alt="ECODrIx Demo" /></div> -->

### 🧬 System Architecture

```mermaid
graph TB
    subgraph Clients["Client Apps"]
        A1[Admin Panel<br/>Next.js 16]
        A2[SaaS Dashboard<br/>Next.js 15]
        A3[LAIE Frontend<br/>Next.js 16]
        A4[Client Websites<br/>@ecodrix/chatbot]
    end

    subgraph API["API Layer"]
        B1[Express 5 Server<br/>Multi-tenant Auth]
        B2[OpenAPI Spec<br/>Auto-generated SDK]
        B3[Rate Limiter<br/>Per-tenant + IP]
    end

    subgraph Core["Core Services"]
        C1[Automation Engine<br/>EventBus + Rules]
        C2[WhatsApp Service<br/>Meta Cloud API]
        C3[Email Service<br/>AWS SES + Postmark]
        C4[Booking Engine<br/>Google Calendar]
        C5[Payment Service<br/>Razorpay]
        C6[LAIE AI Engine<br/>Claude/GPT-4/Gemini]
    end

    subgraph Workers["Background Workers"]
        D1[ErixJobs Queue<br/>MongoDB-backed]
        D2[CRM Worker<br/>Actions Executor]
        D3[Actor Runner<br/>Browser Automation]
        D4[Webhook Worker<br/>HMAC Delivery]
    end

    subgraph Data["Data Layer"]
        E1[(Central DB<br/>System Config)]
        E2[(Tenant DBs<br/>Isolated per Client)]
        E3[(PostgreSQL<br/>LAIE Metadata)]
        E4[(Redis<br/>Cache + Sessions)]
        E5[(AWS S3<br/>Media Storage)]
    end

    subgraph External["External APIs"]
        F1[Meta WhatsApp]
        F2[Google Meet]
        F3[Razorpay]
        F4[AWS Bedrock]
        F5[Anthropic/OpenAI]
    end

    A1 & A2 & A3 & A4 --> B1
    B1 --> B2
    B1 --> B3
    B1 --> C1 & C2 & C3 & C4 & C5 & C6
    C1 --> D1
    D1 --> D2 & D3 & D4
    C2 --> F1
    C4 --> F2
    C5 --> F3
    C6 --> F4 & F5
    B1 --> E1 & E2
    C6 --> E3
    D1 --> E4
    C3 --> E5

    style Clients fill:#1a1b26,stroke:#7aa2f7,color:#c0caf5
    style API fill:#1a1b26,stroke:#bb9af7,color:#c0caf5
    style Core fill:#1a1b26,stroke:#9ece6a,color:#c0caf5
    style Workers fill:#1a1b26,stroke:#e0af68,color:#c0caf5
    style Data fill:#1a1b26,stroke:#f7768e,color:#c0caf5
    style External fill:#1a1b26,stroke:#73daca,color:#c0caf5
```

### ⚡ Automation Flow — How a Trigger Becomes an Action

```mermaid
sequenceDiagram
    participant Client as Client Website
    participant API as Express API
    participant Auth as Tenant Auth
    participant Engine as Automation Engine
    participant Queue as ErixJobs Queue
    participant Worker as CRM Worker
    participant WA as WhatsApp API
    participant Email as AWS SES

    Client->>API: POST /api/saas/workflows/trigger
    API->>Auth: validateClientKey (API key → clientCode)
    Auth-->>API: ✅ Tenant identified
    API->>API: Create EventLog + Find/Create Lead
    API->>Engine: EventBus.emit('lead_created', context)
    Engine->>Engine: Match AutomationRules (trigger + conditions)
    Engine->>Queue: enqueueDelayedAction(actions[])
    Queue->>Worker: Poll & execute (concurrency: 3)
    
    alt Action: send_whatsapp
        Worker->>WA: Resolve variables → Send template
        WA-->>Worker: ✅ Delivered
    else Action: send_email
        Worker->>Email: Render template → SES send
        Email-->>Worker: ✅ Sent
    end
    
    Worker->>API: Update EventLog { status: "completed" }
```

<table>
<tr>
<td width="50%">

### Architecture Highlights
- **Dual-database multi-tenancy** — Central DB for system config + isolated tenant DBs per client
- **Custom job queue** (ErixJobs) — MongoDB-backed, no Redis dependency, retry with exponential backoff
- **Event-driven automation** — Trigger → Rule Match → Context Resolution → Action Execution
- **Real-time layer** — Socket.IO for live WhatsApp inbox updates
- **API-first** — OpenAPI spec, auto-generated SDK, per-tenant rate limiting
- **Idempotency middleware** — Prevents duplicate webhook processing

</td>
<td width="50%">

### System Scale
- **10+ microservices** across 4 frontend apps + 1 monolithic backend
- **Published npm packages** — `@ecodrix/erix-api`, `@ecodrix/erix-react`, `@ecodrix/chatbot`
- **10k+ contacts** per bulk WhatsApp campaign via queue processing
- **Tenant isolation** at every layer — DB, API, auth, CORS, rate limits
- **5 AI models** — Claude, GPT-4, Gemini, Vertex AI, AWS Bedrock
- **Webhook HMAC signing** — All outbound callbacks cryptographically verified

</td>
</tr>
</table>

---

### 📦 Live Modules

| Module | What It Does | Key Tech |
|--------|-------------|----------|
| 🔵 **Multi-Tenant Core** | Tenant-scoped APIs, dynamic DB connections, custom field registry | MongoDB, Connection Pooling, Zod |
| 📱 **WhatsApp CRM** | Message threading, contact management, template sending via Cloud API | Meta Cloud API, Socket.IO, Webhooks |
| 📨 **Bulk Sender** | Excel upload → E.164 normalize → queue → 10k+ contacts delivered | ErixJobs, Bull Queue, Worker Threads |
| 🤖 **LAIE (AI Engine)** | AI lead qualification, scoring, enrichment, autonomous research | Claude/GPT-4/Gemini, Playwright, Crawlee |
| 📧 **Email Marketing** | Campaign builder, SES integration, domain verification, compliance gates | AWS SES, Postmark, DKIM/SPF |
| 📅 **Booking Engine** | Slot availability, real-time booking, conflict prevention, Meet auto-create | Google Calendar API, Razorpay |
| 💳 **Payments** | Order creation, webhook verification, appointment-payment linking | Razorpay, HMAC Webhooks |
| 🎯 **Automation Engine** | Event-driven rules, sequences, variable resolution, delayed actions | EventBus, Handlebars, Cron |
| 📊 **Analytics** | Business metrics, campaign performance, funnel tracking | Recharts, Aggregation Pipelines |
| 🌐 **Browser Automation** | Headless scraping, proxy rotation, session isolation, actor runtime | Playwright, Puppeteer, Crawlee |
| 🔐 **Security Layer** | Plan guards, quota enforcement, storage limits, CORS allowlists | JWT, HMAC, Rate Limiting |


---

### 💡 Code Showcase

<details>
<summary><b>🔌 Tenant Connection Manager — How multi-tenancy works at the DB level</b></summary>

```typescript
// Every tenant gets their own isolated MongoDB connection
// Connections are pooled and cached — no cold starts after first request

const connectionCache = new Map<string, mongoose.Connection>();

export async function getTenantConnection(clientCode: string): Promise<mongoose.Connection> {
  if (connectionCache.has(clientCode)) {
    return connectionCache.get(clientCode)!;
  }

  const dataSource = await ClientDataSource.findOne({ clientCode });
  if (!dataSource) throw new TenantNotFoundError(clientCode);

  const conn = await mongoose.createConnection(dataSource.mongoUri, {
    maxPoolSize: 10,
    serverSelectionTimeoutMS: 5000,
  }).asPromise();

  connectionCache.set(clientCode, conn);
  return conn;
}

// Usage — tenant data never leaks across clients
const { Lead, Pipeline, AutomationRule } = await getCrmModels(clientCode);
const leads = await Lead.find({ status: "qualified" }); // Always scoped to tenant
```

</details>

<details>
<summary><b>🤖 Automation Rule Engine — Event-driven action execution</b></summary>

```typescript
// When a trigger fires, the engine matches rules and executes actions

export async function runAutomations(clientCode: string, trigger: string, context: TriggerContext) {
  const { AutomationRule } = await getCrmModels(clientCode);
  
  // Find all active rules matching this trigger
  const rules = await AutomationRule.find({ 
    clientCode, 
    trigger, 
    isActive: true 
  });

  for (const rule of rules) {
    // Evaluate conditions against lead + event context
    if (!evaluateCondition(rule.condition, context)) continue;

    if (rule.isSequence) {
      await enrollInSequence(clientCode, rule, context.lead);
    } else {
      for (const action of rule.actions) {
        await enqueueDelayedAction({
          clientCode,
          action,
          context,
          delay: action.delaySeconds ?? 0,
        });
      }
    }
  }
}
```

</details>

<details>
<summary><b>📨 Variable Resolution — Dynamic template rendering</b></summary>

```typescript
// Resolves {{lead.firstName}}, {{event.productName}}, {{resolved.meetLink}}

export class VariableResolver {
  private layers: Map<string, Record<string, unknown>>;

  constructor(lead: Lead, event: TriggerPayload, derived: DerivedContext) {
    this.layers = new Map([
      ["lead", lead.toObject()],        // {{lead.firstName}}, {{lead.phone}}
      ["event", event.variables ?? {}],  // {{event.productName}}, {{event.amount}}
      ["resolved", derived],             // {{resolved.meetLink}}, {{resolved.today}}
    ]);
  }

  resolve(template: string): string {
    return template.replace(/\{\{(\w+)\.(\w+)\}\}/g, (_, layer, key) => {
      return String(this.layers.get(layer)?.[key] ?? "");
    });
  }
}

// "Hello {{lead.firstName}}, your meeting: {{resolved.meetLink}}"
// → "Hello Ravi, your meeting: https://meet.google.com/abc-def-ghi"
```

</details>

---

### 📚 Published npm Packages

| Package | Version | Downloads | Description |
|---------|---------|-----------|-------------|
| [`@ecodrix/erix-api`](https://www.npmjs.com/package/@ecodrix/erix-api) | ![npm](https://img.shields.io/npm/v/@ecodrix/erix-api?style=flat-square&color=CB3837) | ![downloads](https://img.shields.io/npm/dm/@ecodrix/erix-api?style=flat-square&color=0052CC) | Isomorphic SDK — WhatsApp, CRM, Storage, Meetings. Auto-generated from OpenAPI. |
| [`@ecodrix/erix-react`](https://www.npmjs.com/package/@ecodrix/erix-react) | ![npm](https://img.shields.io/npm/v/@ecodrix/erix-react?style=flat-square&color=CB3837) | ![downloads](https://img.shields.io/npm/dm/@ecodrix/erix-react?style=flat-square&color=0052CC) | Full React component library — Editor, CRM, Analytics, WhatsApp, Dashboard |
| [`@ecodrix/chatbot`](https://www.npmjs.com/package/@ecodrix/chatbot) | ![npm](https://img.shields.io/npm/v/@ecodrix/chatbot?style=flat-square&color=CB3837) | ![downloads](https://img.shields.io/npm/dm/@ecodrix/chatbot?style=flat-square&color=0052CC) | Lightweight embeddable chatbot widget — iframe-based, zero deps |
| [`erix`](https://www.npmjs.com/package/erix) | ![npm](https://img.shields.io/npm/v/erix?style=flat-square&color=CB3837) | ![downloads](https://img.shields.io/npm/dm/erix?style=flat-square&color=0052CC) | Git automation CLI — one-command commit, push, repo management |

**Quick install:**
```bash
# SDK for any JavaScript/TypeScript project
npm install @ecodrix/erix-api

# React components for dashboards
npm install @ecodrix/erix-react

# Git automation CLI (global)
npm install -g erix
```

---

## 🛠️ Tech Stack (What I Actually Use Daily)

<details open width="100%">
<summary><b>Full Stack Breakdown</b></summary>
<br/>

| Layer | Technologies |
|-------|-------------|
| **Frontend** | ![Next.js](https://img.shields.io/badge/Next.js_16-000?style=flat-square&logo=next.js) ![React](https://img.shields.io/badge/React_19-20232a?style=flat-square&logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript_5-3178C6?style=flat-square&logo=typescript&logoColor=white) ![TailwindCSS](https://img.shields.io/badge/Tailwind_4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) ![Radix UI](https://img.shields.io/badge/Radix_UI-161618?style=flat-square&logo=radixui&logoColor=white) |
| **Backend** | ![Node.js](https://img.shields.io/badge/Node.js_18+-339933?style=flat-square&logo=node.js&logoColor=white) ![Express](https://img.shields.io/badge/Express_5-000?style=flat-square&logo=express) ![Hono](https://img.shields.io/badge/Hono-E36002?style=flat-square&logo=hono&logoColor=white) ![Socket.io](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socket.io) ![Zod](https://img.shields.io/badge/Zod_4-3E67B1?style=flat-square&logo=zod&logoColor=white) |
| **Databases** | ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![Drizzle](https://img.shields.io/badge/Drizzle_ORM-C5F74F?style=flat-square&logo=drizzle&logoColor=black) |
| **AI/ML** | ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white) ![Anthropic](https://img.shields.io/badge/Claude-191919?style=flat-square&logo=anthropic&logoColor=white) ![Google AI](https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white) ![AWS Bedrock](https://img.shields.io/badge/Bedrock-FF9900?style=flat-square&logo=amazon-aws&logoColor=white) |
| **Cloud & Infra** | ![AWS](https://img.shields.io/badge/AWS_(S3,_SES,_Bedrock)-FF9900?style=flat-square&logo=amazon-aws&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000?style=flat-square&logo=vercel) ![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=white) ![Cloudflare](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white) |
| **DevOps** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white) ![PM2](https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=pm2&logoColor=white) |
| **Automation** | ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white) ![Puppeteer](https://img.shields.io/badge/Puppeteer-40B5A4?style=flat-square&logo=puppeteer&logoColor=white) ![Crawlee](https://img.shields.io/badge/Crawlee-00B388?style=flat-square&logo=apify&logoColor=white) |
| **APIs** | ![WhatsApp](https://img.shields.io/badge/WhatsApp_Cloud_API-25D366?style=flat-square&logo=whatsapp&logoColor=white) ![Razorpay](https://img.shields.io/badge/Razorpay-0052CC?style=flat-square&logo=razorpay&logoColor=white) ![Google Meet](https://img.shields.io/badge/Google_Meet_API-00897B?style=flat-square&logo=googlemeet&logoColor=white) |
| **Testing** | ![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white) ![Testing Library](https://img.shields.io/badge/Testing_Library-E33332?style=flat-square&logo=testinglibrary&logoColor=white) ![Biome](https://img.shields.io/badge/Biome-60A5FA?style=flat-square&logo=biome&logoColor=white) |

</details>

---

## ⚙️ How I Work

```mermaid
graph LR
    A[Idea] --> B[Design in Mermaid]
    B --> C[Build MVP]
    C --> D[Ship to Production]
    D --> E[Measure & Iterate]
    E --> A
    
    style A fill:#6D28D9,stroke:#A78BFA,color:#fff
    style B fill:#0052CC,stroke:#7aa2f7,color:#fff
    style C fill:#059669,stroke:#6ee7b7,color:#fff
    style D fill:#DC2626,stroke:#fca5a5,color:#fff
    style E fill:#D97706,stroke:#fcd34d,color:#fff
```

| Principle | How |
|-----------|-----|
| **Ship daily** | Every day has a commit. Small PRs, fast feedback loops. |
| **Design before code** | Mermaid diagrams, OpenAPI specs, and architecture docs come first. |
| **Automate everything** | CI/CD, SDK generation, linting, type checking — all automated. |
| **AI as a multiplier** | I use AI for code review, lead scoring, content generation — not as a crutch. |
| **Build in public** | Document decisions, share numbers, admit mistakes. |


---

## 📊 By The Numbers

<div align="center">

| Metric | Count |
|--------|-------|
| 🏗️ **Production Services** | 10+ microservices |
| 📦 **npm Packages Published** | 4 packages (public registry) |
| 🔌 **API Endpoints** | 80+ REST endpoints |
| 🗄️ **Database Models** | 30+ schemas (MongoDB + PostgreSQL) |
| 🤖 **AI Models Integrated** | 5 (Claude, GPT-4, Gemini, Bedrock, Vertex) |
| 📱 **WhatsApp Messages** | 10k+ per bulk campaign |
| 🧪 **Testing** | Vitest + Property-based (fast-check) |
| 🚀 **Deployment** | Daily via GitHub Actions + Render + Vercel |
| 🖥️ **Frontend Apps** | 4 (Admin, SaaS, LAIE, Portfolio) |
| 🔧 **Background Workers** | 4 (CRM, Actor, Webhook, Cron) |

</div>

---

## 🧠 What Sets Me Apart

<table>
<tr>
<td width="33%" valign="top">

### 🏭 Systems Thinking
I don't just write endpoints — I design **tenant-isolated architectures**, build **custom job queues**, implement **event-driven automation engines**, and handle **webhook signature verification** at scale.

</td>
<td width="33%" valign="top">

### 📦 Ship to npm
I publish and maintain **real packages** used in production. Auto-generated SDKs from OpenAPI specs, React component libraries with CSS isolation, embeddable widgets with zero dependencies.

</td>
<td width="33%" valign="top">

### 🤖 AI-Native Development
Every product I build integrates AI — from **lead scoring with Claude** to **autonomous web research agents** using Playwright + LLMs to **multi-model fallback chains**.

</td>
</tr>
</table>

---

## 📈 GitHub Stats

<div align="center">

<a href="https://github.com/dhanesh1232">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=dhanesh1232&theme=tokyonight" />
</a>

</div>

<div align="center">

<a href="https://github.com/dhanesh1232">
  <img width="49%" src="https://streak-stats.demolab.com/?user=dhanesh1232&theme=tokyonight&hide_border=true" />
</a>
<a href="https://github.com/dhanesh1232">
  <img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=dhanesh1232&theme=tokyonight&utcOffset=5.5" />
</a>

</div>

<div align="center">

<a href="https://github.com/dhanesh1232">
  <img width="32%" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=dhanesh1232&theme=tokyonight" />
</a>
<a href="https://github.com/dhanesh1232">
  <img width="32%" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=dhanesh1232&theme=tokyonight" />
</a>
<a href="https://github.com/dhanesh1232">
  <img width="32%" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=dhanesh1232&theme=tokyonight" />
</a>

</div>

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=dhanesh1232&theme=tokyo-night&hide_border=true&area=true)](https://github.com/dhanesh1232)

</div>

---

## 🗺️ ECODrIx Roadmap

```mermaid
timeline
    title ECODrIx Journey
    section 2025
        Q1-Q2 : Multi-tenant Core
               : WhatsApp CRM
               : Booking + Payments
               : Admin Panel
               : npm Packages Published
    section 2026
        Q1 : Public API Launch
           : 5 Clinic Clients
           : LAIE AI Engine v2
        Q2 : @ecodrix/erix-react
           : Component Library
           : Developer Docs
        Q3 : Client Self-Serve Dashboard
           : No-code Automation Builder
           : White-label Ready
    section 2027
        Multi-Vertical : Salons · Coaching · Legal
                       : Same stack, new templates
                       : 50+ Clients
    section 2028+
        Platform Era : Module Marketplace
                     : White-label Agency Network
                     : 100+ Clients
                     : Series A Ready
```

---

## 🏆 Trophies

<div align="center">

![](https://github-profile-trophy.vercel.app/?username=dhanesh1232&theme=discord&no-frame=true&no-bg=true&column=7&margin-w=8)

</div>

---

## 🏗️ Other Projects

| Project | Description | Stack |
|---------|-------------|-------|
| **[LAIE](https://github.com/dhanesh1232)** | AI-powered lead generation — qualification, scoring, enrichment, autonomous research agents | Next.js 16, Claude/GPT-4, Playwright, PostgreSQL, Drizzle |
| **[Erix Store](https://github.com/dhanesh1232)** | In-memory real-time data store with WebSocket sync & MessagePack serialization | Express, WebSockets, MessagePack, PostgreSQL |
| **[Erix CLI](https://github.com/dhanesh1232/erix)** | One-command Git automation — commit, push, manage repos with interactive prompts | Node.js, Inquirer, Octokit, Chalk, Zod |
| **[Portfolio](https://portfolio.ecodrix.com)** | Personal portfolio & blog | Next.js, TailwindCSS, Framer Motion |

---

## 🤝 Work With Me

<table>
<tr>
<td>🏥</td>
<td><b>ECODrIx Early Access</b></td>
<td>Indian clinics, salons, coaching businesses wanting WhatsApp + CRM + Payments automation</td>
</tr>
<tr>
<td>🧑‍💼</td>
<td><b>Technical Advisory</b></td>
<td>Founders building on WhatsApp Cloud API, multi-tenant SaaS, Node.js/TypeScript at scale</td>
</tr>
<tr>
<td>🏢</td>
<td><b>White-Label Partnership</b></td>
<td>Web agencies wanting to resell ECODrIx under their own brand</td>
</tr>
<tr>
<td>💻</td>
<td><b>Open Source</b></td>
<td>Contributors to Node.js · TypeScript · MongoDB · WhatsApp API ecosystem</td>
</tr>
<tr>
<td>🎙️</td>
<td><b>Build in Public</b></td>
<td>I document architecture decisions, revenue numbers, mistakes, and wins publicly</td>
</tr>
</table>

---

## 📣 Building in Public

I share the full journey — architecture decisions, scaling challenges, revenue milestones, and honest mistakes.

> *"The best way to learn is to build something real, ship it, and let the market tell you what's wrong."*

<div align="center">

[![LinkedIn](https://img.shields.io/badge/Follow_the_Journey-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhanesh-mekalthuru-5baa9323b/)
[![Instagram](https://img.shields.io/badge/Behind_the_Scenes-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/erix.__.after17_59/)
[![Portfolio](https://img.shields.io/badge/See_Everything-0052CC?style=for-the-badge&logo=googlechrome&logoColor=white)](https://portfolio.ecodrix.com/)
[![Coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/dhanesh1232)

</div>

---

<div align="center">

```
 ┌─────────────────────────────────────────────────────────────┐
 │                                                             │
 │   ECODrIx — Invisible Infrastructure for Indian SMBs        │
 │   Built solo · Shipped daily · Powered by AI leverage       │
 │                                                             │
 │   Dhanesh M · India 🇮🇳 · Building in public since 2025      │
 │                                                             │
 └─────────────────────────────────────────────────────────────┘
```

</div>

![footer](https://capsule-render.vercel.app/api?type=waving&color=0:6D28D9,100:0052CC&height=120&section=footer)
