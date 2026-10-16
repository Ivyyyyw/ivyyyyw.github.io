---
# Leave the homepage title empty to use the site title
title: ''
date: 2025-09-29
type: landing


design:
  # Default section spacing
  spacing: '1.5rem'

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
        - date: "Oct 2026"
          text: "I've completed my master's program and graduated from EPFL! Thank you for the wonderful years in Lausanne and for all the support I've received. I'll always cherish the meaningful conversations, celebrations, and time we shared along the way. 🎓🥳🎉✨"
        - date: "Aug 2026"
          text: "Our paper, *The Illusion of Efficacy: Diagnosing the Generative Side Effects of Knowledge Editing*, was accepted at the Grounding Language Models (GroundLM) Workshop at **EMNLP 2026**! Thank you to my co-authors for their support and collaboration! 🎉"
        - date: "Aug 2025"
          text: "Started my research internship at AXA Group Operations in Lausanne, Switzerland 🧀, supervised by Dr. Thibault Laugel. I later continued my research there for my master's thesis."
        - date: "Aug 2025"
          text: "My first-author paper *TactfulToM: Do LLMs Have the Theory of Mind Ability to Understand White Lies?* was accepted at **EMNLP 2025 (Main)** 🥳! I presented it in Suzhou in November 2025 — huge thanks to my co-authors 🙏"
        - date: "Oct 2024"
          text: "Started my six-month research assistant position at the National Institute of Informatics (Tokyo, Japan) 🌸, supervised by Prof. Saku Sugawara. Excited to work on evaluating the social reasoning ablities of LLMs."
    design:
      css_class: 'news-section'
      spacing:
        padding: ["1.25rem","0","1.25rem","0"]   # 上下留白
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
