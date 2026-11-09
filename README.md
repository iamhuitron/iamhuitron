<div align="left">

# Ian Miguel Delgado Huitrón

**Software & Data Engineer · Co-Founder & Technical Lead at [@Xaol-Studio](https://github.com/Xaol-Studio)**  
Informatics at **UNAM** (FES Cuautitlán) · **Google Student Ambassador 2026** · Mexico City / State of Mexico

<p align="left">
  <a href="https://iamhuitron.vercel.app/"><img src="https://img.shields.io/badge/PORTFOLIO-iamhuitron.vercel.app-B89758?style=for-the-badge&logo=vercel&logoColor=FAF8F5&labelColor=141210" alt="Portfolio" /></a>
  <a href="https://xaol-website.vercel.app/"><img src="https://img.shields.io/badge/STUDIO-XAOL_SOFTWARE_STUDIO-1D1A16?style=for-the-badge&logo=github&logoColor=D4B87A&labelColor=141210" alt="XAOL Studio" /></a>
  <a href="https://www.linkedin.com/in/iamhuitron"><img src="https://img.shields.io/badge/LINKEDIN-@iamhuitron-1D1A16?style=for-the-badge&logo=linkedin&logoColor=D4B87A&labelColor=141210" alt="LinkedIn" /></a>
  <a href="mailto:ianhuitron0687@gmail.com"><img src="https://img.shields.io/badge/CONTACT-ianhuitron0687@gmail.com-611624?style=for-the-badge&logo=gmail&logoColor=FAF8F5&labelColor=141210" alt="Email" /></a>
</p>

</div>

---

### `01` · Architectural Focus

I design and build **deterministic, zero-drift software systems and analytical data pipelines**. My work focuses on high-throughput Mexican fiscal auditing (**SAT CFDI 4.0 / Anexo 20 / Art. 69-B**), vectorized columnar storage (**Apache Parquet + DuckDB**), macroeconomic econometric engines (**Banxico SIE**), and sub-second client-side web and mobile applications.

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#141210', 'primaryTextColor': '#FAF8F5', 'primaryBorderColor': '#B89758', 'lineColor': '#B89758', 'secondaryColor': '#1D1A16', 'tertiaryColor': '#0D0C0A', 'mainBkg': '#141210', 'nodeBorder': '#B89758', 'clusterBkg': '#0D0C0A', 'clusterBorder': '#262420', 'titleColor': '#D4B87A', 'edgeLabelBackground': '#141210', 'fontFamily': 'JetBrains Mono, Plus Jakarta Sans, sans-serif' }}}%%
flowchart LR
    subgraph Sources["01 · Data & Fiscal Sources"]
        A1["CFDI 4.0 / 3.3 XML Streams"]
        A2["Banxico SIE Macro Series"]
        A3["POS & Retail Transactions"]
    end

    subgraph Core["02 · Deterministic Core & Lakehouse"]
        B1["Zero-Copy PyArrow & Parquet"]
        B2["Embedded DuckDB Vector SQL"]
        B3["Integer-Cents & Anexo 20 Math"]
    end

    subgraph Delivery["03 · Client & Edge Delivery"]
        C1["Next.js 16 / React 19 Web Apps"]
        C2["React Native + MMKV Mobile"]
        C3["Executive Audit & DIOT Exports"]
    end

    Sources --> Core --> Delivery
```

---

### `02` · Production Systems & Open-Source Registry

#### I. Data Engineering, ETL & Quantitative Analytics

| Repository | Architectural Scope | Stack & Verification |
| :--- | :--- | :--- |
| **[`sat-data-pipeline`](https://github.com/iamhuitron/sat-data-pipeline)** | **CFDI XML to Parquet ETL & DuckDB Engine**<br>Streams raw CFDI 4.0/3.3 XML batches into Hive-partitioned Apache Parquet (`año`/`mes`) with vectorized SQL KPIs and $O(1)$ Art. 69-B EFOS screening. | ![Python](https://img.shields.io/badge/Python-3.12-1D1A16?style=flat-square&logo=python&logoColor=D4B87A&labelColor=141210) ![DuckDB](https://img.shields.io/badge/DuckDB-Vector_SQL-1D1A16?style=flat-square&logo=duckdb&logoColor=D4B87A&labelColor=141210) ![Tests](https://img.shields.io/badge/Tests-Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |
| **[`banxico-series-pipeline`](https://github.com/iamhuitron/banxico-series-pipeline)** | **Macroeconomic Time-Series ETL (Banxico SIE)**<br>Harmonizes USD/MXN FIX, 28-day TIIE, UDIS, and INPC series. Computes YoY inflation, Fisher real interest rates ($r_t \approx i_t - \pi_t$), and Pearson correlation matrices. | ![Python](https://img.shields.io/badge/Python-3.12-1D1A16?style=flat-square&logo=python&logoColor=D4B87A&labelColor=141210) ![Arrow](https://img.shields.io/badge/PyArrow-Parquet-1D1A16?style=flat-square&logo=apachearrow&logoColor=D4B87A&labelColor=141210) ![Tests](https://img.shields.io/badge/Tests-Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |
| **[`pyme-data-analytics`](https://github.com/iamhuitron/pyme-data-analytics)** | **Retail Data Science & Inventory Optimization**<br>RFM customer quintile segmentation, ABC Pareto (80/20) revenue classification, Apriori market-basket lift rules, and Reorder Point (ROP) forecasting. | ![Python](https://img.shields.io/badge/Python-3.12-1D1A16?style=flat-square&logo=python&logoColor=D4B87A&labelColor=141210) ![Models](https://img.shields.io/badge/Models-RFM_/_ABC-B89758?style=flat-square&labelColor=141210&logoColor=FAF8F5) ![Tests](https://img.shields.io/badge/Tests-Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |
| **[`Statix`](https://github.com/iamhuitron/Statix)** | **Visual Fiscal Audit & Anomaly Detection Suite**<br>Interactive Streamlit & Plotly analytics suite with exact `Decimal` reconciliation, z-score ($\sigma > 2.5$) outlier detection, and multi-sheet `.xlsx` ledger exports. | ![Streamlit](https://img.shields.io/badge/Streamlit-1.42-1D1A16?style=flat-square&logo=streamlit&logoColor=D4B87A&labelColor=141210) ![Tests](https://img.shields.io/badge/Pytest-42_Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |

#### II. Fiscal Engineering, FinTech & Transactional Cores

| Repository | Architectural Scope | Stack & Verification |
| :--- | :--- | :--- |
| **[`cfdi-sat-engine`](https://github.com/iamhuitron/cfdi-sat-engine)** | **Zero-Dependency Python CFDI 4.0 Auditor & CLI**<br>100% Python stdlib fiscal engine. Validates Anexo 20 tax equations, RFC syntax, UUID format, and screens SAT Art. 69-B blacklists in $O(1)$ time. | ![Python](https://img.shields.io/badge/Stdlib-Zero_Deps-1D1A16?style=flat-square&logo=python&logoColor=D4B87A&labelColor=141210) ![SAT](https://img.shields.io/badge/SAT-Art._69B-611624?style=flat-square&labelColor=141210&logoColor=FAF8F5) ![CI](https://img.shields.io/badge/CI-Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |
| **[`cfdi-sentinel`](https://github.com/iamhuitron/cfdi-sentinel)** | **In-Memory Client-Side CFDI Auditor & DIOT Generator**<br>Zero-knowledge browser auditing for `.xml` and `.zip` invoice batches. Computes VAT/ISR balances, flags 72h PAC delays, and exports `.xlsx` workbooks. | ![Next.js](https://img.shields.io/badge/Next.js_15-React_19-1D1A16?style=flat-square&logo=next.js&logoColor=D4B87A&labelColor=141210) ![Demo](https://img.shields.io/badge/Live-Demo-B89758?style=flat-square&labelColor=141210&logoColor=FAF8F5) |
| **[`nomina-matrix`](https://github.com/iamhuitron/nomina-matrix)** | **Net-to-Gross Payroll Solver & IMSS 2026 Matrix**<br>Binary search solver converging to exact gross salary ($\pm \$0.005\text{ MXN}$) in $< 25$ iterations, 5-branch IMSS employer burden, and LFT Art. 48/50 severance. | ![TypeScript](https://img.shields.io/badge/TypeScript-5.7-1D1A16?style=flat-square&logo=typescript&logoColor=D4B87A&labelColor=141210) ![Vitest](https://img.shields.io/badge/Vitest-12_Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |
| **[`pyme-manager-core`](https://github.com/Xaol-Studio/pyme-manager-core)** | **Deterministic POS, Inventory & Tax Core (`@Xaol-Studio`)**<br>Integer-cents financial engine preventing IEEE 754 float drift, multi-tier pricing (`RETAIL`/`WHOLESALE`/`MECHANIC`), and PostgreSQL/SQLite schemas. | ![TypeScript](https://img.shields.io/badge/TypeScript-SQL-1D1A16?style=flat-square&logo=postgresql&logoColor=D4B87A&labelColor=141210) ![CI](https://img.shields.io/badge/CI-Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |

#### III. Cross-Platform Applications, SaaS & Combinatorial Solvers

| Repository | Architectural Scope | Stack & Verification |
| :--- | :--- | :--- |
| **[`Flowday`](https://github.com/iamhuitron/Flowday)** | **Offline-First Productivity Suite & Native Android Widgets**<br>Built with React Native 0.76 + Expo SDK 52 (New Architecture), sub-millisecond `react-native-mmkv` persistence, custom Kotlin AppWidgets, and CI APK releases. | ![Expo](https://img.shields.io/badge/Expo_52-React_Native-1D1A16?style=flat-square&logo=expo&logoColor=D4B87A&labelColor=141210) ![Web](https://img.shields.io/badge/Live-Web_&_APK-B89758?style=flat-square&labelColor=141210&logoColor=FAF8F5) |
| **[`UniSched-Optimizer`](https://github.com/iamhuitron/UniSched-Optimizer)** | **Combinatorial University Schedule Solver & Local OCR**<br>Backtracking CSP solver with geometric table reconstruction (`pdfjs-dist` + WebAssembly `tesseract.js`) and verified UNAM / IPN / UAM datasets. | ![TypeScript](https://img.shields.io/badge/Next.js-Wasm_OCR-1D1A16?style=flat-square&logo=typescript&logoColor=D4B87A&labelColor=141210) ![Tests](https://img.shields.io/badge/Vitest-35_Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |
| **[`mj-cafe`](https://github.com/Xaol-Studio/mj-cafe)** | **Specialty Coffee Pre-Order SaaS & Barista KDS (`@Xaol-Studio`)**<br>3NF relational database (`MySQL`/`SQLite`), PHP PDO transactional API, digital loyalty stamp engine, and real-time Kitchen Display System. | ![PHP](https://img.shields.io/badge/PHP_8-PDO_SQL-1D1A16?style=flat-square&logo=php&logoColor=D4B87A&labelColor=141210) ![Live](https://img.shields.io/badge/Live-mj--cafe.vercel.app-B89758?style=flat-square&labelColor=141210&logoColor=FAF8F5) |
| **[`whatsapp-networking-hub`](https://github.com/iamhuitron/whatsapp-networking-hub)** | **Zero-Server WhatsApp Community Parser & Directory**<br>100% in-memory `FileReader` & `IndexedDB` parser that converts exported `.txt` community chats into a searchable professional directory. | ![Next.js](https://img.shields.io/badge/Next.js-IndexedDB-1D1A16?style=flat-square&logo=next.js&logoColor=D4B87A&labelColor=141210) ![Tests](https://img.shields.io/badge/Vitest-39_Passing-1B3B2B?style=flat-square&labelColor=141210&logoColor=D4B87A) |
| **[`rutina-optima`](https://github.com/iamhuitron/rutina-optima)** | **Biological Performance & Time-Allocation Command Center**<br>Sartorial Dark Editorial telemetry dashboard for circadian HGH optimization, V-Taper hypertrophy, and high-output academic/engineering scheduling. | ![Web](https://img.shields.io/badge/System-rutina--optima.vercel.app-B89758?style=flat-square&labelColor=141210&logoColor=FAF8F5) ![LifeOS](https://img.shields.io/badge/Telemetry-Life_OS-1D1A16?style=flat-square&labelColor=141210&logoColor=D4B87A) |

---

### `03` · Technical Stack & Tooling

<p align="left">
  <img src="https://img.shields.io/badge/Python_3.12-1D1A16?style=for-the-badge&logo=python&logoColor=D4B87A&labelColor=141210" alt="Python" />
  <img src="https://img.shields.io/badge/TypeScript_5-1D1A16?style=for-the-badge&logo=typescript&logoColor=D4B87A&labelColor=141210" alt="TypeScript" />
  <img src="https://img.shields.io/badge/DuckDB-1D1A16?style=for-the-badge&logo=duckdb&logoColor=D4B87A&labelColor=141210" alt="DuckDB" />
  <img src="https://img.shields.io/badge/Apache_Arrow-1D1A16?style=for-the-badge&logo=apachearrow&logoColor=D4B87A&labelColor=141210" alt="Apache Arrow" />
  <img src="https://img.shields.io/badge/PostgreSQL_&_SQLite-1D1A16?style=for-the-badge&logo=postgresql&logoColor=D4B87A&labelColor=141210" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Next.js_16-1D1A16?style=for-the-badge&logo=next.js&logoColor=D4B87A&labelColor=141210" alt="Next.js" />
  <img src="https://img.shields.io/badge/React_19_&_Expo-1D1A16?style=for-the-badge&logo=react&logoColor=D4B87A&labelColor=141210" alt="React" />
  <img src="https://img.shields.io/badge/PHP_8_PDO-1D1A16?style=for-the-badge&logo=php&logoColor=D4B87A&labelColor=141210" alt="PHP" />
  <img src="https://img.shields.io/badge/GitHub_Actions-1B3B2B?style=for-the-badge&logo=githubactions&logoColor=FAF8F5&labelColor=141210" alt="GitHub Actions" />
</p>

---

### `04` · Institutional & Executive Profile

- **Co-Founder & Technical Lead** at **[XAOL Software Studio](https://xaol-website.vercel.app)** — Delivering bespoke transactional systems, POS/inventory engines, and fiscal auditing platforms for Mexican enterprises.
- **Google Student Ambassador (2026 Cohort)** — Leading technical workshops on AI workflows, modern software engineering, and developer productivity at **UNAM**.
- **B.Sc. in Informatics** — **Universidad Nacional Autónoma de México (UNAM — FES Cuautitlán)**.
