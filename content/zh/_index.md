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
              大家好！我是一名博士研究生，目前就读于 [电子科技大学](https://en.uestc.edu.cn/)。 之前在 [东方希望集团](http://www.easthope.cn/)担任算法工程师。研究方向为时间序列和多模态。
              
              我热衷于接受一切有趣的研究合作与讨论。欢迎随时联系我！   
    design:
      columns: '1'

  - block: markdown
    content:
      title: ' '
      text: |-
        ### 教育背景:
        - **信息技术硕士 (研究型)**
          - 🏛 [**悉尼大学 (澳大利亚)**](https://www.sydney.edu.au/)
        - **电子工程学士**
          - 🏛 [**成都信息工程大学 (中国)**](https://open.ieee.org/partners/chengdu-university-of-information-technology/)

        ### 发表文章:
         {{< spoiler text="📄 [**Towards peer-to-peer sharing of wireless energy services**](https://link.springer.com/chapter/10.1007/978-3-031-26507-5_38)" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "Towards peer-to-peer sharing of wireless energy services." *International Conference on Service-Oriented Computing*. Cham: Springer Nature Switzerland, 2022.
        {{< /spoiler >}}
        {{< spoiler text="📄 [**Monitoring efficiency of iot wireless charging**](https://ieeexplore.ieee.org/abstract/document/10150276)" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "Monitoring efficiency of iot wireless charging." *2023 IEEE International Conference on Pervasive Computing and Communications Workshops and other Affiliated Events (PerCom Workshops)*. IEEE, 2023.
        {{< /spoiler >}}
        {{< spoiler text="📄 [**Energy Loss Prediction in IoT Energy Services**](https://ieeexplore.ieee.org/document/10248251)" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "Energy Loss Prediction in IoT Energy Services." *2023 IEEE International Conference on Web Services (ICWS)*. IEEE, 2023.
        {{< /spoiler >}}
        {{< spoiler text="📄 [**Establishment of Neural Networks Robust to Label Noise**](https://arxiv.org/abs/2211.15279v3)" >}}
          Pengwei Yang, Chongyangzi Teng, and Jack George Mangos. "Establishment of Neural Networks Robust to Label Noise." *arXiv preprint arXiv:2211.15279* (2022).
        {{< /spoiler >}}
        {{< spoiler text="📄 [**Containminated Images Recovery by Implementing Non-negative Matrix Factorisation**](https://arxiv.org/abs/2211.04247v4)" >}}
          Pengwei Yang, Chongyangzi Teng, and Jack George Mangos. "Containminated Images Recovery by Implementing Non-negative Matrix Factorisation." *arXiv preprint arXiv:2211.04247* (2022).
        {{< /spoiler >}}
        {{< spoiler text="📄 [**Multimodal in Multi-Label Classification: A Report**](https://www.researchgate.net/publication/371473901_Multimodal_in_Multi-Label_Classification_A_Report)" >}}
          Chongyangzi Teng, Pengwei Yang, and Mengshen Guo. "Multimodal in Multi-Label Classification: A Report."
        {{< /spoiler >}}
        {{< spoiler text="📄 [**Techniques in Deep Learning: A Report**](https://www.researchgate.net/publication/370277982_Techniques_in_Deep_Learning_A_Report)" >}}
          Chongyangzi Teng, Pengwei Yang, and Mengshen Guo. "Techniques in Deep Learning: A Report."
        {{< /spoiler >}}
    
        ### 项目展示 (from YouTube):
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
      title: '致谢'
      subtitle: ''
      text: |-
        感谢**传感、云计算与服务实验室**、**澳大利亚研究理事会**、**IEEE计算机学会**和**联邦科学与工业研究组织**对物联网能源服务相关研究的支持。本文最终解释权归作者所有。

        <script src="https://cdn.commoninja.com/sdk/latest/commonninja.js" defer></script>
        <div class="commonninja_component pid-12c0f14f-4e06-400d-b55d-f755bdd5351b"></div>
           
    design:
      columns: '1'
  - block: tag_cloud
    content:
      title: 
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
