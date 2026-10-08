# Telis Technologies

**We build digital infrastructure for Africa's informal economy.**

---

## Who We Are

Telis Technologies is a product engineering organization based in Nairobi, Kenya. We design, build, and operate digital platforms that serve the informal economy the workers, communities, and micro-enterprises that power most of Africa's economic activity but remain largely excluded from formal digital systems.

We are a multi-product company. Each product is independently scoped, independently led, and independently shipped. All of them run on the same core platform, the same engineering standards, and the same distribution philosophy: meet people where they are, on the devices they already use.

---

## What We Do

We build infrastructure, not apps.

Our products span health financing, insurance intelligence, mobility, payments, community finance, and whatever comes next. The common thread is not the sector it is the user. Every product we ship serves someone who has been overlooked by traditional technology: a rider, a trader, a farmer, a chama member, a small business owner.

If it can be built on our core, and it serves the informal economy, it belongs in our portfolio.

---

## Product Portfolio

| Product | Vertical | Status |
|---|---|---|
| **Telis Health** | Community health financing | In Design |
| **Telis Shield** | Insurance fraud intelligence | In Design |
| **Telis Ride** | Mobility and rider ecosystems | Planned |
| **Telis Pay** | Payments and cross-border rails | Planned |
| **Telis Core** | Shared platform powering all products | In Design |
| *Additional products* | *To be announced* | *Pipeline* |

Each product has its own repository, roadmap, and team. Telis Core is the shared foundation every product builds on.

---

## How We Build

Our engineering philosophy is simple: **build the core once, ship products fast.**

Every Telis product reuses the same identity system, the same payment rails, the same data layer, and the same access channels. A new product is not a new platform — it is a new configuration on top of what already exists.

```
┌─────────────────────────────────────────────────────────────┐
│                    PRODUCT LAYER                            │
│        Products ship here, fast and independently           │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│                   ACCESS LAYER                              │
│    USSD  │  SMS  │  WhatsApp  │  Agent  │  Partner API      │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│                    TELIS CORE                               │
│   Identity  │  Wallet  │  Payments  │  Data  │  Messaging  │
│   Auth  │  Events  │  Storage  │  Analytics  │  APIs        │
└─────────────────────────────────────────────────────────────┘
                              │
┌─────────────────────────────────────────────────────────────┐
│                    INTEGRATIONS                             │
│   Mobile Money  │  Banks  │  Government  │  Global Rails   │
└─────────────────────────────────────────────────────────────┘
```

**The principle:** 70% of every product is already built. We only build the 30% that is new.

---

## Technology Stack

| Layer | Technologies |
|---|---|
| **Backend** | Java 17+, Spring Boot 3.x, Spring Cloud, Spring Security |
| **Messaging** | Apache Kafka, Spring Cloud Stream |
| **Databases** | PostgreSQL, Redis, MongoDB, TimescaleDB |
| **Search** | Elasticsearch |
| **ML/AI** | Python, TensorFlow, scikit-learn, MLflow |
| **Frontend** | React, React Native, Next.js |
| **Infrastructure** | Docker, Kubernetes, GitHub Actions, ArgoCD |
| **Observability** | Prometheus, Grafana, ELK Stack, OpenTelemetry |
| **Security** | OAuth2, OIDC, mTLS, HashiCorp Vault |

We choose boring, proven technology and use it extremely well. Novelty is not a virtue in infrastructure.

---

## Engineering Principles

These are non-negotiable across every Telis repository and every Telis product.

**API-first.** Every capability is an API before it is a UI. Interfaces are contracts. Contracts are versioned. Versions are respected.

**Shared core, independent products.** Products do not share code directly. They share services through Telis Core. If two products need the same thing, it goes in Core.

**Event-driven by default.** Services communicate through events, not direct calls, wherever possible. Decoupling is survival.

**Inclusion is a technical requirement.** USSD is a primary channel, not a fallback. Low-bandwidth, offline-tolerant, feature-phone-compatible design is the default, not an afterthought.

**Privacy by design.** We handle data that can ruin lives if mishandled. Consent, encryption, minimization, and local hosting are requirements, not preferences.

**Ship small, ship often.** Large releases hide failures. Small releases surface them. We deploy continuously and learn continuously.

**Document everything.** If it is not documented, it does not exist. Documentation is a deliverable, not an afterthought.

**Measure before optimizing.** No performance work without a benchmark. No architecture change without a metric. No product decision without data.

---

## Repository Standards

Every repository under Telis Technologies must meet these standards.

| Requirement | Detail |
|---|---|
| **README** | Every repo explains its purpose, setup, and usage |
| **LICENSE** | Every repo has an explicit license |
| **`.gitignore`** | Every repo excludes build artifacts and secrets |
| **CI/CD** | Every repo has automated build, test, and deploy pipelines |
| **Tests** | Every service has unit and integration tests |
| **Health checks** | Every service exposes health and readiness endpoints |
| **Structured logging** | Every service emits structured, queryable logs |
| **Metrics** | Every service exposes Prometheus-compatible metrics |
| **API specs** | Every API has an OpenAPI specification |
| **Migrations** | Every database change is a versioned migration |
| **Security scans** | Every PR passes dependency and secret scanning |

Repositories that do not meet these standards are not production-ready.

---

## Organization Repositories

| Repository | Purpose | Visibility |
|---|---|---|
| `.github` | Organization profile, templates, community health | Public |
| `telis-core` | Shared platform services | Private |
| `telis-health` | Community health financing product | Private |
| `telis-shield` | Insurance fraud intelligence product | Private |
| `telis-ride` | Mobility and rider ecosystem product | Private |
| `telis-pay` | Payments and cross-border rails product | Private |
| `telis-infra` | Infrastructure-as-code and deployment | Private |
| `telis-docs` | Technical documentation and specs | Private |
| `telis-design` | Design system and brand assets | Private |
| `telis-sdk` | Client SDKs and developer tooling | Private |

---

## Roadmap

**Year 1 — Foundation**
Build Telis Core. Ship the first product. Establish engineering standards, CI/CD, and security baseline.

**Year 2 — Expansion**
Scale the first product. Launch a second product on the same core. Prove the multi-product model.

**Year 3 — Payments & Region**
Launch payments infrastructure. Expand to new markets. Open APIs to third-party developers.

**Year 4 — Platform**
Full product suite live across multiple markets. Telis Core becomes the default infrastructure layer for the informal economy.

---

## Contributing

We welcome contributions from engineers, designers, and domain experts who share our mission.

**Before contributing:**
1. Read the [Contributing Guide](CONTRIBUTING.md)
2. Review the [Code of Conduct](CODE_OF_CONDUCT.md)
3. Check open issues and project boards
4. Understand the engineering principles above

**What we look for:**
- Clarity over cleverness
- Tests over assertions
- Documentation over assumptions
- Small PRs over large ones
- Questions over silence

---

## Security

We take security seriously. If you discover a vulnerability, report to Telis Org and receive a bug bounty. Do not open public issues for security matters.

---

## Contact

| Channel | Details |
|--Coming soon |

---

## License

Unless otherwise specified, all repositories under Telis Technologies are proprietary and confidential.

---

## The Five

Telis was not born in a boardroom. It was born from five people who decided to build something that outlasts them.

The name is not a word. It is an acronym. Every letter is an initial — a signature — a promise made by one of the five founders who started this.

- **T** — Tristan
- **E** — Eugene
- **L** — Lameck
- **I** — Ingrid
- **S** — Silas

We started as five. We will scale as many. But the name will always carry the five who began.

We do not claim to have all the answers. We claim to have the resolve to find them. We will iterate, we will fail forward, and we will keep building until the infrastructure we imagined becomes the standard others build on.

**We will strive. We will achieve. We will conquer ; not markets, but problems. Not competitors, but the barriers that keep ordinary people locked out of systems built for someone else.**

This is where Telis came from. This is what we carry forward.

**T · E · L · I · S**

*Five founders. One mission. Building for the people who were never the target audience.*

**Telis Technologies**

*Build the core once. Ship products that matter.*