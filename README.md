<p align="center">
  <img alt="pluto-logo" src="resources/pluto_logo_rounded_corners.png" width="300">
  <h3 align="center">Enabling Massively Parallel Computation in DRAM via Lookup Tables</h3>
</p>

<p align="center">
    <a href="https://github.com/CMU-SAFARI/pLUTo/blob/master/LICENSE">
        <img alt="GitHub" src="https://img.shields.io/badge/License-MIT-yellow.svg">
    </a>
    <a href="https://github.com/CMU-SAFARI/pLUTo/releases">
        <img alt="GitHub Release" src="https://img.shields.io/github/release/CMU-SAFARI/pLUTo">
    </a>
  <br>
    <a href="https://doi.org/10.1109/MICRO56248.2022.00067"><img src="https://img.shields.io/badge/DOI-10.1109/MICRO56248.2022.00067-blue" alt="MICRO DOI"></a>
    <a href="https://doi.org/10.48550/arXiv.2104.07699"><img src="https://img.shields.io/badge/DOI-10.48550/arXiv.2104.07699-blue" alt="arXiv DOI"></a>
    <a href="https://doi.org/10.5281/zenodo.6942058"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.6942058.svg" alt="Zenodo DOI"></a>
</p>

This repository contains the artifact evaluation materials associated with the MICRO 2022 submission of [pLUTo: Enabling Massively Parallel Computation
In DRAM via Lookup Tables](pLUTo.pdf).

Two artifacts are provided:

1. The SPICE simulations (used to produce Figure 6 in the paper).
2. The pLUTo simulation model (used to produce Figures 7-13 in the paper).

The instructions to reproduce each of the artifacts are provided in `README.md` files in their respective directories.

<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#what-is-pluto">What is pLUTo?</a></li>
    <li><a href="#repository-structure">Repository Structure</a></li>
    <li><a href="#execution-instructions">Execution Instructions</a></li>
    <li><a href="#citation">Citation</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## What is pLUTo?

## Repository Structure

We point out next the repository structure and some important folders and files.
All benchmark folders have similar structure to the one shown for BFS.
The microbenchmark folder contains eight different microbenchmarks, each with similar folder structure.
The repository also includes `run_*.py` scripts to run strong and weak scaling experiments for PrIM benchmarks.

```
.
+-- LICENSE
+-- README.md
+-- run_strong_full.py
+-- run_strong_rank.py
+-- run_weak.py
+-- BFS/
|   +-- baselines/
|	|	+-- cpu/
|	|	+-- gpu/
|   +-- data/
|   +-- dpu/
|   +-- host/
|   +-- support/
|   +-- Makefile
+-- BS/
|   +-- ...
+-- GEMV/
|   +-- ...
+-- HST-L/
|   +-- ...
+-- HST-S/
|   +-- ...
+-- MLP/
|   +-- ...
+-- Microbenchmarks/
|   +-- Arithmetic-Throughput/
|   +-- CPU-DPU/
|   +-- MRAM-Latency/
|   +-- Operational-Intensity/
|   +-- Random-GUPS/
|   +-- STREAM/
|   +-- STRIDED/
|   +-- WRAM/
+-- NW/
|   +-- ...
+-- RED/
|   +-- ...
+-- SCAN-SSA/
|   +-- ...
+-- SCAN-RSS/
|   +-- ...
+-- SEL/
|   +-- ...
+-- SpMV/
|   +-- ...
+-- TRNS/
|   +-- ...
+-- TS/
|   +-- ...
+-- UNI/
|   +-- ...
+-- VA/
|   +-- ...
```

## Execution Instructions

## Citation

Please cite pLUTo as follows:

_João Dinis Ferreira, Gabriel Falcao, Juan Gómez-Luna, Mohammed Alser, Lois Orosa, Mohammad Sadrosadati, Jeremie S. Kim, Geraldo F. Oliveira, Taha Shahroodi, Anant Nori, and Onur Mutlu. ["pLUTo: Enabling Massively Parallel Computation in DRAM via Lookup Tables".](https://arxiv.org/abs/2104.07699) In Proceedings of the 55th Annual IEEE/ACM International Symposium on Microarchitecture (MICRO), 2022. https://doi.org/10.1109/MICRO56248.2022.00067._

You can also use the following BibTeX entry for this purpose:

```bibtex
@inproceedings{ferreira2022pluto,
  author = {Ferreira, João Dinis and Falcao, Gabriel and Gómez-Luna, Juan and Alser, Mohammed and Orosa, Lois and Sadrosadati, Mohammad and Kim, Jeremie S. and Oliveira, Geraldo F. and Shahroodi, Taha and Nori, Anant and Mutlu, Onur},
  title = {{pLUTo: Enabling Massively Parallel Computation in DRAM via Lookup Tables}},
  doi = {10.1109/MICRO56248.2022.00067},
  booktitle = {Proceedings of the 55th Annual IEEE/ACM International Symposium on Microarchitecture (MICRO)},
  year = {2022}
}
```

## License

Distributed under the MIT License. See LICENSE for more information.

## Contact

João Dinis Ferreira - hello@joaof.eu

## Acknowledgements

We acknowledge support from SAFARI Research Group's industrial partners.
