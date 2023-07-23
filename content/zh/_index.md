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
        杨朋卫是悉尼大学计算机科学学院Athman Bouguettaya教授指导下的研究型硕士生，拥有深厚的计算机科学与电子信息科学交叉学科背景。作为悉尼大学传感器、云和服务实验室的研究员，杨朋卫的学术追求是探索计算机科学的各个层面，包括众包、服务计算、深度学习和可信机器学习。
        
        杨朋卫对学术研究的投入体现在他对该领域的贡献上。他在面向服务计算国际会议(ICSOC，CCF-B)上成功发表了一篇演示论文，在IEEE普适计算和通信国际会议(PerCom，CCF-B)上发表了另一篇演示论文。此外，杨朋卫有一篇被IEEE国际万维网服务大会(ICWS，CCF-B)全文接收的研究长文。目前，他正计划扩大他的研究，并向服务计算领域的著名期刊IEEE Transactions on Services Computing（TSC，中科院JCR一区）提交扩展版本。杨朋卫的学术历程反映了他对计算机科学的热情和对在其领域产生影响的执着。
        
        **研究兴趣：** 面向服务计算，物联网，自然语言处理，深度学习，可信机器学习

        **导师简介：** Athman Bouguettaya教授是计算机科学领域的一位杰出科学家, 于2022年被评为服务计算与物联网领域全球前2%的顶尖学者。他是澳大利亚新南威尔士州悉尼大学的教授和计算机科学学院的前院长。作为一名学者，他取得了极其卓越的成就，如IEEE院士、IEEE计算机协会杰出科学家、ACM杰出科学家、ACM杰出发言人以及WISE院士。他在2023年被任命为IEEE计算机协会院士评估委员会副主席。     
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
        {{< spoiler text="📄 [**Energy Loss Prediction in IoT Energy Services**](https://arxiv.org/abs/2305.10238)" >}}
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
    
        ### 项目展示:
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
        <script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=IPz9CHURQbIcxY1LcH-h8QSuFwl3DVHDYvYkveXsHqc&cl=ffffff&w=a"></script>      
    design:
      columns: '1'
---
