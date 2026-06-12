# thesis_playground

Publicly shareable code from my senior thesis on reinforcement learning for
financial time series.

I train RL agents on **synthetic** price data generated from stochastic
differential equations (starting with geometric Brownian motion), each
discretized with an Euler–Maruyama scheme. Working in a controlled,
model-driven setting lets me study how an agent's learned behavior depends on
the underlying data-generating process before moving to real market data.

## Notebooks

- `DQN_stochastic_gen_1.ipynb` — Generates GBM price paths via an Euler scheme,
  discretizes the market state into return quartiles, learns an action-value
  function with Q-learning, and evaluates the resulting policy by the
  distribution of final PnL across thousands of simulated paths versus a random
  baseline.

## Setup

```bash
pip install numpy matplotlib
```

---

*This is exploratory "playground" code — work in progress, not the final thesis.*
