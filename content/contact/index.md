---
title: Contact
date: 2025-10-24

type: landing

sections:
  - block: contact
    content:
      title: Contact VIVID Lab
      text: |-
        欢迎就科研合作、招生与项目洽谈联系 VIVID Lab（Volumetric Intelligence, Visual Imaging & Data）。邮件一般在 24–48 小时内回复。
      email: songsensen@xju.edu.cn
      address:
        street: 新疆大学博达校区未来技术学院 313
        city: 乌鲁木齐
        region: 新疆
        country: 中国
        country_code: CN
      coordinates:
        latitude: '43.840699290825754'
        longitude: '87.74201'
      directions: 从校门进入后直行约 200 米，右转至未来技术学院楼 3 层 313 室。
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # Email form provider
      form:
        # provider: netlify
        provider:
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '1'
      background:
        gradient_start: '#f8f2e8'
        gradient_end: '#dfe9f3'
        gradient_angle: 120
        text_color_light: false
      spacing:
        padding: ['120px', '0', '120px', '0']
      css_class: contact-hero

  - block: markdown
    content:
      title:
      subtitle: ''
      text: |
        <div class="contact-banner-inner">
          <div class="contact-banner-eyebrow">Visit Our Campus</div>
          <div class="contact-banner-title">新疆大学博达校区 · 未来技术学院</div>
        </div>
    design:
      columns: '1'
      background:
        image:
          filename: xjdx.png
          filters:
            brightness: 0.65
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['180px', '0', '180px', '0']
      css_class: contact-banner
---
