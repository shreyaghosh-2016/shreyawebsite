---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: featured
    content:
      title: Featured Publications 
      text: |-
        {{% callout note %}}
        **See Full Publication** [here](https://shreyaghosh-2016.github.io/publications) 
        [**Google Scholar Link**](https://scholar.google.com/citations?user=a5OKo7wAAAAJ&hl=en)
        {{% /callout %}}
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '1'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Postdoctoral scholar
          company: The Pennsylvania State University
          company_url: ''
          company_logo: org-gc
          location: Pennsylvania, USA
          date_start: '2021-12-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Research (Misinformation detection)
              * Research (Wildlife informatics)
              * Student Mentoring and assisting in their research
        - title: Senior research associate
          company: Indian Institute of Technology Kharagpur (IIT Kharagpur)
          company_url: ''
          company_logo: iitkgp
          location: Kharagpur, India
          date_start: '2021-01-01'
          date_end: '2021-11-30'
          description: Led research project on COVID-19 and mentored undergraduate and postgraduate students.
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2021-01-25'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Neural Networks and Deep Learning
          url: ''
        - certificate_url: https://www.edx.org
          date_end: ''
          date_start: '2021-01-01'
          description: Formulated informed blockchain models, hypotheses, and use cases.
          organization: edX
          organization_url: https://www.edx.org
          title: Blockchain Fundamentals
          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
        - certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'Object-Oriented Programming in R'
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
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
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    id: section-1
    content:
      title: Section 1
      subtitle: A subtitle
      text: Add any **markdown** formatted content here - text, images, videos, galleries - and even HTML code!

  
  
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  
  - block: features
    content:
      title: Skills
      items:
        - name: Mobility analysis
          #description: 100%
          icon: car
          icon_pack: fas
        - name: Natural lanuage processing
          #description: 100%
          icon: list-check
          icon_pack: fas
        - name: Social media data analytics
          #description: 10%
          icon: magnifying-glass-chart
          icon_pack: fas
        - name: Cloud computing
          #description: 100%
          icon: cloud
          icon_pack: fas
        - name: Data mining
          #description: 100%
          icon: magnifying-glass-chart
          icon_pack: fa
        - name: Python, R, C, PostGreSQL, QGIS, TensorFlow
          #description: 10%
          icon: fa-python
          icon_pack: fa
  
  - block: contact
    id: contact
    content:
      title: Contact
      #subtitle:
      #text: |-
      #Contact (add or remove contact options as necessary)
      email: shreya.cst@gmail.com
      phone: 814-769-3989
      #appointment_url: 'https://calendly.com'
      address:
        street: 413A Eric J. Barron Innovation Hub
        city: State College
        region: PA
        postcode: '16801'
        country: United States
        country_code: US
      #directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/cstghosh'
        
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://psu.zoom.us/my/shreya2022'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      
    design:
      columns: '2'
---
