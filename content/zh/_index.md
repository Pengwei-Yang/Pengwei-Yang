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
        杨朋卫是悉尼大学计算机科学学院Athman Bouguettaya教授指导下的研究型硕士生，拥有深厚的电子信息科学与技术背景。作为悉尼大学传感器、云和服务实验室的研究员，杨朋卫的学术追求是探索计算机科学的各个层面，包括众包、服务计算、深度学习和可信机器学习。
        
        杨朋卫对学术研究的投入体现在他对该领域的贡献上。他在面向服务计算国际会议(ICSOC，CCF-B)上成功发表了一篇演示论文，在IEEE普适计算和通信国际会议(PerCom，CCF-B)上发表了另一篇演示论文。此外，杨朋卫还向IEEE国际网络服务会议(ICWS，CCF-B)提交了一篇研究长文。目前，他正计划扩大他的研究，并向服务计算领域的著名期刊IEEE Transactions on Services Computing（TSC，中科院JCR一区）提交扩展版本。杨朋卫的学术历程反映了他对计算机科学的热情和对在其领域产生影响的执着。
        
        **研究兴趣：** 面向服务计算，物联网，自然语言处理，深度学习，可信机器学习

        **导师简介：** Athman Bouguettaya教授是计算机科学领域的一位杰出科学家, 在2022年被评为服务计算与物联网领域全球前2%的顶尖学者。他是澳大利亚新南威尔士州悉尼大学的教授和计算机科学学院的前院长。他是澳大利亚服务科学协会的创始成员和前任主席。他曾任澳大利亚皇家墨尔本大学计算机科学与信息技术学院的教授和院长，以及澳大利亚联邦科学与工业研究组织服务计算领域的科学领袖。作为一名学者，他取得了极其卓越的成就，如IEEE院士、ACM杰出科学家、IEEE计算机协会杰出科学家、ACM杰出发言人以及WISE院士。他在2023年被任命为IEEE计算机协会院士评估委员会副主席。     
                
        **   ** 
        
        **   ** 

    design:
      columns: '1'
  - block: collection
    content:
      title: 头条新闻
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
