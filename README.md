<div align="center">

# Bejjam Charan Sai Teja

**I build LLM applications with durable memory, Python services with tested
edges, and security tools that document their limits.**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bejjam-charan-sai-teja-/)
[![Email](https://img.shields.io/badge/Email-25d41a6633@sriindu.ac.in-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:25d41a6633@sriindu.ac.in)
[![GitHub](https://img.shields.io/badge/GitHub-charansaiteja--cloud-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/charansaiteja-cloud)

AI/ML undergraduate · Hyderabad, India · open to AI, backend, and security engineering roles

</div>

---

I'm an AI/ML undergraduate, and my favourite part of a project is the part after
the demo works: scoping memory so one customer can never recall another's data,
adding the coverage gate that fails the build, writing down what the tool does
*not* do.

That bias runs through most of what I build — local LLM applications on Ollama
and Qwen3, FastAPI backends with typed boundaries, and network tooling measured
by tests rather than screenshots.

## What I'm focused on

- **LLM engineering** — local inference, fact extraction, per-customer memory
  isolation, and evaluation harnesses that check extraction quality instead of
  vibes.
- **Backend engineering** — FastAPI, SQLAlchemy, Pydantic, SQLite/PostgreSQL,
  typed Python, and containerised deployments.
- **Security engineering** — packet analysis, anomaly detection, static analysis
  with Bandit and Semgrep, and secure-code review.

## Selected work

### [Support AI](https://github.com/charansaiteja-cloud/AI-AGENT) · a support agent that remembers the customer

`Python` `FastAPI` `React` `Ollama` `Qwen3` `Hindsight` `SQLite`

A full-stack support console where a customer explains their setup once and a new
conversation later still knows their device, preferences, and recurring issue.
Qwen3 extracts durable facts, Hindsight stores them in a bank scoped to that
customer, and SQLite stays the source of truth for application data.

The constraint that made it interesting was isolation: memory is keyed per
customer so recall cannot leak across accounts, and deleting a customer deletes
their memory bank. The UI exposes what was recalled, which model answered, and
how long it took.

```text
React console ──▶ FastAPI ──┬──▶ SQLite            app state
                            ├──▶ Ollama qwen3:8b   generation
                            └──▶ Hindsight         one bank per customer
```

**91 backend tests · 92.1% backend branch coverage · Ruff · CI for backend and frontend**

[Code](https://github.com/charansaiteja-cloud/AI-AGENT) ·
[How the memory works](https://github.com/charansaiteja-cloud/AI-AGENT/blob/main/article.md)

### [Secure Code Review](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview) · static analysis you can audit

`Python` `FastAPI` `Bandit` `Semgrep` `SQLite`

A reference service that runs Bandit and Semgrep, normalises both tools into one
finding schema, and then demonstrates the fixes it recommends: parameterised
SQL, defensive middleware, input limits. CI runs the suite and publishes a
CycloneDX SBOM alongside the test results.

**65 tests · Bandit and Semgrep integrated · SBOM in CI**

[Code](https://github.com/charansaiteja-cloud/CodeAlpha_SecureCodeReview)

### Smaller builds

- **[Basic Network Sniffer](https://github.com/charansaiteja-cloud/CodeAlpha_BasicNetworkSniffer)** —
  metadata-first Scapy sniffer with protocol decoding, BPF filters, CSV export,
  and a bounded ICMP preview. **16 tests.**
- **[Phishing Awareness Training](https://github.com/charansaiteja-cloud/CodeAlpha_PhishingAwarenessTraining)** —
  Streamlit training module with annotated examples, a scored quiz, and a
  completion flow. **16 tests, CI.**
- **[SentinelNet](https://github.com/charansaiteja-cloud/SentinelNet)** — a small
  NIDS *simulation* I built to understand the capture → threshold → alert loop.
  Deliberately a simulation: no live capture, flow reassembly, or blocking.
- **[CodeAlpha bundle](https://github.com/charansaiteja-cloud/codealpha_tasks)** —
  the three internship tasks in one reviewable monorepo.

## How I work

- **Measure the claim.** Test counts and coverage come from runs, not memory.
- **Type the edges.** Pydantic at the boundary, explicit schemas between layers.
- **Write the limits down.** A README that hides what a tool cannot do is a bug.
- **Keep it runnable.** Docker Compose or one command; no undocumented setup.

## Toolbox

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

Coursework: machine learning, data structures, database management systems,
operating systems, computer networks, and software engineering.

## Certifications

- **Microsoft** — Unlocking AI for Everyone
- **Tata / Forage** — GenAI Powered Data Analytics Job Simulation
- **Tata / Forage** — Cybersecurity Analyst Job Simulation
- **Infosys Springboard** — Introduction to Cyber Security
- **Infosys Springboard** — Prompt Engineering

## Connect

- **Email:** [25d41a6633@sriindu.ac.in](mailto:25d41a6633@sriindu.ac.in) — fastest way to reach me
- **LinkedIn:** [Bejjam Charan Sai Teja](https://www.linkedin.com/in/bejjam-charan-sai-teja-/)
- **GitHub:** [@charansaiteja-cloud](https://github.com/charansaiteja-cloud)

I'm open to AI engineering, LLM application, backend, and security engineering
opportunities where careful implementation and measurable quality matter.

<sub>Metrics above are from the repositories' test runs, October 2026.</sub>
