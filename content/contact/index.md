---
title: Contact
date: 2025-10-24

type: landing

sections:
  - block: contact
    content:
      title: Contact
      text: |-
       欢迎就科研合作、招生与项目洽谈联系我。邮件一般在 24–48 小时内回复。
      email: songsensen@xju.edu.cn
      address:
        street: 新疆大学博达校区未来技术学院313
        city: 乌鲁木齐
        region: 新疆省
        country: 中国
        country_code: CN
      coordinates:
        latitude: '43.840699290825754'
        longitude: '87.74201'
      directions: 校门进入后直行 200 米，右转至未来技术学院楼 3 层 313 室
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
