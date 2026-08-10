---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-07-21
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'Biography'
        education: 'Education'
        interests: 'Research interests'
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: Research
      subtitle: ''
      text: |-
        My research combines techno-economic analysis with accounting to study how firms and economies can decarbonize at the lowest cost. That includes:

        - **Economics of decarbonization technologies.** Assessing the cost, efficiency, and competitiveness of emerging climate technologies, such as electrolytic ("green") hydrogen and carbon removal technologies.
        - **Carbon accounting and investment incentives.** How alternative carbon accounting rules shape firms' production and investment decisions.
        - **Carbon removal portfolios.** Comparing carbon removal pathways over time and designing cost-effective, dynamic removal portfolios.

        Happy to chat about any related question!
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Selected papers
      filters:
        folders:
          - publications
          - working-papers
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Further papers
      text: ''
      filters:
        folders:
          - publications
          - working-papers
        exclude_featured: true
    design:
      view: citation
---
