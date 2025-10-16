---
title: Contact
date: 2022-10-24

type: landing

sections:
  - block: contact
    content:
      title: Contact
      text: |-
        We’re always happy to hear from you. Whether you have questions about our projects, collaboration opportunities, or services, our teams are ready to assist.

        With presence in multiple locations, we strive to provide timely responses and connect you with the right person for your needs. Use the interactive map below to find detailed contact information, including phone numbers, email addresses, and hours you can reach us.

        We look forward to connecting with you and supporting your inquiries — your message is important to us.
      locations:
      - name: "Sheffield"
        email: info@nubificus.co.uk
        phone: +44 7428318494
        address:
          street: Office 159, Queen st 88
          city: Sheffield
          region: South Yorkshire
          postcode: 'S10 3FW'
          country: United Kingdom
          country_code: UK
        coordinates:
          latitude: '53.38466'
          longitude: '-1.46996'
        directions: 
        office_hours:
          - 'Monday to Friday 10:00 to 18:00'
        appointment_url: 'https://calendly.com'
        #contact_links:
        #  - icon: comments
        #    icon_pack: fas
        #    name: Discuss on Forum
        #    link: 'https://discourse.gohugo.io'

        # Automatically link email and phone or display as text?
        autolink: true
      - name: "Halkida"
        email: info@nubis-pc.eu
        phone: +30 2221 181522
        address:
          street: Tynnichou 4
          city: Halkida
          region: Evia
          postcode: '34133'
          country: Greece
          country_code: GR
        coordinates:
          latitude: '38.46075'
          longitude: '23.59060'
        directions: Enter through the green door, take the stairs to the first floor
        office_hours:
          - 'Monday to Friday 10:00 to 18:00'
        appointment_url: 'https://calendly.com'
        #contact_links:
        #  - icon: comments
        #    icon_pack: fas
        #    name: Discuss on Forum
        #    link: 'https://discourse.gohugo.io'

        # Automatically link email and phone or display as text?
        autolink: true
      - name: "Athens"
        email: info@nubis-pc.eu
        phone: +30 210 6726412
        address:
          street: Chalandri Office
          city: Chalandri
          region: Attiki
          postcode: '15231'
          country: Greece
          country_code: GR
        coordinates:
          latitude: '38.01185'
          longitude: '23.78997'
        directions: #Enter through the green door, take the stairs to the first floor
        office_hours:
          - 'Monday to Friday 10:00 to 18:00'
        appointment_url: 'https://calendly.com'
        #contact_links:
        #  - icon: comments
        #    icon_pack: fas
        #    name: Discuss on Forum
        #    link: 'https://discourse.gohugo.io'
    
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
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: contact.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen
---
