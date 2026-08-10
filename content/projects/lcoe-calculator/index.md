---
title: "LCOE Calculator — U.S. solar & wind"
date: "2026-06-15T00:00:00Z"
summary: "An interactive tool estimating the levelized cost of electricity for solar and wind across U.S. states and market segments."
tags:
  - Levelized cost of electricity
  - Solar
  - Wind
  - Interactive tool

image:
  alt_text: "Wind turbines standing in farmland under a clear sky."
links:
  - type: site
    url: https://huggingface.co/spaces/UniMaMISES/LCOE_calculator_shiny
    label: "Open in a new tab"
---

An interactive web application, built with **Shiny for Python**, that estimates the **levelized cost of electricity (LCOE)** for **solar and wind across U.S. states**. Costs can be compared across the utility, commercial, and residential segments, and wind capacity factors can be derived from alternative reanalysis datasets (HRRR, ERA5, MERRA2). The tool combines modelled hourly capacity factors with technology cost assumptions to show how generation costs vary by location and market segment.

A collaboration with Thimo Merke and Minghao Chen.

<div style="margin: 1.5rem 0;">
  <iframe
    src="https://unimamises-lcoe-calculator-shiny.hf.space"
    title="LCOE Calculator — U.S. solar and wind"
    style="width: 100%; height: 820px; border: 1px solid #e5e7eb; border-radius: 12px;"
    loading="lazy"
    allow="fullscreen">
  </iframe>
</div>
