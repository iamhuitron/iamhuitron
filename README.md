# Ian Miguel Delgado Huitrón

<p align="left">
  <strong>Software Engineer & Systems Builder</strong> · Co-Founder & Tech Lead at <a href="https://github.com/Xaol-Studio"><strong>@Xaol-Studio</strong></a><br>
  Informatics Undergraduate at <strong>UNAM (FES Cuautitlán)</strong> · <strong>Google Student Ambassador 2026</strong>
</p>

<p align="left">
  <a href="https://portfolio-pink-five-jaih91sunw.vercel.app/"><img src="https://img.shields.io/badge/Live_Portfolio-2563eb?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://github.com/Xaol-Studio"><img src="https://img.shields.io/badge/Studio-@Xaol--Studio-059669?style=flat-square&logo=github&logoColor=white" alt="Xaol Studio" /></a>
  <a href="https://www.linkedin.com/in/ian-miguel-delgado-huitron-18b035349/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:ianhuitron0687@gmail.com"><img src="https://img.shields.io/badge/Email-ianhuitron0687@gmail.com-d97706?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Location-CDMX%20%2F%20Edo.%20M%C3%A9x-475569?style=flat-square" alt="Location" />
</p>

---

### Executive Profile

I design and engineer **deterministic software systems, high-speed client-side applications, and transactional data pipelines**. My technical background combines computer science fundamentals at UNAM with practical experience in municipal public accounting and internal audit. 

This gives me a concrete engineering edge: I build software with extreme discipline regarding **data integrity, financial arithmetic precision, zero-knowledge privacy, and offline performance**.

- **Co-Founder & Technical Lead** at [XAOL Software Studio](https://github.com/Xaol-Studio): Architecting custom web platforms, inventory management engines, and compliance tools for PyMEs and enterprises.
- **Google Student Ambassador 2026**: Leading technical workshops, AI developer initiatives, and student engineering communities across UNAM campus.
- **Engineering Philosophy**: Prefer client-side computation and local-first storage when privacy matters; enforce strict relational database constraints over loose application-level checks; design for sub-millisecond lookups and zero external runtime bloat.

---

### Engineering Stack

```
Core Languages:     TypeScript · Python · Go · Java · SQL (PostgreSQL, SQLite)
Frontend & Mobile:  Next.js (App Router) · React 19 · React Native / Expo (SDK 52) · Tailwind CSS
State & Storage:    Zustand · MMKV (Sub-ms) · IndexedDB · Web Workers · Redis
Systems & DevOps:   Docker · GitHub Actions (Automated CI/CD, Signed APKs) · Linux/Bash · Vercel
Domain Expertise:   Mexican SAT CFDI 4.0 / Anexo 20 · Art. 69-B EFOS Detection · Constraint Solvers
```

---

### Flagship Systems & Production Repositories

#### 🏢 [XAOL Software Studio](https://github.com/Xaol-Studio)
**Co-Founder & Lead Engineer** · *Commercial Software & Business Platforms*
- Independent software development studio building high-conversion capture websites, relational inventory/POS systems, and fiscal processors for Mexican businesses.
- Engineered 5 production-ready interactive simulators running client-side with zero cloud cold-starts: **PyME Manager** (SQL inventory), **MediCitas Pro** (medical scheduling), **SAT Sentinel** (tax auditor), **AutoQuote Pro** (wholesale quoting), and **FoodOrder Pro** (direct kitchen order dispatch).
- Architected the open-source [`pyme-manager-core`](https://github.com/Xaol-Studio/pyme-manager-core) engine: deterministic integer-cents financial math, SAT Anexo 20 tax reconciliation, and transactional POS cart state machines with native CI/CD.
- **Links:** [Organization](https://github.com/Xaol-Studio) · [Core Engine](https://github.com/Xaol-Studio/pyme-manager-core) · [Live Platform](https://xaol-website.vercel.app)

#### 🛡️ [CFDI Sentinel](https://github.com/iamhuitron/cfdi-sentinel)
**In-Browser CFDI 4.0 Fiscal Auditor & Anexo 20 Engine** · *TypeScript, Next.js 15, Web Workers, Vitest*
- 100% client-side zero-knowledge architecture: parses thousands of XMLs and ZIP packages in memory without transmitting sensitive financial records to external servers.
- Evaluates mathematical consistency of taxes, discounts, and retentions according to SAT Anexo 20 specifications.
- Screens suppliers in $O(1)$ time against the official Art. 69-B SAT blacklist (EFOS / simulated operations).
- **Links:** [Repository](https://github.com/iamhuitron/cfdi-sentinel) · [Live Demo](https://xaol-website.vercel.app/demo/sat-sentinel.html)

#### 🐍 [CFDI SAT Engine](https://github.com/iamhuitron/cfdi-sat-engine)
**High-Throughput Batch CFDI Validator & CLI** · *Python 3.10+, Standard Library, CI/CD*
- Lightweight, zero-dependency Python package and CLI engineered for server environments, ERP pipelines, and batch tax fraud prevention.
- Features automated GitHub Actions CI pipeline, multi-platform unit tests, and instant CSV/JSON report exports.
- **Links:** [Repository](https://github.com/iamhuitron/cfdi-sat-engine)

#### 📱 [FlowDay](https://github.com/iamhuitron/Flowday)
**Offline-First Mobile Productivity Suite** · *React Native, Expo SDK 52 (New Architecture), Zustand, MMKV*
- Sub-millisecond synchronous storage via native MMKV bindings, preventing UI hitching or state desynchronization.
- Automated delivery pipeline: GitHub Actions builds, tests, signs, and releases production APKs automatically on version tag.
- **Links:** [Repository](https://github.com/iamhuitron/Flowday) · [Web Demo](https://flowday-rho.vercel.app/)

#### 🗓️ [UniSched Optimizer](https://github.com/iamhuitron/UniSched-Optimizer)
**Combinatorial University Schedule Solver** · *TypeScript, React, pdf.js, Tesseract.js*
- Backtracking algorithm with constraint satisfaction that evaluates thousands of course/group combinations against user-defined time windows and free-day rules.
- Includes client-side OCR and raw PDF timetable parsing running entirely in the browser.
- **Links:** [Repository](https://github.com/iamhuitron/UniSched-Optimizer) · [Live Demo](https://uni-sched-optimizer.vercel.app/)

#### ⚓ [NetNaval](https://github.com/iamhuitron/NetNaval)
**Distributed Desktop Game & Real-Time Network Chat** · *Go, Wails v2, WebSockets*
- Cross-platform native desktop application packaging Go concurrency and network state with a modern web frontend.
- Resilient peer-to-peer and client-server socket protocol with automated game state recovery.
- **Links:** [Repository](https://github.com/iamhuitron/NetNaval)

---

### Technical Metrics & Commitments

- **100% Privacy by Design:** All financial tools operate client-side or on self-hosted infrastructure. Zero third-party telemetry on sensitive fiscal data.
- **Performance Benchmarks:** Sub-50ms query responses on local IndexedDB/MMKV schemas; zero-layout-shift UI architectures.
- **Continuous Delivery:** Strict CI/CD workflows across projects enforcing type checking, linting, and automated unit testing prior to merge.

---

### Contact & Collaboration

I am open to technical discussions, freelance engineering contracts through **XAOL Studio**, and select **Junior Software Engineer / Full Stack / FinTech** roles (Remote or Hybrid in CDMX / State of Mexico).

- **GitHub:** [@iamhuitron](https://github.com/iamhuitron)
- **Studio:** [github.com/Xaol-Studio](https://github.com/Xaol-Studio)
- **Email:** [ianhuitron0687@gmail.com](mailto:ianhuitron0687@gmail.com)
- **LinkedIn:** [Ian Miguel Delgado Huitrón](https://www.linkedin.com/in/ian-miguel-delgado-huitron-18b035349/)
- **WhatsApp (Business / Studio):** [+52 593 126 9253](https://wa.me/525931269253)
