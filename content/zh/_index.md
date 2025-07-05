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
      title: ''
      text: |-
              **大家好！👋 我是一名人工智能博士研究生，目前就读于电子科技大学，导师为[王国庆]教授(https://faculty.uestc.edu.cn/wangguoqing2/zh_CN/index.htm)。曾任东方希望集团算法工程师，并曾在悉尼大学担任科研助理。十分感谢[刘同亮](https://tongliang-liu.github.io/)教授与我的硕士导师[Athman Bouguettaya](https://www.sydney.edu.au/engineering/about/our-people/academic-staff/athman-bouguettaya.html)教授在我进入学术界一直以来的支持与指导。**
              
              **我的研究方向主要为时间序列与多模态。我热衷于接受一切有趣的研究合作与讨论。欢迎随时联系！**   
    design:
      columns: '1'

  - block: markdown
    content:
      title: ' '
      text: |-
        ### 📖 教育背景:
        - **2025年6月 - 至今, 人工智能博士研究生, 电子科技大学**
    
        - **2022年2月 - 2023年8月, 信息技术(研究途径)硕士, 悉尼大学(澳大利亚)**
    
        - **2016年9月 - 2020年6月, 电子信息科学与技术工学学士, 成都信息工程大学**

        ### 💼 工作经历:
        - **2024年3月 - 2025年6月, 算法工程师, 东方希望集团(中国)**
    
        - **2023年8月 - 2024年2月, 科研助理, SCSLab(澳大利亚)**

        ### 🔥 新闻:
        - **2023年7月, 于 ICWS 2023 (CCF-B) 担任分会场主持.**

        - **2023年5月, 一篇文章被 ICWS 2023 (CCF-B) 接收.**

        - **2023年3月, 一篇文章被 PerCom 2023 (CCF-B) 接收.**

        - **2022年12月, 一篇文章被 ICSOC 2022 (CCF-B) 接收.**

        ### 🏆 荣誉及获奖情况:
        - **2025年4月, 中国工业算法挑战赛全国14名**

        - **2023年8月, 高等研究学位支持基金, 悉尼大学**

        - **2023年2月, 高等研究学位支持基金, 悉尼大学**

        - **2019年5月, 大学生“科创杯”竞赛一等奖**

        ### 📝 发表文章:
        {{< spoiler text="**Energy Loss Prediction in IoT Energy Services**" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "[Energy Loss Prediction in IoT Energy Services](https://ieeexplore.ieee.org/document/10248251)." *2023 IEEE International Conference on Web Services (ICWS)*. IEEE, 2023.
        {{< /spoiler >}}
        {{< spoiler text="**Monitoring efficiency of iot wireless charging**" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "[Monitoring efficiency of iot wireless charging](https://ieeexplore.ieee.org/abstract/document/10150276)." *2023 IEEE International Conference on Pervasive Computing and Communications Workshops and other Affiliated Events (PerCom Workshops)*. IEEE, 2023.
        {{< /spoiler >}}
        {{< spoiler text="**Towards peer-to-peer sharing of wireless energy services**" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "[Towards peer-to-peer sharing of wireless energy services](https://link.springer.com/chapter/10.1007/978-3-031-26507-5_38)." *International Conference on Service-Oriented Computing*. Cham: Springer Nature Switzerland, 2022.
        {{< /spoiler >}}
        {{< spoiler text="**Establishment of Neural Networks Robust to Label Noise**" >}}
          Pengwei Yang, Chongyangzi Teng, and Jack George Mangos. "[Establishment of Neural Networks Robust to Label Noise](https://arxiv.org/abs/2211.15279v3)." *arXiv preprint arXiv:2211.15279* (2022).
        {{< /spoiler >}}
        {{< spoiler text="**Containminated Images Recovery by Implementing Non-negative Matrix Factorisation**" >}}
          Pengwei Yang, Chongyangzi Teng, and Jack George Mangos. "[Contaminated Images Recovery by Implementing Non-negative Matrix Factorisation](https://arxiv.org/abs/2211.04247v4)." *arXiv preprint arXiv:2211.04247* (2022).
        {{< /spoiler >}}
        {{< spoiler text="**Multimodal in Multi-Label Classification: A Report**" >}}
          Chongyangzi Teng, Pengwei Yang, and Mengshen Guo. "[Multimodal in Multi-Label Classification: A Report](https://www.researchgate.net/publication/371473901_Multimodal_in_Multi-Label_Classification_A_Report)."
        {{< /spoiler >}}
        {{< spoiler text="**Techniques in Deep Learning: A Report**" >}}
          Chongyangzi Teng, Pengwei Yang, and Mengshen Guo. "[Techniques in Deep Learning: A Report.](https://www.researchgate.net/publication/370277982_Techniques_in_Deep_Learning_A_Report)"
        {{< /spoiler >}}
    
        ### 🗂️ 项目展示 (YouTube):
        - **Monitoring Efficiency of IoT Wireless Charging**
        {{< youtube 8cYG6jscivE >}}

        - **Towards Peer-to-Peer Sharing of Wireless Energy Services**
        {{< youtube d-bdFGk6z4A >}}

        - **Energy Loss Prediction in IoT Energy Services**
        {{< youtube arKnVtVJmpo >}}
    
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

  
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |-

        <script src="https://cdn.commoninja.com/sdk/latest/commonninja.js" defer></script>
        <div class="commonninja_component pid-12c0f14f-4e06-400d-b55d-f755bdd5351b"></div>
           
    design:
      columns: '1'
  
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |-
        <script type="text/javascript" id="clstr_globe" src="//clustrmaps.com/globe.js?d=IPz9CHURQbIcxY1LcH-h8QSuFwl3DVHDYvYkveXsHqc"></script> 
    design:
      columns: '1'
---
