# Bejjam Charan Sai Teja

**AI/ML engineer building practical LLM applications, secure backends, and
well-tested Python tools.**

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)](https://react.dev/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)

I am an Artificial Intelligence and Machine Learning undergraduate in Telangana,
India. I like turning model capabilities into software that is understandable,
tested, and safe to operate: local LLM applications, retrieval and memory
systems, Python services, and security tooling.

## What I'm focused on

- **LLM engineering** — Ollama and Qwen3, durable conversational memory,
  prompt design, and evaluation harnesses that measure extraction quality.
- **Backend engineering** — FastAPI, SQLAlchemy, SQLite/PostgreSQL, typed
  Python, and containerised deployments.
- **Security engineering** — network anomaly detection, packet analysis,
  secure-code review, and static analysis with Bandit and Semgrep.
- **Engineering quality** — tests with measured coverage, Ruff, Mypy, Bandit,
  and GitHub Actions on every push.

## Featured projects

| Project | Description | Verification |
| --- | --- | --- |
| [**AI Customer Support Agent**](https://github.com/charansaiteja-cloud/AI-AGENT) | Full-stack support agent with Qwen3 via Ollama, per-customer long-term memory in Hindsight, optional API-key auth, attachments, and a React UI. | 121 backend + 17 frontend tests · 85.2% backend coverage · Ruff, Mypy, CI |
| [**SentinelNet**](https://github.com/charansaiteja-cloud/SentinelNet) | ML-assisted network anomaly detector. Learns a baseline with Isolation Forest, scores live or replayed traffic, applies risky-port rules, and emits JSONL alerts with cooldown. | 48 tests · 91% branch coverage · Ruff, Mypy, Bandit · Docker image |
| [**Secure Code Review**](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview) | FastAPI reference service that orchestrates Bandit and Semgrep, normalises findings, and demonstrates defensive middleware and parameterised SQL. | 74 tests · 82.8% branch coverage · Ruff and Bandit clean · Python 3.11/3.12 CI |
| [**Basic Network Sniffer**](https://github.com/charansaiteja-cloud/CodeAlpha_BasicNetworkSniffer) | Metadata-first Scapy sniffer with protocol decoding, CSV export, BPF filtering, and a bounded ICMP preview. | 18 tests · Ruff clean · Python 3.9–3.12 CI |
| [**Phishing Awareness Training**](https://github.com/charansaiteja-cloud/CodeAlpha_PhishingAwarenessTraining) | Streamlit training module with annotated phishing examples, an interactive quiz, scoring, and a completion flow. | 16 tests · 98.9% branch coverage · Ruff clean |
| [**CodeAlpha Project Bundle**](https://github.com/charansaiteja-cloud/codealpha_tasks) | The three CodeAlpha tasks in one reviewable monorepo, with a root CI workflow that runs all 108 tests. | 108 tests across three suites · root CI |

### SentinelNet at a glance

```text
live interface ─┐
                ├─▶ Scapy capture ─▶ 11-feature packet vector ─▶ baseline
PCAP replay ────┘                                              │
                                                               ▼
                                      Isolation Forest ─▶ explicit threshold
                                                               │
                            every later packet ─▶ score / rules ─▶ JSONL alert
```

It is an anomaly detector, not a full IDS: it does not reassemble flows, inspect
payloads, or block traffic. The README documents those limits alongside the
risky-port heuristic and baseline assumptions.

## Technical toolkit

| Area | Tools |
| --- | --- |
| Languages | Python, Java, C, SQL |
| AI / LLMs | Ollama, Qwen3, Hindsight, prompt engineering, local inference |
| Backend | FastAPI, SQLAlchemy, Pydantic, REST APIs, SQLite |
| Frontend | React, Vite, JavaScript, CSS |
| Quality | Pytest, pytest-cov, Ruff, Mypy, Bandit, pip-audit |
| Delivery | Docker, Docker Compose, GitHub Actions, Git |
| Security | Linux, Wireshark, Nmap, Burp Suite, Semgrep, OSINT |

## Education

**B.Tech. in Artificial Intelligence and Machine Learning**<br>
Sri Indu College of Engineering & Technology, Hyderabad, Telangana

Coursework and interests include machine learning, data structures, database
management systems, operating systems, computer networks, and software
engineering.

## Certifications and professional development

- Microsoft — Unlocking AI for Everyone
- Tata / Forage — GenAI Powered Data Analytics Job Simulation
- Tata / Forage — Cybersecurity Analyst Job Simulation
- Infosys Springboard — Introduction to Cyber Security
- Infosys Springboard — Prompt Engineering

## Connect

- **GitHub:** [@charansaiteja-cloud](https://github.com/charansaiteja-cloud)
- **LinkedIn:** Bejjam Charan Sai Teja
- **Email:** [25d41a6633@sriindu.ac.in](mailto:25d41a6633@sriindu.ac.in)

I am open to AI engineering, LLM application, backend, and security engineering
opportunities where careful implementation and measurable quality matter.
