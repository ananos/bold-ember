---
title: urunc - The unikernel container runtime

summary: urunc aspires to be runc for unikernels
abstract: 'The main goal of urunc is to bridge the gap between traditional unikernels and containerized environments, enabling seamless integration with cloud-native architectures. Designed to fully leverage the container semantics and benefits from the OCI tools and methodology, urunc aims to become “runc for unikernels”, while offering compatibility with the Container Runtime Interface (CRI). Unikernels are packaged inside OCI-compatible images and urunc launches the unikernel on top of the underlying Virtual Machine or seccomp monitors. Thus, developers and administrators can package, deliver, deploy and manage unikernels using familiar cloud-native practises.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2030-06-01T13:00:00Z'
date_end: '2030-06-01T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2017-01-01T00:00:00Z'

authors: ["ananos","cmainas"]
tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
  focal_point: Right

url_code: 'https://github.com/urunc-dev/urunc'
url_pdf: ''
url_slides: ''
url_video: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides:

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ['urunc']
---
