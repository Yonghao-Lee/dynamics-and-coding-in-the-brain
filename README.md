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
| 02 | [**week02.pdf**](week02.pdf) | **The autapse** (a neuron with a synapse onto itself) with a linear activation function: fixed points, amplification by feedback, stability by perturbation analysis, the full solution r(t), the vector-field picture, and the link to Week 1's eigenvalues. **Non-linear autapse** with a logistic activation function: graphical fixed points, local vs. global stability, linearisation (λ = Jg′), saddle-node bifurcations and the bifurcation diagram (based on Loewenstein et al., §2.3.1; the lecture stopped just before attractors, which open Week 3). **Bonus hour 2:** linear algebra as geometry: the determinant as an area factor, eigenvectors as stretch directions, linearizing an inhibitory network, decoupling two mutually inhibiting neurons (winner-take-all), eigenvector shortcuts for all-ones, equal-row-sum and symmetric matrices. **TA session 2:** exam 2015 Q2: one excitatory tanh population (pitchfork, proof that the outer states are stable) and an E–I pair (trace–determinant, stable spiral / node / saddle regimes, oscillations). Mistakes in the bonus-hour and TA notes corrected. Practice problems with full solutions and cheat sheets. |
| 03 | [**week03.pdf**](week03.pdf) | **Attractors and bistability** of the autapse: memory written by a brief input pulse, the two ingredients (positive feedback and saturation), half-stable fixed points. **Mutual inhibition**: the homogeneous fixed point, the Jacobian, network modes (homogeneous and heterogeneous eigenvectors), symmetry breaking and the pitchfork bifurcation, disinhibition, basins of attraction and the separatrix, decision making and perceptual bistability. **Excitation and inhibition**: the E–I pair with a threshold-linear activation, its unique fixed point, trace/determinant stability, the Hopf bifurcation, limit cycles and oscillations from delayed negative feedback (Loewenstein et al., §2.3.1–2.3.3; the lecture stopped before §2.3.4). Book errors corrected. Practice problems with full solutions and a cheat sheet. |

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

The figures in `figures/` are taken from the lecture slides and the course book [LMLF] and remain the property of their original authors. They are reproduced here for study purposes, with the original references given in the captions.

These are unofficial student notes. If you find an error, please open an issue.
