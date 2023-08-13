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
        - name: Misinformation
          tag: misinformation
        - name: Mobility
          tag: Mobility
        - name: Night time light
          tag: Night time light
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: experience
    id: experience
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
          company_url: 'https://www.psu.edu/'
          company_logo: org-gc
          location: Pennsylvania, USA
          date_start: '2021-12-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * **Research (Misinformation detection):** Understanding misinformation propagation in social network and proposing mitigation techniques
              * **Research (Wildlife informatics):** Predicting human wildlife conflicts and mitigating strategies
              * **Research (Night time data analytics)**
              * **Research (Exploring generative language model for cross-domain applications such as trajectory trace analysis)** 
              * Student Mentoring and assisting in their research
              
        - title: Senior research associate
          company: Indian Institute of Technology Kharagpur (IIT Kharagpur)
          company_url: 'https://www.iitkgp.ac.in/'
          company_logo: iitkgp
          location: Kharagpur, India
          date_start: '2021-01-01'
          date_end: '2021-11-30'
          description: Led research project on COVID-19 and mentored undergraduate and postgraduate students. • Analysis of mobility and other context and predicting COVID-19 hotspots and assisting in zone-based lockdown strategy. • Socio-economical impacts of COVID-19 at India
              
        - title: PhD research scholar
          company: Indian Institute of Technology Kharagpur (IIT Kharagpur)
          company_url: 'https://www.iitkgp.ac.in/'
          company_logo: iitkgp
          location: Kharagpur, India
          date_start: '2016-08-01'
          date_end: '2020-12-30'
          description: |2-
              Research projects include:

              * Analysis of large scale GPS traces to explore human movement behaviours and Transferring mobility knowledge from source to target region to annotate trajectory trips and POI-classification

              

              * Temporal fingerprinting of individuals by modelling and analysing their activity patterns

              * Cloud-fog-edge-IoT based collaborative framework to facilitate applications related to improved health-care, transportation and urban planning in less delay along with less energy consumption

              * Developed Activity-aware Internet of Health Things (IoHT), and Mobility-aware Internet of Spatial Things (Mobi-IoST)
              
        - title: MS research scholar
          company: Indian Institute of Technology Kharagpur (IIT Kharagpur)
          company_url: 'https://www.iitkgp.ac.in/'
          company_logo: iitkgp
          location: Kharagpur, India
          date_start: '2015-08-01'
          date_end: '2016-12-30'
          description: |2-
              Research projects include:

              * Decision Support System for transportation of hazardous materials

              

              * Designed a SDI (Spatial Data Infrastructure) to assist in routing decisions regarding transportation of hazardous materials
              
        - title: Undergraduate research project
          company: Indian Institute of Engineering Science and Technology, Shibpur (IIEST)
          company_url: 'https://www.iiests.ac.in/'
          company_logo: iiest
          location: Shibpur, India
          date_start: '2014-08-01'
          date_end: '2015-12-30'
          description: |2-
              Research projects include:

              * Decision Support System for transportation of hazardous materials

              

              * Designed a SDI (Spatial Data Infrastructure) to assist in routing decisions regarding transportation of hazardous materials
    design:
      columns: '2'
  - block: accomplishments
    id: posts
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Recent News!'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: 
          date_end: ''
          date_start: '2023-11-13'
          description: 'In collaboration with ACM SIGSPATIAL, we are pleased to announce the call for papers for [GeoWildLife 2023](https://geowildlife2023.ist.psu.edu/), a workshop dedicated to bridging the gap between AI-enabled spatio-temporal data analytics and wildlife conservation.'
          organization: SigSpatial
          organization_url: https://sigspatial2023.sigspatial.org/
          title: GeoWildLife 2023!
          url: 'https://geowildlife2023.ist.psu.edu/'
        - certificate_url: 
          date_end: ''
          date_start: '2023-11-13'
          description: 'In collaboration with ACM SIGSPATIAL, we are pleased to announce the call for papers for [GeoSocial 2023](http://www.geosocial.iitkgp.ac.in/). The workshop aims to bring together a diverse community of researchers, practitioners, and students from various disciplines to exchange ideas, share knowledge, and foster collaboration in the burgeoning field of geocomputational and socio-economic data analysis.'
          organization: SigSpatial
          organization_url: https://sigspatial2023.sigspatial.org/
          title: GeoSocial 2023!
          url: 'http://www.geosocial.iitkgp.ac.in/'
        - certificate_url: 
          date_end: ''
          date_start: '2023-10-22'
          description: 'In collaboration with CIKM 2023, we are pleased to announce the call for papers for [InfoWild 2023](https://wildinfo.ist.psu.edu/), a workshop dedicated to explore and enhance AI’s role in big data analysis for wildlife conservation, in brief, Nature Through the Lens of AI . It seeks to address crucial challenges related to data heterogeneity, scale integration, data privacy, mitigating biases, and decision-making under uncertainty. This workshop is centred around leveraging AI’s prowess in deciphering complex spatio-temporal data patterns for wildlife conservation, thereby contributing significantly to the broader canvas of AI for social good.'
          organization: CIKM
          organization_url: https://uobevents.eventsair.com/cikm2023/
          title: InfoWild 2023!
          url: 'https://wildinfo.ist.psu.edu/'
    design:
      columns: '2'

  
  
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
          icon_pack: fas
        - name: Python, R, C, PostGreSQL, QGIS, TensorFlow
          #description: 10%
          icon: list-check
          icon_pack: fas
  
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
