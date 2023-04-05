---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: 
    design:
      background:
        color: black
        text_color_light: true
        image:
          # Add your image background to `assets/media/`.
          filename: li-yang-5h_dMuX_7RE-unsplash.webp
          filters:
            brightness: 0.5
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '学术简历'
      text: |-
        杨朋卫是悉尼大学计算机科学学院Athman Bouguettaya教授指导下的研究型硕士生，拥有深厚的电子信息科学和技术背景。作为悉尼大学传感器、云和服务实验室的研究员，杨朋卫的工作是探索计算机科学的各个层面，包括众包、服务计算、深度学习和可信的机器学习。
        
        杨朋卫对研究的投入体现在他对该领域的贡献上。他在面向服务计算国际会议（ICSOC，CCF-B）上成功发表了一篇演示论文，在IEEE普适计算和通信国际会议（PerCom，CCF-B）上发表了另一篇演示论文。此外，彭伟还向IEEE国际网络服务会议（ICWS，CCF-B）提交了一篇研究长文。目前，他正计划扩大他的研究，并向服务计算领域的著名期刊IEEE Transactions on Services Computing（TSC，中科院JCR一区）提交扩展版本。杨朋卫的学术历程反映了他对计算机科学的热情和对在其领域产生影响的执着。
        
        **研究兴趣：** 面向服务计算，物联网，自然语言处理，深度学习，可信机器学习

        **导师简介：** Athman Bouguettaya教授是计算机科学领域的一位杰出科学家。他是澳大利亚新南威尔士州悉尼大学的教授和计算机科学学院的前院长。他曾任澳大利亚墨尔本RMIT大学计算机科学和信息技术学院的教授和院长，以及澳大利亚堪培拉CSIRO ICT中心的服务计算科学负责人。作为一名学者，他取得了令人印象深刻的成就，如IEEE院士、ACM杰出科学家、IEEE计算机协会杰出访问者、ACM杰出发言人和WISE院士。     
        

    design:
      columns: '1'
  - block: collection
    content:
      title: 新闻头条
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
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
      columns: '1'
---
