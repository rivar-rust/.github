<p align="center">
   <img src="assets/rivar.png" alt="RIVAR banner" />
</p>

Rivar is a Rust-based library for quantitative and computational risk management. It provides implementations of portfolio risk measures and simulation methods designed for correctness, reproducibility, and performance.

The project focuses on transforming financial risk models into structured, maintainable, and computationally efficient systems. Rivar is intended for research environments, academic exploration, and production-oriented risk analytics.

Visit - [RiVaR](https://rivar-rho.vercel.app/)


---

## Purpose

Financial risk modeling is often split between two domains:

* Mathematical modeling of risk measures
* Practical implementation in scalable systems

Rivar aims to unify both within a single Rust-native framework.

The library implements formally defined risk measures such as Value at Risk (VaR) and Conditional Value at Risk (CVaR), and provides Monte Carlo simulation infrastructure for estimating complex portfolio loss distributions.

---

## Core Capabilities

### Risk Measures

* Parametric Value at Risk
* Historical Value at Risk
* Monte Carlo Value at Risk
* Conditional Value at Risk (Expected Shortfall)

### Simulation Engine

* Monte Carlo scenario generation
* Configurable simulation size
* Parallel execution
* Deterministic numerical behavior

### Portfolio Modeling

* Weighted portfolio structures
* Loss distribution construction
* Risk factor abstraction
* Modular model definitions

### Statistical Computation

* Empirical quantile estimation
* Efficient selection algorithms
* Configurable confidence levels
* Reproducible simulation outputs

---

## Installation

```bash
cargo install rivar
```

---

## Example Usage

```bash
rivar init --template risk-model
rivar calculate --var --confidence 0.95
rivar backtest --strategy my-strategy
rivar analyze --portfolio holdings.json
```

---

## Design Principles

Rivar is developed with the following principles:

1. Mathematical clarity
   Risk measures are implemented according to their formal definitions.

2. Separation of concerns
   Quantitative models and computational execution are structured independently.

3. Deterministic execution
   No garbage collection pauses or hidden runtime behavior.

4. Memory safety
   Rust’s ownership model prevents data races and memory leaks.

5. Scalability
   Monte Carlo simulations and portfolio computations are designed to scale with increasing data size.

---

## Architecture Overview

Rivar follows a layered structure:

* Data Layer: Portfolio and market data representation
* Model Layer: Formal risk measure definitions
* Simulation Layer: Scenario generation and numerical execution
* Interface Layer: CLI and integration endpoints

This separation ensures that mathematical definitions remain independent from performance optimizations.

---

## Intended Use Cases

Rivar may be used for:

* Academic research in risk modeling
* Portfolio risk estimation
* Backtesting and stress analysis
* Experimental computational finance systems
* Integration into larger financial software stacks

---

## Documentation

Documentation and usage guides are available at:

[https://docs.rivar.dev](https://docs.rivar.dev)

---

## Status

Rivar is under active development. Contributions, reviews, and discussions are welcome.


