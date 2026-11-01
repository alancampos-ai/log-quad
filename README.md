# Logarithmic-quadratic algorithm

#### Article: <small><strong>A logarithmic-quadratic algorithm for vector optimization</strong> <a href=""><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a> <a href=""><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a> <a href="https://drive.google.com/drive/folders/16uPBllfo0AtHJPpoD4PN4eJzginXYtKX?usp=sharing"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We develop a logarithmic–quadratic primal–dual method for cone-ordered convex vector optimization. A normalized dual weight evolves jointly with the primal variable via barrier and quadratic regularization. We establish maximal monotonicity, existence under attainment conditions, and exact and summably inexact convergence to weak Pareto solutions. Strong monotonicity yields contraction and perturbation bounds. Experiments compare eleven methods on orthant, Lorentz-cone, and vector Tikhonov problems at $n=1600$ with 20 paired seeds. At representative settings, mean stationarity residuals are $2.237\times10^{-12}$, $4.300\times10^{-2}$, and $2.945\times10^{-9}$, with success rates of $100\%$, $5\%$, and $100\%$; scalarization succeeds in $75\%$ of Lorentz runs. The stationarity comparisons with logarithmic–quadratic scalarization have Holm-adjusted $p$-values of $1.907\times10^{-5}$, $0.125$, and $1.907\times10^{-5}$.

#### Dependencies

The experiments used Ubuntu 24.04.4 LTS and Python 3.12.12 with the following dependencies:

* NumPy 2.3.5
* SciPy 1.17.0
* Matplotlib 3.10.8
* psutil 7.2.2
* PyYAML 6.0.3

#### Installation

```bash
docker build --pull -f docker/Dockerfile -t k-optim:9.0.0 .
docker run --rm -v k-optim-workspace:/workspace k-optim:9.0.0
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
