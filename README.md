# Buffon's Needle — Interactive Monte Carlo Simulation

An interactive, browser-based exploration of **Buffon's Needle**, a classic problem in geometric probability that estimates π by randomly dropping needles onto parallel lines.

This demonstration connects **Monte Carlo simulation, statistical convergence, and geometric reasoning** through hands-on experimentation.

## Live Demo



## Features

- **Needle-Drop Simulation:** Simulate 1–1,000 random needle drops per batch, or watch an animated single drop.
- **Real-Time Statistics:** Track total drops, line crossings, crossing proportion, and the current estimate of π.
- **Monte Carlo Convergence:** Visualize how the estimated value of π evolves as the number of drops increases.
- **Adjustable Parameters:** Modify needle length, distance between parallel lines, and animation speed.
- **Interactive Geometry Explorer:** Drag the needle's midpoint or endpoints to investigate the geometric conditions for crossing a line.
- **Long-Needle Challenge:** Explore why the standard probability formula fails when the needle length exceeds the spacing between lines, and discover the corrected formula.
- **Guided Introduction:** Learn about the history of π, Buffon's Needle problem, and the Law of Large Numbers.


## Mathematical Background

Let:

- $L$ = needle length
- $d$ = distance between parallel lines
- $N$ = total number of needle drops
- $C$ = number of crossings

For a needle of length $L \leq d$, the theoretical probability of crossing a line is:

$$
P(\text{cross}) = \frac{2L}{\pi d}
$$

Using the observed crossing proportion $C/N$, we obtain the Monte Carlo estimator:

$$
\hat{\pi} = \frac{2LN}{dC}, \qquad C>0
$$

As the number of independent drops increases, the observed crossing proportion approaches its theoretical probability, illustrating the **Law of Large Numbers**.

### The Long-Needle Case

When $L>d$, the standard formula no longer applies.

Defining $r=L/d>1$, the corrected crossing probability becomes:

$$
P(\text{cross})=\frac{2}{\pi}\left[r-\sqrt{r^2-1}+\operatorname{arcsec}(r)\right]
$$

The interactive challenge allows users to explore this distinction and understand why mathematical assumptions matter.


## Acknowledgments

Developed as an interactive mathematics demonstration with guidance from **Professor Bo Yang** at the **University of Wisconsin–Madison**.

## References & Further Reading

- Weisstein, Eric W. [“Buffon's Needle Problem.”](https://mathworld.wolfram.com/BuffonsNeedleProblem.html) *MathWorld—A Wolfram Web Resource.*
- Ventrella, Jeffrey. [“Buffon's Needle.”](https://www.ventrella.com/Buffon/) Interactive visualization, *Ventrella.com*.
