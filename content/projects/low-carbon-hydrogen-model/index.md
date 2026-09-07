---
title: "Low-Carbon Hydrogen Optimization Model"
date: "2026-03-11T00:00:00Z"
summary: "Open-source model code that reproduces the Power-to-Gas results behind my Nature Communications paper on carbon accounting rules for hydrogen."
tags:
  - Green hydrogen
  - Carbon accounting
  - Optimization
  - Reproduction code

image:
  alt_text: "Stainless-steel process piping with valves and pressure gauges at an industrial plant."
links:
  - type: code
    url: https://github.com/phholler/Low-Carbon-Hydrogen-Model-Reproduction
    label: "View on GitHub"
---

The optimization model behind
[*How Carbon Accounting Rules Shape Incentives for Hydrogen Production*](/publications/carbon-accounting-hydrogen/),
released so that the published results can be reproduced and extended. Written
in **Python** as Jupyter notebooks, it simulates and optimizes the operation and
capacity choice of **Power-to-Gas** systems under alternative carbon accounting
rules, with electricity prices, capacity factors, technology costs and policy
support all exposed as inputs.

Unlike the other entries here this is not an interactive calculator but the
research code itself, for readers who want to verify the reported numbers or
apply the model to a different setting. The paper is joint work with Gunther
Glenk and Stefan Reichelstein.
