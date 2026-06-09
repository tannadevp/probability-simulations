# Probability, Simulated

A growing collection of classical probability problems — built, broken, and fixed in Jupyter Notebook.
The idea is simple: instead of just accepting a mathematical result, simulate it. Run it 100,000 times and watch the numbers confirm (or occasionally embarrass) the theory.

---

## Simulations

### 01) Monty Hall Problem
Switch or stay? The simulation runs 100,000 games and tracks win rates for both strategies, alongside a convergence plot showing the Law of Large Numbers in action.  
Result: Switch wins ~66.7%. Stay wins ~33.3%.

### 02) Random Walks
A walker at 0 moves ±1 each step with equal probability. Where do they end up after n steps? Includes trajectory plots, a histogram of final positions (converging to a normal distribution), and a scaling plot confirming the √n RMS displacement law.  
Result: Expected displacement = 0. Typical displacement = √n.

### 03) Gambler's Ruin
A gambler with ₹k plays fair-or-biased ₹1 rounds against a wealthier opponent until one goes broke. Even a perfectly fair game gives only a k/N chance of survival. Includes ruin probability curves (simulated vs. theoretical), game duration histograms, and wealth trajectory plots.  
Result: P(survival) = k/N for fair game. Decays exponentially when p < 0.5.

---

## Coming Soon

- **The Kelly Criterion**
- **Central Limit Theorem** 
- **Markov Chains** 

---

## Stack

```
Python 3
Jupyter Notebook
random · matplotlib · math 
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
