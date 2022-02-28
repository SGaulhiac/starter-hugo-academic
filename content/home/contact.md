---
# An instance of the Contact widget.
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 130

title: Contact
subtitle:

content:
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

  # Contact details (edit or remove options as required)
  email: gaulhiac@ualberta.ca
  #phone: 888 888 88 88
  address: 
    street: Mathematical and Statistical Sciences
    University of Alberta
    city: Edmonton
    region: AB
    postcode: 'T6G 2G1'
    country: Canada
    country_code: CA
  coordinates:
    latitude: '37.4275'
    longitude: '-122.1697'
  #directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
  
  

design:
  columns: '2'
---
