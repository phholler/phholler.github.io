---
title: Papers
type: landing
cms_exclude: true

sections:
  - block: markdown
    content:
      text: |-
        # Papers
    design:
      columns: '1'
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publications
    design:
      view: citation
  - block: collection
    id: working-papers
    content:
      title: Working papers
      filters:
        folders:
          - working-papers
    design:
      view: citation
---
