<div align="center">

# Bejjam Charan Sai Teja

**AI/ML Engineer building memory-aware LLM applications, tested Python backends, and security tools with documented limits.**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bejjam-charan-sai-teja-)
[![CIKSHA](https://img.shields.io/badge/CIKSHA-Profile-111827?style=flat-square&logo=link&logoColor=white)](https://ciksha.com/@charansaiteja)
[![GitHub](https://img.shields.io/badge/GitHub-charansaiteja--cloud-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/charansaiteja-cloud)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:25d41a6633@sriindu.ac.in)

Hyderabad, India · B.Tech. AI/ML Undergraduate · **Open to AI Engineering, LLM Application, Backend, and Security Engineering roles**

</div>

> **Review in 60 seconds:** [Support AI demo](https://raw.githubusercontent.com/charansaiteja-cloud/AI-AGENT/main/docs/demo/demo.gif) → [AI-AGENT repo](https://github.com/charansaiteja-cloud/AI-AGENT) (memory isolation + 121 backend tests / 84.9% branch coverage, 83% gate) → [Secure Code Review](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview) (Bandit + Semgrep + SBOM) → [Contact](#connect). *Metrics sourced from linked repository READMEs/docs/CI.*

## At a glance

- I build **memory-aware LLM systems** (local inference, fact extraction, per-customer isolation), **typed FastAPI/Python services**, and **practical security tooling**.
- I focus on what matters after the demo: **data isolation**, **measured tests/coverage**, **reproducible Docker setup**, and **explicit limitations**.
- **Fastest contact:** [25d41a6633@sriindu.ac.in](mailto:25d41a6633@sriindu.ac.in) · [LinkedIn](https://www.linkedin.com/in/bejjam-charan-sai-teja-) · [CIKSHA](https://ciksha.com/@charansaiteja)

## Selected work

### [Support AI](https://github.com/charansaiteja-cloud/AI-AGENT) — memory-aware customer support agent
[![CI](https://github.com/charansaiteja-cloud/AI-AGENT/actions/workflows/ci.yml/badge.svg)](https://github.com/charansaiteja-cloud/AI-AGENT/actions/workflows/ci.yml) `Python` `FastAPI` `React` `Vite` `Ollama` `Qwen3` `Hindsight` `SQLite` `Docker Compose`

Full-stack support console: a customer can explain context once and return later with relevant recall. Qwen3 extracts durable facts; Hindsight stores them in a **dedicated bank per customer**; SQLite holds application state.

<p align="center">
  <a href="https://github.com/charansaiteja-cloud/AI-AGENT" title="Open Support AI repository">
    <img src="https://raw.githubusercontent.com/charansaiteja-cloud/AI-AGENT/main/docs/demo/demo.gif" alt="Support AI demo: create customer, extract facts, recall context, verify memory isolation" width="880" />
  </a>
</p>

- **Key constraint (engineering):** per-customer memory isolation — no cross-customer recall; deleting a customer deletes that memory bank.
- **Implementation highlights:** typed API boundaries, overlapped/efficient request flow, memory/latency/model visibility, attachment handling (text/Markdown/CSV/JSON/PDF, as implemented).
- **Quality (verified from repository README):** 121 backend tests, **84.9%** backend branch coverage (**83% gate**), 17 frontend tests, Ruff, backend/frontend CI.
- **Evaluate quickly:** [Code](https://github.com/charansaiteja-cloud/AI-AGENT) · [Architecture](https://github.com/charansaiteja-cloud/AI-AGENT/blob/main/article.md) · [Demo video](https://github.com/charansaiteja-cloud/AI-AGENT/blob/main/docs/demo/demo.mp4) · Run: `git clone https://github.com/charansaiteja-cloud/AI-AGENT && cd AI-AGENT && docker compose up --build -d` *(local Ollama/model setup required; see repo README)*

```text
React console ──▶ FastAPI ──┬── SQLite            app state
                            ├── Ollama / Qwen3    generation & extraction
                            └── Hindsight         one bank per customer
```

### [Secure Code Review](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview) — auditable static analysis lab/service
[![CI](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview/actions/workflows/ci.yml/badge.svg)](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview/actions/workflows/ci.yml) `Python` `FastAPI` `SQLite` `Bandit` `Semgrep` `CycloneDX` `Docker Compose`

Normalizes Bandit/Semgrep findings into an auditable workflow with secure patterns, scan containment, and remediation-oriented reporting.

- **Security focus:** parameterized SQL patterns, defensive middleware, input validation/limits, fail-closed API-key behavior where misconfigured, contained scan targets.
- **Quality (verified from repository README/docs):** 74 tests, **82.8%** branch coverage *(recorded 2026-10-27 in repo docs)*, Bandit + Semgrep integrated, CycloneDX SBOM in CI.
- **Links:** [Code](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview) · [Security policy](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview/blob/main/docs/security-policy.md)

### [SentinelNet](https://github.com/charansaiteja-cloud/SentinelNet) — ML-assisted network anomaly detection
[![CI](https://github.com/charansaiteja-cloud/SentinelNet/actions/workflows/ci.yml/badge.svg)](https://github.com/charansaiteja-cloud/SentinelNet/actions/workflows/ci.yml) `Python` `Scapy` `scikit-learn (Isolation Forest)` `JSONL alerts` `Docker Compose`

Baseline-driven anomaly detection with live capture and PCAP replay (no root required for replay), structured alerts, and privacy-conscious handling (no payload storage).

- **Quality (verified from repository README):** 48 tests, **~91%** coverage; Ruff, Mypy, Bandit, pip-audit documented.
- **Limitations (documented):** anomaly detector, **not** a full IDS/IPS — no flow reassembly, payload inspection, or traffic blocking.
- **Link:** [Code](https://github.com/charansaiteja-cloud/SentinelNet)

## Additional projects

| Project | What it demonstrates | Stack |
| --- | --- | --- |
| [Basic Network Sniffer](https://github.com/charansaiteja-cloud/CodeAlpha_BasicNetworkSniffer) | Metadata-first packet decoding (IPv4/IPv6/ARP/TCP/UDP/ICMP/DNS), BPF filtering, bounded previews, streaming capture (`store=False`) | Python · Scapy · pytest |
| [Phishing Awareness Training](https://github.com/charansaiteja-cloud/CodeAlpha_PhishingAwarenessTraining) | Annotated examples, scored quiz, completion/certificate flow with tests and CI | Python · Streamlit · pytest |
| [CodeAlpha Tasks](https://github.com/charansaiteja-cloud/codealpha_tasks) | Monorepo bundling internship/security tasks with per-task tests/workflows | Python · Security tooling |

## How I work

- **Measure claims:** tests, coverage, and CI — not screenshots.
- **Type boundaries:** validate inputs; keep contracts explicit (Pydantic/schemas).
- **Isolate data:** separate tenant/customer context; make deletion explicit.
- **Document limits:** state what a system does *and* does not do.
- **Ship runnable code:** reproducible setup (Docker/Compose) and automated checks.

## Toolbox

| Area | Technologies |
| --- | --- |
| Languages | Python, Java, C, SQL |
| AI / LLM | Ollama, Qwen3, Hindsight, prompt/fact extraction, local inference, evaluation-minded workflows |
| Backend | FastAPI, SQLAlchemy, Pydantic, REST APIs, typed Python |
| Frontend | React, Vite, JavaScript, CSS |
| Data | SQLite, PostgreSQL-oriented design |
| Quality & Security | pytest, pytest-cov, Ruff, Mypy, Bandit, Semgrep, pip-audit |
| Delivery & Tools | Docker, Docker Compose, GitHub Actions, Git, Linux, Scapy, Wireshark, Nmap, Burp Suite, OSINT |

## Education & certifications

**B.Tech. in Artificial Intelligence and Machine Learning** — Sri Indu College of Engineering & Technology, Hyderabad, Telangana, India  
*Relevant coursework:* Machine Learning, Data Structures, DBMS, Operating Systems, Computer Networks, Software Engineering.

**Certifications:** Microsoft — *Unlocking AI for Everyone*; Tata/Forage — *GenAI Powered Data Analytics Job Simulation*, *Cybersecurity Analyst Job Simulation*; Infosys Springboard — *Introduction to Cyber Security*, *Prompt Engineering*.

## Connect

- **Email (fastest):** [25d41a6633@sriindu.ac.in](mailto:25d41a6633@sriindu.ac.in)
- **LinkedIn:** [Bejjam Charan Sai Teja](https://www.linkedin.com/in/bejjam-charan-sai-teja-)
- **CIKSHA:** [@charansaiteja](https://ciksha.com/@charansaiteja)
- **GitHub:** [@charansaiteja-cloud](https://github.com/charansaiteja-cloud)

<sub>Professional profile README. Project metrics are sourced from the linked repositories’ READMEs/docs/CI at the time referenced; verify current results in each repository.</sub>
