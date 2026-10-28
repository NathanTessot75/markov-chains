# Markov Explorer

**Build, simulate and play with Markov chains in real time.**

Markov Explorer is an interactive tool for exploring discrete-time Markov chains through two modes: a free **sandbox** to build and simulate any transition graph, and a **levels** mode with progressive puzzles to solve. It accompanies a co-authored mathematical paper on Markov chains (PSL University, January 2026) covering stationary distributions, the Perron–Frobenius theorem, convergence and hidden Markov models.

---

## Modes

### Sandbox
Build your own Markov chain:
- Add and move states on an SVG canvas
- Set the transition probabilities between each pair of states
- Run the simulation step by step or continuously
- See the stationary distribution computed in real time

### Levels
Solve puzzles based on Markov chain theory:

| # | Title | Concept | Difficulty |
|---|-------|---------|------------|
| 1 | World Tour | Deterministic cycle | Easy |
| 2 | The Well | Absorbing state | Medium |
| 3 | The Hierarchy | Controlled stationary distribution | Hard |
| 4 | The Tourist | Hitting time | Medium |

Each level has a precise goal (for example, "make state C absorbing") and checks automatically whether your chain satisfies it.

---

## Under the hood

- **Interactive SVG canvas**: draggable nodes, zoom and pan
- **Stationary distribution**: numerical solution of πP = π
- **Animated simulation**: the path followed state by state
- **Automatic validation** of each level's goal
- **No build step**: a single HTML file (React and Tailwind loaded from a CDN)

The interface is in French.

---

## Usage

No installation needed: open `index.html` in a browser.

```bash
git clone https://github.com/NathanTessot75/markov-chains.git
cd markov-chains
open index.html
```

---

## Concepts covered

- Discrete-time Markov chains
- Stochastic transition matrices (rows summing to 1)
- Stationary distribution (left eigenvector for λ = 1)
- Absorbing states, cycles, ergodicity

---

## License

© 2026 Nathan Tessot. All rights reserved.
