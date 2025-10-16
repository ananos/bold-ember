---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        Nubificus
      image:
        filename: welcome.jpg
      text: |
        <br>

        **Nubificus** is a specialized research group focused on tackling complex virtualization and cloud-edge computing challenges. The team regularly collaborates with leading academic institutions and R&D organizations on European projects, driving innovation in hardware acceleration, serverless frameworks, and resource orchestration for next-generation distributed infrastructures.
  - block: portfolio
    content:
      title: |
        Virtualization Research
      image:
        filename: welcome.jpg
      text: |
        <br>

        Our team brings state-of-the-art research to commercial projects
      filters:
        author: ''
        category: ''
        tag: ''
      offset: 0
      order: desc
      page_type: projects
      design:
        view: compact

  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 3
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: 'news'
      offset: 0
      #order: desc
      page_type: post
    design:
      view: card
      columns: '4'
  

  - block: collection
    content:
      title: Latest Publications
      text: ""
      count: 5
      filters:
        folders:
          - publication
        #publication_type: 'article'
    design:
      view: citation
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
          filename: coders.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen

#
#  - block: markdown
#    content:
#      title:
#      subtitle:
#      text: |
#        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
#    design:
#      columns: '1'
---
