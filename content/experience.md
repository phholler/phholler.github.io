---
title: 'CV'
date: 2023-10-24
type: landing
cms_exclude: true

design:
  spacing: '5rem'

# Page sections
sections:
  - block: markdown
    content:
      text: |-
        # Curriculum Vitae

        A full PDF version is available from the [homepage](/).
    design:
      columns: '1'
  - block: resume-experience
    content:
      username: me
    design:
      # Hugo date format (year only, to match the CV's granularity)
      date_format: '2006'
      # Education or Experience section first?
      is_education_first: false
  - block: resume-skills
    content:
      title: Methods & Tools
      username: me
  - block: resume-awards
    content:
      title: Grants & Scholarships
      username: me
    design:
      date_format: '2006'
  - block: markdown
    content:
      title: Languages
      text: |-
        German (native) · English (C2) · French (C2) · Spanish (C1)
    design:
      columns: '1'
---
