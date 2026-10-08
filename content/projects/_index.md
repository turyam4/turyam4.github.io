---
title: 'Blogs & Projects'
date: 2024-05-19
type: landing

design:
  # Section spacing
  spacing: '5rem'

# Page sections
sections:
  - block: collection
    content:
      title: Selected Projects
      text: A focused selection of my work in graph machine learning and related research projects.
      filters:
        folders:
          - projects
    design:
      view: card
      fill_image: false
      columns: 1
      show_date: false
      show_read_time: false
      show_read_more: true

  - block: collection
    content:
      title: Recent Experiences & Blogs
      text: Latest updates from workshops, summer schools, and research experiences.
      filters:
        folders:
          - events
    design:
      view: card
      fill_image: true
      columns: 1
      show_date: true
      show_read_time: true
      show_read_more: true
---
