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
    - block: markdown
      id: contact
      content:
          title: Contact
          text: '<b>University of Jaén</b> <br>
              Computer Science Department <br>
              A3-241 <br>
              Campus Las Lagunillas, 23071, Jaén | +34 953 21 24 76 <br>
              <a href="https://uvirtual.ujaen.es/pub/es/informacionacademica/tutorias/p/75194"><it>Office hours:</it></a> <br>
              - Tuesday: 17:30-18:30 <br>
              - Thursday: 16:30-17:30 <br>
              - Friday: 9:00-13:30 <br>'
---
