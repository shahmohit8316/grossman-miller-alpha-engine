# 📈 Grossman-Miller Alpha Engine

> “In a noisy world, the insider isn’t lucky. He’s prepared.”

A cutting-edge simulator of the legendary **Grossman-Miller (1988)** market microstructure model — built to extract alpha from asymmetric information, belief distortion, and rational expectations.

This isn’t just replication. This engine is designed to evolve into a real-time **insider strategy optimizer** and **rational market maker simulator** — capable of live alpha extraction and backtested profit curves.

---

## 💡 What is This?

A modular, research-grade system that simulates:

- 📊 **Signal-noise model of asset pricing**
- 🧠 **Optimal insider strategies (β*) under rational expectations**
- 💸 **Market maker pricing rules and belief systems**
- 🔁 **Market clearing with private + public information**
- 📈 **PnL tracking of informed vs uninformed agents**

---

## 🏗️ Repository Architecture

| Folder | Purpose |
|--------|---------|
| `core_model/` | All OCaml modules for insider demand, market clearing, and equilibrium pricing |
| `alpha_extraction/` | Tools for computing, plotting, and optimizing α from private signals |
| `math_engine/` | Variance-covariance systems, rational expectation derivations, integration tools |
| `simulations/` | Scenarios for different noise intensities, information endowments, and insider edges |
| `benchmarks/` | Performance logs of β* search, equilibrium convergence, and insider win rate |
| `experiments/` | Model testing: robustness to signal strength, multi-agent insider environments |
| `docs/` | Full derivation of GM model, PDF notebooks, β* proofs beyond MIT PhD level |
| `config/` | Simulation parameters: signal-noise ratio, liquidity depth, number of market makers |
| `visuals/` | Graphs: belief update over time, insider advantage, price vs signal divergence |
| `README.md` | What you’re reading now. A war manifesto. |

---

## 🚀 Features

✅ Full pipeline from insider signal to equilibrium pricing  
✅ OCaml-native numeric implementation (type-safe, high-speed)  
✅ Supports symbolic β*, numerical optimization, brute force grid  
✅ Auto-graphing of insider alpha over signal strength  
✅ Multi-agent extension planned: insider + market maker + noise trader

---

## 🔬 Alpha Extraction Modes

| Mode | Description |
|------|-------------|
| `beta_grid.ml` | Brute-force search over β to maximize E[Profit] |
| `belief_update.ml` | Tracks how prices embed insider signal |
| `variance.ml` | Symbolic + numerical decomposition of price variance |
| `alpha_curve.ml` | α (PnL) vs β plot for visualization of optimal strategy |
| `base_case.ml` | Classic Grossman-Miller setup (1988, Econometrica) |

---

## 📎 Usage

```bash
# Compile
dune build

# Run base model simulation
dune exec simulations/base_case.exe

# Graph alpha curve
dune exec alpha_extraction/alpha_curve.exe
