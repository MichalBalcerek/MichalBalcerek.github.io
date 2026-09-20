---
layout: page
title: Research
permalink: /research/
nav: true
nav_order: 1
math: true
description: Stochastic models, memory, and statistical evidence from trajectories.
---

My research concerns **stochastic processes, anomalous diffusion, and statistical inference**.
I study how memory, heterogeneity, and dependence between spatial directions shape random motion,
and how these properties can be recognised in observed trajectories. Single-particle tracking
provides an important connection between the mathematical models and experiments in living cells.

## Current research

### Anomalous diffusion

I study stochastic models of motion whose mean-squared displacement does not grow linearly with time.
Current work includes heterogeneous and switching diffusion, non-Gaussian behaviour, and
two-dimensional models with dependent components. The aim is to connect features of a trajectory
with the mechanisms represented by its mathematical model.

### Long-memory processes

Fractional Brownian motion and its extensions provide models in which past and future increments
are dependent. I am interested in how this dependence changes when diffusivity or the Hurst
exponent varies across trajectories or evolves in time. Recent work includes multifractional
models with a stochastically varying exponent and the analysis of covariance and spectral structure.

### Statistical inference

I develop and study methods for identifying stochastic models and estimating their parameters
from data. This includes distinguishing diffusion regimes, detecting changes within a trajectory,
assessing Gaussianity, and accounting for measurement noise. Statistical methods and simulations
help connect theoretical properties with the short, imperfect trajectories available in experiments.

## Methods

Stochastic modelling · covariance and spectral analysis · hypothesis testing · parameter estimation ·
change-point detection · numerical simulation · statistical and machine-learning methods

## Technical overviews

The notes below introduce representative models and questions behind these directions.
Open a topic for equations, a short explanation, and links to related papers.

<details class="technical-overview" markdown="1">
<summary>Fractional Brownian motion: memory and a changing Hurst exponent</summary>

A standard fractional Brownian motion $$B_H(t)$$ is a centred Gaussian process with covariance

$$
\mathbb{E}[B_H(t)B_H(s)]
=\frac{1}{2}\left(t^{2H}+s^{2H}-|t-s|^{2H}\right),
\qquad 0<H<1.
$$

Its mean-squared displacement grows as $$t^{2H}$$. The value $$H=1/2$$ gives Brownian motion;
for $$H>1/2$$, increments have positive, long-range dependence, while $$H<1/2$$ gives
negatively correlated increments.

A single exponent may be too restrictive for heterogeneous systems. My work with collaborators
considers both random exponents and exponents that evolve during a trajectory. In telegraphic
multifractional Brownian motion, a smoothed switching process drives the Hurst exponent.
This gives a tractable model for changing memory and a way to investigate such changes in data.

**Representative papers:**
[Random Hurst exponent (2022)]({{ '/publications/#BalcerekEtAl2022RandomH' | relative_url }}) ·
[Telegraphic multifractional Brownian motion (2025)]({{ '/publications/#BalcerekEtAl2025Telegraphic' | relative_url }})

</details>

<details class="technical-overview" markdown="1">
<summary>Two-dimensional anomalous diffusion</summary>

A planar trajectory contains information that is lost when each coordinate is analysed separately.
One starting point for a dependent model is a pair of correlated Brownian drivers:

$$
\widetilde W_1(t)=W_1(t),\qquad
\widetilde W_2(t)=\rho W_1(t)+\sqrt{1-\rho^2}\,W_2(t),
\qquad |\rho|\leq 1,
$$

where $$W_1$$ and $$W_2$$ are independent two-sided Brownian motions. Memory enters through the
**causal Mandelbrot–van Ness kernel**,

$$
K_H(t,s)=a_H\left[(t-s)_+^{H-\frac12}-(-s)_+^{H-\frac12}\right],
\qquad
a_H=\frac{\sqrt{\Gamma(2H+1)\sin(\pi H)}}{\Gamma(H+\frac12)}.
$$

Here $$x_+^\alpha=x^\alpha$$ for $$x>0$$ and zero otherwise, including when $$\alpha=0$$.
For $$t\geq0$$, the two coordinates are

$$
X_j(t)=\sigma_j\int_{\mathbb R}K_{H_j}(t,s)\,\mathrm d\widetilde W_j(s),
\qquad j=1,2,\quad H_j\in(0,1),\quad\sigma_j>0.
$$

The normalization gives $$\operatorname{Var}[X_j(t)]=\sigma_j^2t^{2H_j}$$, allowing different
scaling in each direction. When $$H_j=1/2$$, the kernel reduces to the indicator of
$$[0,t)$$ and that coordinate becomes scaled Brownian motion.

My recent work with collaborators studies the resulting two-dimensional fractional Brownian
motion through its auto-covariances, cross-covariances, and power spectra. Related work on turning
angles examines how directional dependence appears in the geometry of trajectories. These
complementary descriptions help distinguish temporal memory from dependence between coordinates.

**Representative papers:**
[Turning-angle analysis (2025)]({{ '/publications/#BalcerekEtAl2025TurningAngles' | relative_url }}) ·
[Two-dimensional fractional Brownian motion (2026)]({{ '/publications/#BalcerekEtAl2026TwoDimensionalFBM' | relative_url }})

</details>

<details class="technical-overview" markdown="1">
<summary>Inference from trajectories: changing dynamics and non-Gaussianity</summary>

For sampled positions $$X_0,\ldots,X_N$$, a basic statistic is the time-averaged mean-squared displacement,

$$
\overline{\delta^2}(m)
=\frac{1}{N-m+1}\sum_{i=0}^{N-m}\|X_{i+m}-X_i\|^2,
\qquad 1\leq m\leq N.
$$

Its dependence on the lag $$m$$ describes the scale of motion, but does not by itself identify
the underlying process. Short trajectories, measurement noise, and changes of diffusion regime
make the inference problem harder.

My work includes tests for fractional models and methods for detecting changes within a
trajectory. In the collaborative CINNAMON method, statistical tools are combined with neural
networks and features extracted from trajectories to classify motion, locate change points,
and estimate parameters between them.

A complementary question concerns the displacement distribution. For a centred scalar
displacement $$Z$$, kurtosis is

$$
K=\frac{\mathbb{E}[Z^4]}{\mathbb{E}[Z^2]^2}.
$$

A Gaussian distribution has $$K=3$$. Our work on heterogeneous fractional Brownian motion
studies how fluctuating diffusivity changes this statistic and compares it with distributional
distances. Kurtosis is a useful diagnostic, although the value three alone does not establish Gaussianity.

**Representative papers:**
[Testing in a noisy environment (2020)]({{ '/publications/#BalcerekBurnecki2020NoisyFBM' | relative_url }}) ·
[Evaluating Gaussianity (2025)]({{ '/publications/#BalcerekEtAl2025Gaussianity' | relative_url }}) ·
[CINNAMON (2025)]({{ '/publications/#MalinowskiEtAl2025CINNAMON' | relative_url }})

</details>

## Research projects

Research awards and collaborations supporting these topics include the projects below.

<div class="projects">
  <div class="row row-cols-1 row-cols-md-2">
    {% assign sorted_projects = site.projects | sort: "importance" %}
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>

<nav class="page-links" aria-label="Further research information">
  <a href="{{ '/projects/' | relative_url }}">All project details →</a>
  <a href="{{ '/publications/' | relative_url }}">All publications →</a>
  <a href="{{ '/students/' | relative_url }}">For students →</a>
</nav>
