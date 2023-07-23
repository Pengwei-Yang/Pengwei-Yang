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
      title: 'Introduction'
      subtitle: 'Academic Bio'
      text: |-
        Pengwei Yang is a Research Master Student under the supervision of Prof. Athman Bouguettaya in the School of Computer Science at the University of Sydney, with a strong interdisciplinary background in Computer Science and Electronic Information Science. As a researcher in the Sensors, Clouds, and Services Lab at the University of Sydney, Pengwei's work explores various facets of computer science, including Crowdsourcing, Service Computing, Deep Learning, and Trustworthy Machine Learning. 
        
        Pengwei Yang's commitment to research has been evident in his contributions to the field. He has successfully published a demo paper at the International Conference on Service-Oriented Computing (ICSOC, Core A) and another demo paper at the IEEE International Conference on Pervasive Computing and Communications (PerCom, Core A*). Furthermore, Pengwei has a full research paper accepted by the IEEE International Conference on Web Services (ICWS, Core A), which is a significant achievement in his field of research. He is currently planning to expand upon his research and submit an extended version to the IEEE Transactions on Services Computing (TSC), a prestigious journal in the area of service computing. Pengwei Yang's academic journey reflects his passion for computer science and a dedication to making an impact in his field.
        
        **Research Interests:** Service-oriented Computing, IoT, Natural Language Processing, Deep Learning, Trustworthy Machine Learning

        **Advisor Bio:** Prof. Athman Bouguettaya is a distinguished academic in the field of computer science. He is Professor and former Head of School of Computer Science at The University of Sydney, NSW, Australia. His impressive accomplishments as a scholar and researcher have garnered him various prestigious awards and designations, such as IEEE Fellow, IEEE Computer Society Distinguished Scientist, ACM Distinguished Scientist, ACM Distinguished Speaker, and WISE Fellow. He is serving as the Vice-Chair of the 2023 IEEE Computer Society Fellow Evaluating Committee.
        
    design:
      columns: '1'
  - block: markdown
    content:
      title: ' '
      text: |-
    
        **Education:**
        - **MA in Information Technology (Research Pathway)**
          - 🏛 [**The University of Sydney (Australia)**](https://www.sydney.edu.au/)
        - **BA in Engineering**
          - 🏛 [**Chengdu University of Information Technology (China)**](https://open.ieee.org/partners/chengdu-university-of-information-technology/)

        **Publication:**
        {{< spoiler text="📄 [Towards peer-to-peer sharing of wireless energy services](https://link.springer.com/chapter/10.1007/978-3-031-26507-5_38)" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "Towards peer-to-peer sharing of wireless energy services." *International Conference on Service-Oriented Computing*. Cham: Springer Nature Switzerland, 2022.
        {{< /spoiler >}}
        {{< spoiler text="📄 [Monitoring efficiency of iot wireless charging](https://ieeexplore.ieee.org/abstract/document/10150276)" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "Monitoring efficiency of iot wireless charging." *2023 IEEE International Conference on Pervasive Computing and Communications Workshops and other Affiliated Events (PerCom Workshops)*. IEEE, 2023.
        {{< /spoiler >}}
        {{< spoiler text="📄 [Energy Loss Prediction in IoT Energy Services](https://arxiv.org/abs/2305.10238)" >}}
          Pengwei Yang, Amani Abusafia, Abdallah Lakhdari, and Athman Bouguettaya. "Energy Loss Prediction in IoT Energy Services." *2023 IEEE International Conference on Web Services (ICWS)*. IEEE, 2023.
        {{< /spoiler >}}
        {{< spoiler text="📄 [Establishment of Neural Networks Robust to Label Noise](https://arxiv.org/abs/2211.15279v3)" >}}
          Pengwei Yang, Chongyangzi Teng, and Jack George Mangos. "Establishment of Neural Networks Robust to Label Noise." *arXiv preprint arXiv:2211.15279* (2022).
        {{< /spoiler >}}
        {{< spoiler text="📄 [Containminated Images Recovery by Implementing Non-negative Matrix Factorisation](https://arxiv.org/abs/2211.04247v4)" >}}
          Pengwei Yang, Chongyangzi Teng, and Jack George Mangos. "Containminated Images Recovery by Implementing Non-negative Matrix Factorisation." *arXiv preprint arXiv:2211.04247* (2022).
        {{< /spoiler >}}
        {{< spoiler text="📄 [Multimodal in Multi-Label Classification: A Report](https://www.researchgate.net/publication/371473901_Multimodal_in_Multi-Label_Classification_A_Report)" >}}
          Chongyangzi Teng, Pengwei Yang, and Mengshen Guo. "Multimodal in Multi-Label Classification: A Report."
        {{< /spoiler >}}
        {{< spoiler text="📄 [Techniques in Deep Learning: A Report](https://www.researchgate.net/publication/370277982_Techniques_in_Deep_Learning_A_Report)" >}}
          Chongyangzi Teng, Pengwei Yang, and Mengshen Guo. "Techniques in Deep Learning: A Report."
        {{< /spoiler >}}

        **Project:**
        - **Monitoring Efficiency of IoT Wireless Charging**
        {{< youtube 8cYG6jscivE >}}

        - **Towards Peer-to-Peer Sharing of Wireless Energy Services**
        {{< youtube d-bdFGk6z4A >}}

        **   **

        
        **   ** 
    design:
      columns: '1'
  
  - block: collection
    content:
      title: Top News
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
      title: 'Acknowledgements'
      subtitle: ''
      text: |-
        Greatly appreciate the support from **Sensors, Clouds, and Services Lab**, **Australian Research Council**, **IEEE Computer Society**, and **Commonwealth Scientific and Industrial Research Organisation**. The statements made herein are solely the responsibility of the author.       
    design:
      columns: '1'
  - block: tag_cloud
    content:
      title: 
    design:
      columns: '1'

---
