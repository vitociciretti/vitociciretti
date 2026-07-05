# Vito Ciciretti

**I build systems that simulate worlds and agents — then stress-test what they claim.** Multi-agent social simulations, LLM-driven worlds, and the graph-memory and evaluation infrastructure underneath them — with research roots in quantitative finance, where I spend as much effort trying to break a result as I do building it.

PhD in Finance *(candidate)*, University of Essex · MSc Artificial Intelligence / Computer Science *(candidate)* · MSc Quantitative Finance, Bocconi University

[LinkedIn](https://www.linkedin.com/in/vitociciretti/) · [Google Scholar](https://scholar.google.com/citations?user=T9wbYUcAAAAJ&hl=en) · vciciretti8@gmail.com

---

## What I actually do

One question runs through all of it: how does complex, collective behavior **emerge** — from markets, from crowds, from populations of agents — and how much of an apparent signal actually survives honest scrutiny.

On the research side, that means treating markets as **networks** rather than an unordered basket of correlations — minimum spanning trees, threshold graphs, spectral and random-matrix methods — and using that topology to detect regime change and build more robust portfolios. On the building side, it becomes **agentic simulation**: spinning up populations of LLM-driven agents to rehearse how a scenario plays out, together with the memory, retrieval, and evaluation infrastructure that makes those simulations trustworthy rather than merely plausible.

Underneath both is methodological honesty. A lot of published "signal" in this space evaporates under a genuinely out-of-sample test, so I spend real effort re-running pipelines with blocked splits, leakage checks, and walk-forward validation — and reporting it plainly when the result is a clean negative rather than an inflated positive.

## Research

- **[Network Risk Parity: graph theory-based portfolio construction](https://link.springer.com/article/10.1057/s41260-023-00347-8)** — *Journal of Asset Management*, 2024 (with A. Pallotta)
- **[Adaptive Market Anomaly Detection (AMAD): enhancing minimum spanning tree stability](https://www.sciencedirect.com/science/article/pii/S1544612325012553)** — *Finance Research Letters*, 2025 (with A. Pallotta)
- **[An early-warning risk signals framework to capture systematic risk in financial markets](https://www.tandfonline.com/doi/abs/10.1080/14697688.2025.2482637)** — *Quantitative Finance*, 2025
- **[Market regime detection via realized covariances](https://arxiv.org/abs/2104.03667)** — *Economic Modelling*, 2022 (with A. Bucci)
- **Building optimal regime-switching portfolios** — *The North American Journal of Economics and Finance*, 2023 (with A. Bucci)

[Full list — 12 publications — on Google Scholar →](https://scholar.google.com/citations?user=T9wbYUcAAAAJ&hl=en)

## Selected open-source work

| Project | What it is |
|---|---|
| **[synfin](https://github.com/vitociciretti/synfin)** | Synthetic financial time-series generator — regime-switching GARCH, factor models, calibrated presets |
| **[causality-toolkit](https://github.com/vitociciretti/causality-toolkit)** | Lead-lag / causality analysis for time series (CCF, Granger, Transfer Entropy, DTW, Wavelet Coherence, CCM) |
| **[delphi](https://github.com/vitociciretti/delphi)** | Multi-agent world-simulation engine, extended with a financial-market scenario layer (built on MiroFish + OASIS) |
| **[demiurge](https://github.com/vitociciretti/demiurge)** | A god-game about simulated reality — a colony of inhabitants tries to notice it's in a simulation |
| **[Godot: The Existentialist Game](https://github.com/vitociciretti/godot-existentialist-game)** | A Beckett two-hander built in the Godot engine — you play one tramp, an LLM plays the other |

## Simulated minds — and the stack that runs them

This is where the agentic-simulation work lives, held to the same standard as the research.

The three projects above aren't just tech demos of each other's engines — they're
places to actually think about simulated minds. 

**Godot: The Existentialist Game**
puts an LLM in Beckett's other chair and just talks, forever, until you stop
waiting. 

**Delphi** spins up a parallel digital world from a news article, a
policy draft, or a market signal, and rehearses how it plays out. 

**Demiurge** is
a god-game about simulated reality, built around one invariant: private noise
should never wake anyone up — only *shared* anomalies should.

Under those sits a **local-first AI infrastructure stack** — private for now, early, but built to the same bar as
everything else here: a hybrid dense+BM25+RRF retrieval engine with a full
retrieval-trace panel, a GraphRAG memory layer on the same substrate with
fact-level citations, a knowledge-graph quality gate with reversible repairs, a
durable DAG orchestrator with exactly-once effects and resume-from-failure, an
eval/monitoring system that grades production traces with the *same* scorer as
CI, and a cryptographic agent-identity and payments rail with its own adversarial
test suite. It shows up in the graph below as its own cluster.

I also got tired of losing track of which of my ~25 projects were actually
running, stale, or safely forgotten — so I built **Helm**, a manifest-driven
control panel: one card per project with live git status and a start/stop
button for the handful that are actual services. Private, still rough, but
it's already the first thing I open in the morning.

## Everything else I've built

The projects above are public and linked; the rest is private research and
production work, named below so the shape of it is visible.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/network-graph-dark.svg">
  <img alt="Project network graph — published research, data infrastructure, regime and network research, strategy engines, risk tooling, creative simulation, personal tooling, and an AI infrastructure stack" src="assets/network-graph-light.svg">
</picture>
