---
# Leave the homepage title empty to use the site title
title: ''
date: 2025-09-29
type: landing


design:
  # Default section spacing
  spacing: '3rem'

sections:
  - block: resume-biography-custom
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      headings:
        about: '  '
        about_icon: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: 'bio-section'
      icon: ''
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: news-custom
    id: news
    content:
      title: News
      items:
        - date: "Aug 2025"
          text: "Started my six-month internship at AXA Group Operations in Lausanne, Switzerland 🧀, supervised by Dr. Thibault Laugel. Working on research topics related to the interpretability of large language models — an exciting journey ahead! 🚀"
        - date: "Aug 2025"
          text: "My first-author paper *TactfulToM: Do LLMs Have the Theory of Mind Ability to Understand White Lies?* was accepted at **EMNLP 2025 (Main)** 🥳! I'll be presenting it in Suzhou this November — huge thanks to my amazing co-authors 🙏"
        - date: "Oct 2024"
          text: "Started my six-month research assistant position at the National Institute of Informatics (Tokyo, Japan) 🌸, supervised by Prof. Saku Sugawara. Excited to work on evaluating the social reasoning ablities of LLMs."
    design:
      css_class: 'news-section'
      spacing:
        padding: ["1.3rem","0","1.rem","0"]   # 上下留白
      container: max-w-6xl                        # 和 Bio 更接近的宽度

  - block: publications-custom
    id: publications
    content:
      title: Publications
    design:
      css_class: 'publications-section'
      spacing:
        padding: ["1.3rem","0","1.3rem","0"]
      container: max-w-6xl

  - block: experience-custom
    id: experience
    content:
      title: Experience
      username: admin
    design:
      css_class: 'experience-section'
      spacing:
        padding: ["1.3rem","0","1.3rem","0"]
      container: max-w-6xl
---