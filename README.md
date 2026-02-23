# UK-NNSS High Performance Conjugate Gradients (HPCG) benchmark

This repository contains the instructions for running the standard HPCG
benchmark as part of the UK-NNSS procurement.

## Status

Stable

## Maintainers

- @aturner-epcc ([https://github.com/aturner-epcc](https://github.com/aturner-epcc))

## Overview

### Software

- [HPCG](https://www.hpcg-benchmark.org/)


## Building the benchmark

**Important:** All results submitted should be based on a version of HPCG that
meets [Top500 submission guidelines](https://www.hpcg-benchmark.org/faq/index.html).

### Permitted modifications

Offerors are permitted to modify the benchmark in any way compatible with Top500
submission guidelines.

## Running the benchmark

### Required tests

The bidder is required to run the following tests

- Single node HPCG performance
  + Single node HPCG runs across all compute nodes that run for at least 30 minutes on each node
  + The difference between the maximum measured single-node performance and the minimum
    measured single-node performance must be equal to or less than 5% of the mean measured single-node performance.
- Full system HPCG performance
  + A full system run of HPCG using a minimum of 99% of all compute nodes under Top500 
    submission rules that runs for at least 30 minutes
  + This run should provide data for a valid Top500 submission

## Reporting results

The primary figure of merit (FoM) is the HPCG performance in GFLOP/s.

The bidder should provide:

- For the single node runs: the minimum, maximum and mean single node HPCG performance
  across all nodes
- Details on how the tests were run, including any batch job submission
  scripts and HPCG input files
- All data printed to STDOUT by the HPCG software for all HPCG runs (single node and full system)
- Data on energy use (in kWh) for each HPCG run and peak power draw (in kW)
  for each HPCG run (per node for single node runs and aggregate for full system runs)

## License

This benchmark description and associated files are released under the MIT license.
