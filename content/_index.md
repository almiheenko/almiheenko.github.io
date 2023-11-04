---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  - block: features
    id: skills
    content:
      title: Skills
      items:
        - name: Programming
          description: 'Python, R, Bash, cluster managers. Supervised/unsupervised machine learning, deep learning'
          #percent: 80
          icon: code
          icon_pack: fas
        - name: Genomics
          description: 'Next‐generation and long‐read genome sequencing data, metagenomics, ChIP‐seq'
          icon: dna
          icon_pack: fas
        - name: Transcriptomics & Proteomics
          description: 'Single‐cell, spatial, bulk RNA‐Seq data. Mass-spectrometry‐based quantitative proteomics data'
          icon: database
          icon_pack: fas
        - name: Algorithms
          description: 'Implementation and development of bioinformatic algorithms'
          icon: circle-nodes 
          icon_pack: fas
          #design:
          #  columns: '1'

  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: Card
      # For Showcase view, flip alternate rows?
      #flip_alt_rows: false
    sort_by: 'Date'
  - block: collection
    id: publications
    content:
      title: Publications
      text: 
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '1'
      view: citation
    sort_by: 'Date'
  - block: portfolio
    id: teaching
    content:
      title: Teaching Positions 
      filters:
        folders:
          - teaching
        featured_only: false
    design:
      columns: '1'
      view: showcase
    sort_by: 'Date'
---
