# Ian Miguel Delgado Huitrón

<p align="left">
  <strong>Data & Software Engineer · Systems Builder</strong> · Co-Founder & Tech Lead at <a href="https://github.com/Xaol-Studio"><strong>@Xaol-Studio</strong></a><br>
  Informatics Undergraduate at <strong>UNAM (FES Cuautitlán)</strong> · <strong>Google Student Ambassador 2026</strong>
</p>

<p align="left">
  <a href="https://iamhuitron.vercel.app/"><img src="https://img.shields.io/badge/Live_Portfolio-10b981?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://github.com/Xaol-Studio"><img src="https://img.shields.io/badge/Studio-@Xaol--Studio-059669?style=flat-square&logo=github&logoColor=white" alt="Xaol Studio" /></a>
  <a href="https://www.linkedin.com/in/ian-miguel-delgado-huitron-18b035349/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:ianhuitron0687@gmail.com"><img src="https://img.shields.io/badge/Email-ianhuitron0687@gmail.com-d97706?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Location-CDMX%20%2F%20Edo.%20M%C3%A9x-475569?style=flat-square" alt="Location" />
</p>

---

### Executive Profile

I engineer **high-performance data pipelines, embedded OLAP engines, and deterministic software systems**. My technical foundation combines computer science at UNAM with practical experience in municipal public accounting and fiscal auditing.

Currently, I specialize in **Data Engineering & Applied Analytics**, designing scalable data lakes, zero-copy columnar ingestion pipelines (Apache Arrow + DuckDB + Parquet), and econometric time-series models for Mexican financial and retail markets.

- **Data Engineering & FinTech Core**: Building high-throughput ETL engines for Mexican SAT CFDI 4.0 XMLs, Banxico macroeconomic series, and transactional PyME retail datasets with zero external runtime expenses ($0 budget architectures).
- **Co-Founder & Technical Lead** at [XAOL Software Studio](https://github.com/Xaol-Studio): Architecting custom web platforms, relational inventory/POS engines, and compliance tools for Mexican businesses.
- **Google Student Ambassador 2026**: Organizing technical workshops, developer conferences, and AI/data initiatives across UNAM campus.
- **Engineering Principles**: Columnar-first storage (Parquet/Arrow); embedded analytical SQL (DuckDB); zero-knowledge client-side computation; strict automated test coverage across all releases.

---

### Engineering & Data Stack

```
Data Engineering:    DuckDB (OLAP) · Apache Arrow (PyArrow) · Parquet · Hive Partitioning · Streaming XML (lxml)
Data Science:        Pandas · NumPy · RFM Segmentation · ABC Pareto Analysis · Market Basket (Apriori) · Econometrics
Languages:           Python 3.10+ · TypeScript · SQL (PostgreSQL, SQLite, DuckDB) · Go · Java · PHP
Web & Mobile:        Next.js 15/16 (App Router) · React 19 · React Native / Expo (SDK 52) · Tailwind CSS
State & Storage:     Zustand · MMKV · IndexedDB · Web Workers · Zero-Knowledge Local-First
Systems & DevOps:    GitHub Actions CI/CD · Docker · Linux/Bash · Git · Pytest · Vitest
Domain Expertise:    Mexican SAT CFDI 4.0 / Anexo 20 · SAT Art. 69-B EFOS Detection · Banxico SIE API · IMSS 2026
```

---

### Flagship Data Engineering & Analytics Systems

#### ⚡ [SAT Data Pipeline](https://github.com/iamhuitron/sat-data-pipeline)
**High-Performance XML-to-Parquet ETL & DuckDB Analytics Engine** · *Python 3.12, DuckDB, Apache Arrow, Parquet, pytest*
- Ingests bulk Mexican SAT CFDI 4.0 XML invoices via memory-constant chunked XML parsing (`lxml`).
- Batches records into zero-copy Apache Arrow tables, persisting into Hive-partitioned columnar Parquet lakes (`year=YYYY/month=MM`).
- Executes sub-second analytical SQL queries over hundreds of thousands of fiscal records using an embedded DuckDB OLAP engine.
- Instant $O(1)$ hash cross-referencing against the official Mexican SAT Article 69-B EFOS (shell company) blacklist.
- **Links:** [Repository](https://github.com/iamhuitron/sat-data-pipeline)

#### 📈 [Banxico Series Pipeline](https://github.com/iamhuitron/banxico-series-pipeline)
**Automated Macroeconomic ETL & Econometric Time-Series Engine** · *Python 3.12, DuckDB, Apache Arrow, Parquet, pytest*
- Automated data pipeline extracting official Mexican central bank indicators (USD/MXN FIX, TIIE 28d, UDIS, INPC inflation) from the Banxico SIE API.
- Stores historical time-series in an embedded DuckDB data lake with partitioned Parquet backing.
- Codifies econometric routines: automated Fisher equation calculation (nominal TIIE vs. YoY INPC inflation to compute real interest rates) and cross-series Pearson correlation matrices.
- **Links:** [Repository](https://github.com/iamhuitron/banxico-series-pipeline)

#### 🛒 [PyME Data Analytics](https://github.com/iamhuitron/pyme-data-analytics)
**Transactional Retail Data Science & Inventory Intelligence** · *Python 3.12, DuckDB, PyArrow, Parquet, pytest*
- Production-grade data analytics engine converting raw transactional sales and stock histories into operational business intelligence for Mexican PyMEs.
- Quantile-based RFM (Recency, Frequency, Monetary) customer segmentation with behavioral cohort categorization (*Champions, Loyal, At Risk, Hibernating*).
- ABC Pareto (80/20) inventory classification, statistical Reorder Point (ROP) calculation, and Market Basket association rules (Apriori Support, Confidence, Lift).
- **Links:** [Repository](https://github.com/iamhuitron/pyme-data-analytics)

#### 🏛️ [Statix](https://github.com/iamhuitron/Statix)
**Municipal Fiscal Audit Analytics & Automated PDF Reconciliation** · *Python, Streamlit, ReportLab, Pandas, pytest*
- Born directly out of municipal government accounting experience: automates invoice reconciliation and municipal ledger matching.
- Generates structured, audit-ready compliance PDF reports programmatically with ReportLab.
- Comprehensive 42-test pytest suite guaranteeing calculation accuracy across tax brackets and ledger entries.
- **Links:** [Repository](https://github.com/iamhuitron/Statix)

---

### Software Engineering & Client-Side Systems

#### 🏢 [XAOL Software Studio](https://github.com/Xaol-Studio)
**Co-Founder & Lead Engineer** · *Commercial Software & Business Platforms*
- Independent software development studio building capture websites, relational inventory/POS engines, and fiscal processors for Mexican businesses.
- Architected the open-source [`pyme-manager-core`](https://github.com/Xaol-Studio/pyme-manager-core) engine: deterministic integer-cents financial math, SAT Anexo 20 tax reconciliation, and transactional POS cart state machines with native CI/CD.
- **Links:** [Organization](https://github.com/Xaol-Studio) · [Core Engine](https://github.com/Xaol-Studio/pyme-manager-core) · [Live Platform](https://xaol-website.vercel.app)

#### 🛡️ [CFDI Sentinel](https://github.com/iamhuitron/cfdi-sentinel)
**In-Browser CFDI 4.0 Fiscal Auditor & SAT Art. 69-B Sentinel** · *TypeScript, Next.js 15, Web Workers, Vitest*
- 100% client-side zero-knowledge architecture: parses thousands of XMLs and ZIP packages in memory without transmitting sensitive financial records to external servers.
- Screens suppliers in $O(1)$ time against the official Art. 69-B SAT blacklist (EFOS / simulated operations) and validates Anexo 20 tax formulas.
- **Links:** [Repository](https://github.com/iamhuitron/cfdi-sentinel) · [Live Demo](https://xaol-website.vercel.app/demo/sat-sentinel.html)

#### 💼 [Nomina-Matrix](https://github.com/iamhuitron/nomina-matrix)
**Mexican Payroll Reverse-Engineering (Net-to-Gross) & IMSS 2026 Labor Suite** · *Next.js 15, TypeScript, SheetJS, Vitest*
- Inverts progressive Mexican income tax curves (ISR Art. 96) via sub-cent binary search convergence in < 25 iterations.
- Full compliance with 2026 progressive IMSS pension quotas and statutory LFT termination calculations.
- **Links:** [Repository](https://github.com/iamhuitron/nomina-matrix)

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

---

### Technical Metrics & Commitments

- **100% Zero-Cost / High Efficiency:** All data pipelines and analytics suites run on local, embedded engines (DuckDB, Parquet, PyArrow) without incurring expensive cloud or managed database bills.
- **100% Privacy by Design:** Financial and fiscal tools operate client-side or on self-hosted infrastructure. Zero third-party telemetry on sensitive fiscal data.
- **Automated Verification:** Strict CI/CD workflows across projects enforcing multi-version testing, type checking, linting, and automated unit testing prior to merge.

---

### Contact & Collaboration

I am open to technical discussions, freelance engineering contracts through **XAOL Studio**, and select **Data Engineer / Data Analyst / Software Engineer** roles (Remote or Hybrid in CDMX / State of Mexico).

- **GitHub:** [@iamhuitron](https://github.com/iamhuitron)
- **Studio:** [github.com/Xaol-Studio](https://github.com/Xaol-Studio)
- **Email:** [ianhuitron0687@gmail.com](mailto:ianhuitron0687@gmail.com)
- **LinkedIn:** [Ian Miguel Delgado Huitrón](https://www.linkedin.com/in/ian-miguel-delgado-huitron-18b035349/)
- **WhatsApp (Business / Studio):** [+52 593 126 9253](https://wa.me/525931269253)
