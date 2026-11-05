# Supply Chain Implementation Manager for Shippers

![Python](https://img.shields.io/badge/python-3.10%2B-blue) ![SQLite](https://img.shields.io/badge/SQLite-stdlib-lightgrey) ![Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen) ![Tests](https://img.shields.io/badge/tests-unittest-success)

**A project-management tool for supply chain transformation at shippers (BCOs): a 32-week, six-phase methodology turned into software — schedule, RACI, diagnosis, control tower, action plan, KPIs and governance rituals in one place.**

> Built by **Marcelo Gurgel Carvalho** — 15+ years in commercial management for ports, shipping and logistics; Lean practitioner (Kaizen, Kaikaku, 3-Step Model, SQDC).

## The business problem

Supply chain improvement projects at mid-sized shippers usually live in slides and spreadsheets. Diagnosis, targets, actions and follow-up are disconnected, so the project loses rhythm after the kickoff and results are impossible to prove.

## What it does

| Module | Delivers |
|---|---|
| **Methodology** | 6 phases, 36 activities, owner/support, start and end weeks, deliverable and RACI for each |
| **Schedule** | Gantt and milestones calculated from each client's start date; portfolio view across clients |
| **Diagnosis** | Supply chain map, cost-to-serve (product, inventory and delivery cost per customer) and a 0–5 maturity radar |
| **Control Tower** | **OTIF measured per order** (all items, full quantity, by the promised date) for sales and inbound; 95% target with supplier alerts |
| **Action Plan** | What / owner / due date / status / linked KPI; **auto-suggests actions** from diagnosis gaps and control-tower alerts |
| **KPIs** | 7 project indicators with baseline, target and readings (logistics cost/revenue, cost per ton, OTIF, MAPE, inventory turns, coverage, procurement saving) + a catalog of 30 cross-functional KPIs with root-cause drivers |
| **Governance** | Three rituals — Steering Committee, Workstream review and S&OP — with agendas |
| **Data intake** | Spreadsheet templates and validated imports (rejects unknown SKUs/channels); Brazil heat map by state |

## Technical decisions

- **Python standard library only** (`http.server`, `sqlite3`) — runs on any laptop, no installation.
- **Business rules centralized** in one core module; REST API; single-page HTML interface.
- **Automated tests** with `unittest`.
- **Explicit metric definitions:** the OTIF rule is documented and enforced in code, avoiding the classic "on-time by carrier ETA" distortion.

---

## 🇧🇷 Resumo em português

Ferramenta para gerir **projetos de implementação de supply chain em embarcadores**: metodologia de 6 fases e 32 semanas, com cronograma, RACI, diagnóstico (mapa da cadeia, custo para servir e maturidade), Torre de Controle com **OTIF por pedido**, Plano de Ação que sugere ações a partir das lacunas, 7 indicadores do projeto e catálogo de 30 KPIs, além dos rituais de Comitê, Frentes e S&OP. Feita apenas com Python e SQLite da biblioteca padrão, com testes automatizados.

*Source code is private. Demo available on request.* · [LinkedIn](https://www.linkedin.com/in/marcelo-gurgel-b-carvalho-04770886)
