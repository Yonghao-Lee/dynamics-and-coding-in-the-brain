# Dynamics and Coding in the Brain: Weekly Notes

Textbook-style study notes for **Dynamics and Coding in the Brain** (HUJI 769001, Fall 2026/7). Each week's PDF can be read on its own:

- Every term is defined in plain words before it is used.
- Every derivation is done step by step.
- Every new idea comes with a worked numerical example.
- Common mistakes, including errors in the original handouts, are flagged in boxes.

No neuroscience background is assumed. You need undergraduate linear algebra and calculus.

## Contents

| Week | Notes | What you will learn |
|---|---|---|
| 01 | [**week01.pdf**](week01.pdf) | **Lecture:** neurons, spikes, chemical synapses, Dale's principle, the rate model, length and time scales of the brain, the fruit-fly compass, the questions of dynamics and coding. **Bonus hour:** differential equations from scratch: solving ṅ = an, fixed points, external input and convolution, the time constant τ. **TA session:** coupled linear systems ẋ = Mx solved through eigenvectors, left vs. right eigenvectors, stability, the trace/determinant test. Ends with practice problems with full solutions and a one-page cheat sheet. |
| 02 | [**week02.pdf**](week02.pdf) | **The autapse** (a neuron with a synapse onto itself) with a linear activation function: fixed points, amplification by feedback, stability by perturbation analysis, the full solution r(t), the vector-field picture, and the link to Week 1's eigenvalues. **Non-linear autapse** with a logistic activation function: graphical fixed points, local vs. global stability, linearisation (λ = Jg′), saddle-node bifurcations and the bifurcation diagram, attractors, bistability and storing a bit of memory with a brief input pulse, the half-stable case λ = 1. Practice problems with full solutions and a cheat sheet. Based on Loewenstein et al., §2.3.1. |

New weeks are added as the course goes on.

## How each week is organised

1. **Part A, the lecture**, rewritten as a textbook chapter.
2. **Part B, the bonus hour**: the mathematical background.
3. **Part C, the TA session**: every worked example solved in full.
4. **Practice problems** with full solutions, and a **cheat sheet**.

The colour-coded boxes are:

| Box | Colour | Meaning |
|---|---|---|
| DEF | green | definition |
| KEY IDEA | pink | intuition |
| FORMULA | purple | key fact or result |
| EXAMPLE | blue | worked example |
| PITFALL | gold | common mistake or slide correction |

## Building from source

The notes are plain LaTeX (pdfLaTeX with tcolorbox, TikZ and pgfplots):

```sh
pdflatex -interaction=nonstopmode week01.tex
pdflatex -interaction=nonstopmode week01.tex   # second run for the contents
# likewise for week02.tex, ...
```

## Sources and credits

- The course lectures and TA sessions (Y. Loewenstein, Y. Burak and the teaching assistants).
- Y. Loewenstein, G. Mongillo, I. Landau and L. Fox, *The Dynamics of Computation in Neuronal Networks* (draft). Its explanations are cited in the text as [LMLF].

The figures in `figures/` are taken from the lecture slides and remain the property of their original authors. They are reproduced here for study purposes, with the original references given in the captions.

These are unofficial student notes. If you find an error, please open an issue.
