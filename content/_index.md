---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
    # Default section spacing
    spacing: '6rem'

sections:
    - block: resume-biography-3
      id: about
      content:
          # Choose a user profile to display (a folder name within `content/authors/`)
          username: admin
          text: ''
      design:
          css_class: dark
          background:
              color: black
              image:
                  # Add your image background to `assets/media/`.
                  filename: stacked-peaks.svg
                  filters:
                      brightness: 1.0
                  size: cover
                  position: center
                  parallax: false
    - block: collection
      id: news
      content:
          title: 📰 Recent News
          subtitle: ''
          text: ''
          # Page type to display. E.g. post, talk, publication...
          page_type: news
          # Choose how many pages you would like to display (0 = all pages)
          count: 2
          # Filter on criteria
          filters:
              author: ''
              category: ''
              tag: ''
              exclude_featured: false
              exclude_future: false
              exclude_past: false
              publication_type: ''
          # Choose how many pages you would like to offset by
          offset: 0
          # Page order: descending (desc) or ascending (asc) date.
          order: desc
      design:
          # Choose a layout view
          view: date-title-summary
    - block: collection
      id: papers
      content:
          title: 🌟 Featured Publications
          filters:
              folders:
                  - publication
              featured_only: true
      design:
          view: citation
          columns: 1
    - block: collection
      content:
          title: 📝 Recent Publications
          text: ''
          filters:
              folders:
                  - publication
              author: ''
              category: ''
              tag: ''
              publication_type: ''
              exclude_featured: true
      design:
          columns: '2'
          view: citation
---
