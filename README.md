# Benchmarking Debye-Calculated Vibrational Entropies Against Phonon Calculations

**Northeastern University | Data-Driven Renewables Research Lab | Summer & Fall 2026**

Project Researcher: Kiyan Heidari<br>
Research Advisor: Prof. Peter Schindler

## Overview

This project investigates the accuracy and computational efficiency of Debye-based approximations for predicting vibrational entropy in crystalline materials.

Two approaches are benchmarked against phonon-based calculations:

1. **Bulk Modulus Debye Model:** Uses bulk elastic properties to approximate vibrational entropy.
2. **Bulk and Shear Modulus Debye Model:** Incorporates both bulk and shear elastic properties.

The objective is to evaluate whether computationally inexpensive Debye approximations can provide reliable estimates of vibrational entropy across materials and temperatures.

## Research Objectives

- Benchmark Debye-based vibrational entropy predictions against phonon calculations.
- Compare the accuracy of bulk-only and bulk-and-shear formulations.
- Quantify temperature-dependent model error at 20 K, 100 K, 300 K, and 600 K.
- Evaluate computational runtime and accuracy-efficiency tradeoffs.
- Identify limitations of low-cost vibrational entropy approximations.

## Methodology

A computational benchmarking workflow was used to evaluate both Debye formulations against reference phonon calculations across 158 materials.

Model performance was analyzed using:

- Predicted versus reference entropy scatter plots.
- Signed prediction errors across temperatures.
- Computational runtime distributions.
- Comparisons of model accuracy and systematic bias.

## Results

### Agreement with Phonon Calculations

At 20 K, both Debye formulations show limited agreement with phonon-based entropy calculations.

Agreement improves at higher temperatures, although material-dependent deviations remain.

### Accuracy Comparison

The bulk-modulus formulation exhibits lower average absolute error at lower temperatures, while including shear information provides modest improvements at higher temperatures.

The bulk-and-shear approach does not consistently outperform the simpler model.

### Computational Efficiency

Median runtimes:

| Method | Median Runtime |
|---|---:|
| Bulk Modulus Debye | 0.62 s |
| Bulk and Shear Debye | 1.98 s |
| Phonon-Based | 12.82 s |

Both Debye formulations provide substantial computational savings relative to phonon-based calculations.

## Key Takeaways

- Debye-based approximations offer significantly lower computational costs.
- Adding shear modulus information does not guarantee better predictions.
- The simplest approximation may offer a favorable accuracy-cost tradeoff for high-throughput materials screening.
- Debye approximations simplify the vibrational behavior of crystalline materials and cannot fully capture material-specific phonon characteristics.

## Research Presentation

See `CollectiveGraphs.png` for the research results.
