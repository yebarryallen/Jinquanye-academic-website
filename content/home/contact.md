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
  email: yebarryallen@gmail.com
  phone: +86 18170671329
  address:
    street: Xuefu Avenue Nanchang University Qianhu Campus
    city: Nanchang
    region: Jiangxi
    postcode: '330000'
    country: China
    country_code: PRC
  coordinates:
    latitude: '28.664'
    longitude: '115.809'
  directions: When you arrive at Gate 3 of the Qianhu Campus of Nanchang University, go straight and turn right into Student Residence Building 9.
  office_hours:
    - 'All day 8:00-20:00'
  appointment_url: 'https://calendly.com'
  contact_links:
    - icon: twitter
      icon_pack: fab
      name: DM Me
      link: 'https://twitter.com/yebarryallen'
    - icon: video
      icon_pack: fas
      name: Zoom Me
      link: 'https://zoom.com'

design:
  columns: '2'
---
