# Probability, Simulated

A growing collection of classical probability problems — built, broken, and fixed in Jupyter Notebook.
The idea is simple: instead of just accepting a mathematical result, simulate it. Run it 100,000 times and watch the numbers confirm (or occasionally embarrass) the theory.

---

## Simulations

### 01) Monty Hall Problem
The one where switching doors doubles your chances, and almost nobody believes it until they see the numbers.
The simulation runs 100,000 games of the Monty Hall problem and tracks the win rate of two strategies — Stay and Switch. It also includes a convergence plot showing how the win rates stabilise as more games are played, which is the Law of Large Numbers in action.

**Result:** Switch wins ~66.7% of the time. Stay wins ~33.3%.

### 02) Random Walks
A walker starts at 0 and moves left or right with equal probability at every step. The question is: where do they end up after n steps?
The intuitive answer is "probably near zero." The actual answer is that the typical distance from zero grows as √n — which is not obvious and takes a simulation to really appreciate.
Includes sample trajectory plots, a histogram of final positions (which converges to a normal distribution, a preview of the CLT), and an RMS displacement vs. steps scaling plot confirming the √n law.

**Result:** Expected displacement = 0. Typical displacement = √n.

---

## Coming Soon

- **Gambler's Ruin**
- **The Kelly Criterion**
- **Central Limit Theorem** 
- **Markov Chains** 

---

## Stack

```
Python 3
Jupyter Notebook
random · matplotlib
```

No heavy dependencies. Everything is built with the standard library and matplotlib, deliberately, so the logic stays visible.

---

## Running It

Clone the repo and open any notebook in Jupyter:

```bash
git clone https://github.com/yourusername/probability-simulations
cd probability-simulations
jupyter notebook
```

Each notebook is self-contained. Run all cells top to bottom.
The one configurable value in each notebook is `n` (number of simulations) — you can change it to see how results shift with fewer or more runs.

---
## Contributions & Suggestions

If you have ideas for new simulations, spot something wrong in the existing ones, or just want to suggest a better way to explain something, feel free to open an issue or reach out directly. Always open to it!

*Built by Tanu Singh — BTech in Computer Science and Engineering, IIITDMJ*
