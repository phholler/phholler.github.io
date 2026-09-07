---
title: 'Projects'
date: 2024-05-19
type: landing

# Page sections
sections:
  - block: markdown
    id: projects-intro
    content:
      text: |-
        # Projects

        Tools and code I have built alongside my research and released publicly:
        interactive calculators that make the underlying techno-economic models
        available to others, and the model code behind published papers. The aim
        is the same in both cases — the assumptions behind the results should be
        open to inspection, reproduction and reuse.
    design:
      columns: '1'
  - block: collection
    id: project-list
    content:
      title: ''
      filters:
        folders:
          - projects
    design:
      # Sits directly under the intro block, so drop its own top padding.
      spacing:
        padding: ['0', '0', '3rem', '0']
      view: article-grid
      fill_image: false
      columns: 2
      show_date: false
      show_read_time: false
      show_read_more: false
---
