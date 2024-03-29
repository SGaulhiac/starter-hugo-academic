---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  # - block: features
  #  content:
  #   title: Skills
  #  items:
  #      - name: R
  #        description: 90%
  #        icon: r-project
  #        icon_pack: fab
 # - block: experience
  #  content:
   #   title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
    #  date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
     # items:
      #  - title: CEO
      #   company: GenCoin
      #   company_url: ''
      #   company_logo: org-gc
      #   location: California
      #   date_start: '2021-01-01'
      #   date_end: ''
      #   description: |2-
      #        Responsibilities include:

      #        * Analysing
      #        * Modelling
      #        * Deploying
  
    
  - block: portfolio
    id: research
    content:
      title: Research
      filters:
        folders:
          - publication
        exclude_featured: true
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
        - name: Publications
          tag: Publications
        - name: Preprint
          tag: Preprint
        - name: PhD thesis
          tag: PhD
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: citation
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
    # design:
      # columns: '2'
      # view: citation
      
  - block: collection
    id: notes
    content:
      title: Notes and Slides
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
    
 # - block: features
 #  id: teaching
 #  content:
 #     title: Teaching
 #     items:
 #       - title: Calculus 1, Math100
 #         company: Instructor
 #         company_url: ''
 #         location: University of Alberta
 #         date_start: '2021'
 #         date_end: '2022'
 #       - title: Differential equations (level L2)
 #         company: Teaching Assistant
 #         location: Sorbonne Université
 #         date_start: '2019'
 #         date_end: '2020'
 #   # design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      # columns: '2'
      # view: citation
      # For Showcase view, flip alternate rows?
      # flip_alt_rows: false
  
 # - block: collection
 #   id: featured
 #   content:
 #     title: Featured Publications
 #     filters:
 #       folders:
 #         - publication
 #       featured_only: true
 #   design:
 #     columns: '2'
 #     view: card
  
  - block: collection
    id: music
    content:
      title: Music
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      # Contact (add or remove contact options as necessary)
      email: sgaulhiac@impan.pl
      # phone: 888 888 88 88
      # appointment_url: ""
      address:
        street: 'ul. Sniadeckich 8'
        city: Warsaw
        #region: CA
        postcode: '00-656'
        country: Poland
        country_code: PL
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
       #  - 'Monday 10:00 to 13:00'
       # - 'Wednesday 09:00 to 10:00'
      # contact_links:
      #  - icon: twitter
       #   icon_pack: fab
       #  name: DM Me
       # link: 'https://twitter.com/Twitter'
       # - icon: skype
       #   icon_pack: fab
       #   name: Skype Me
       #   link: 'skype:echo123?call'
       # - icon: video
       #   icon_pack: fas
       #   name: Zoom Me
       #   link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
