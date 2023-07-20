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

        **Advisor Bio:** Prof. Athman Bouguettaya is a distinguished academic in the field of computer science. He is Professor and former Head of School of Computer Science at The University of Sydney, NSW, Australia. He was previously Professor and Head of School of Computer Science and Information Technology at RMIT University, Melbourne, Australia and Science Leader in Service Computing at CSIRO ICT Centre, Canberra. Australia. His impressive accomplishments as a scholar and researcher have garnered him various prestigious awards and designations, such as IEEE Fellow, IEEE Computer Society Distinguished Scientist, ACM Distinguished Scientist, ACM Distinguished Speaker, and WISE Fellow. He is serving as the Vice-Chair of the 2023 IEEE Computer Society Fellow Evaluating Committee.
        
        **   ** 
        
        **   ** 
    design:
      columns: '1'
    
  - block: tag_cloud
    content:
      title: My title
      subtitle: My subtitle
      text: **Deep Learning** **Machine Learning** **Internet of Things** **Energy Services**
      # Choose a taxonomy from the `taxonomies` list in `config.yaml` to display (e.g. tags, categories, authors)
      taxonomy: tags
      # Choose how many tags you would like to display (0 = all tags)
      count: 4
    design:
      # Minimum and maximum font sizes (1.0 = 100%).
      font_size_min: 0.7
      font_size_max: 2.0
  
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
---
