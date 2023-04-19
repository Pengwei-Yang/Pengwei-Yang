---
title: Service-oriented Computing Research Project
summary: Energy Loss Estimation in IoT Services
tags:
- Demo
date: "2023-04-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
Project_link: (https://www.researchgate.net/profile/Pengwei-Yang/research)

image:
  caption: Photo by Pengwei Yang
  focal_point: Smart
  
# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---
## Orientation
Battery limitation, as a significant deficiency, obstacles the development of IoT devices. Crowdsourcing energy service (CES) was thus proposed to give a novel solution to the aforementioned problem [1]. However, to the best of our knowledge, although recent studies have made substantial progress based on simulation analysis of the proposed techniques using synthetic datasets [2][3][4][5], there is hardly existing research utilizing real-world data. [6] is an exception, proposing a CES energy sharing platform, despite the fact that its feasibility has only been demonstrated through back-to-back reverse charging. Besides, as mentioned in [1], mobility is one challenge that CES facing presently. To address the problem of mobility, over a distance wireless power transfer (WTP) technique is required. Thus, there is a call for establishing a real-world CES platform that allows energy transfer over a distance. That’s our first research question: How can we extend the existing CES platform to realize energy sharing over a distance?

Furthermore, as indicated in [2], energy loss estimation is one important research direction in the field of CES. We transformed the research question of energy loss to energy consumption based on logical deduction. Actually, there is a set of research focused on the energy consumption field. Most of them focused on identifying the energy-hungry modules on the IoT devices while there are some researchers start studying to predict energy consumption using machine learning algorithms [7][8]. As a result, we plan to study our second research question: how can we build machine learning models to analyze the wireless energy transmission loss given data on energy consumption of IoT devices?

## Background
As for the field of CES, the majority of research focuses on coming up with algorithms to allocate a fair, attracting crowdsourcing energy service as well as build a self-sustained CES ecosystem. In terms of the existing literature, [2] proposed a self-sustainable model that leverages energy harvesting, wireless power transfer, and crowdsourcing. [3], [4], [5] respectively delivered ideas of solving energy fluctuation problem, permitting the partial consumption and re-invocation of intermittent services, and leveraging user spatio-temporal preferences. In addition, a concept of reward was proposed in [9] to motivate the participation of provider. A further methodology was then put forward to consider both aspects of provider and consumer [6]. Besides, [10] shows an idea of building energy sharing platform. Nevertheless, researchers only experimented on back-to-back reverse charging instead of distance-based wireless energy sharing.

With regard to the field of WPT, current research can be classified into two categories: near-field charging and far-field charging [11]. Near-field wireless power transfer techniques are widely utilized in IoT devices because of their ensured safety [11]. Simultaneously, the feasibility of far-field wireless power transfer technique has been demonstrated in [12].

In terms of IoT device energy consumption, according to a review [7], traditional research methodologies can be categorized into hardware-based and software-based profiling. Apart from that, there are researchers who profile user patterns based on energy consumption [13][14]. Several researchers start research on estimating energy consumption using machine learning algorithms [7][8]. Furthermore, [8] demonstrated the better performance of time-series machine learning model (e.g., LSTM) than traditional models such as MLP. Therefore, we plan to focus on building time-series models.

## Gap

- There is no CES energy sharing platform that allows users sharing energy over a distance
- There is no research focus on predicting energy loss derived from energy charging in the field of CES

## Objective

- Extend an existing CES energy sharing platform to enable power transfer over a distance
- Utilize machine learning algorithms to predict the energy loss derived from the wireless power transfer process

## Methodology

Our first objective is to establish a CES platform that enables energy transfer over a distance. As introduced in Section 2, we plan to use near-field wireless power transfer technique. To give a high-level explanation, it is basically an energy transfer process between two coils. Hence, we plan to do experiments using different types of coils to maximize the mobility of the platform.

Our final objective is to build machine learning models to predict energy loss. However, it’s hard to directly detect the loss. Hence, we come up with a logical deduction to transform this question into research energy consumption. The methodology we take is shown in the above Figure.

To the best of our knowledge, the total energy loss contains actual energy loss and energy self-consumptions of both provider and consumer. Considering the difficulty of detecting currency simultaneously, we plan to asynchronously collect data in two states, i.e., charging and not charging status. As shown in the Figure, we can respectively get the data of provider transfer, consumer gain, provider usage, and consumer usage. The loss energy of the provider in charging state includes the power of provider usage and real transfer. Besides, real receive energy by consumer contains both consumer gain and consumer self-consumption. Thus, the total loss can be calculated using real transfer deducting real received energy. 

Basically, we can get the loss by using data collected from energy consumption. In terms of the data we collected, they are time-series data. As mentioned in Section 2, we plan to focus on building time-series models (e.g., RNNs) for estimating energy consumption. Additionally, for the feature selection process, battery level is our first focus. We might add other variables such as battery temperature, CPU usage, etc. to enhance the accuracy of our model.

As for our evaluation metric, we plan to use the method that shown in below Equation, where Y denotes the energy observations per time window of the time series and Y hat denotes the energy predictions for each time step in a series.

- $f(\hat{Y},Y) = |\frac{\sum{ \hat{y}} - \sum{y}}{\sum{y}}|$

To sum up, our contributions can be seen as follows:
- Build a CES platform that enables energy transfer over a distance.
- The platform can automatically show the info on energy loss that might derive from the crowdsourcing energy service process.

### Reference

[1] *Amani Abusafia and Athman Bouguettaya. Reliability model for incentive-driven iot energy
services. In MobiQuitous 2020-17th EAI International Conference on Mobile and Ubiquitous
Systems: Computing, Networking and Services, pages 196–205, 2020.*

[2] *Amani Abusafia, Athman Bouguettaya, and Sajib Mistry. Incentive-based selection and com-
position of iot energy services. In 2020 IEEE International Conference on Services Computing
(SCC), pages 304–311, 2020.*

[3] *Raja Wasim Ahmad, Abdullah Gani, Siti Hafizah Ab. Hamid, Feng Xia, and Muhammad
Shiraz. A review on mobile application energy profiling: Taxonomy, state-of-the-art, and
open research issues. Journal of Network and Computer Applications, 58:42–59, 2015.*

[4] *Hossein Falaki, Ratul Mahajan, Srikanth Kandula, Dimitrios Lymberopoulos, Ramesh Govin-
dan, and Deborah Estrin. Diversity in smartphone usage. In Proceedings of the 8th Interna-
tional Conference on Mobile Systems, Applications, and Services, page 179–194. Association
for Computing Machinery, 2010.*

[5] *Abdallah Lakhdari, Amani Abusafia, and Athman Bouguettaya. Crowdsharing wireless energy
services. In CIC, pages 18–24. IEEE, 2020.*

[6] *Abdallah Lakhdari and Athman Bouguettaya. Fluid composition of intermittent iot energy
services. In 2020 IEEE International Conference on Services Computing (SCC), pages 329–
336. IEEE, 2020.*


[7] *Abdallah Lakhdari and Athman Bouguettaya. Fairness-aware crowdsourcing of iot energy
services. In ICSOC, pages 351–367. Springer, 2021.*

[8] *Abdallah Lakhdari and Athman Bouguettaya. Proactive composition of mobile iot energy
services. In 2021 IEEE International Conference on Web Services (ICWS), pages 192–197.
IEEE, 2021.*

[9] *Abdallah Lakhdari, Athman Bouguettaya, Sajib Mistry, Azadeh Ghari Ghari Neiat, and
Basem Suleiman. Elastic composition of crowdsourced iot energy services. In MobiQuitous
2020-17th EAI International Conference on Mobile and Ubiquitous Systems: Computing, Net-
working and Services, pages 308–317, 2020.*

[10] *Abdallah Lakhdari, Athman Bouguettaya, and Azadeh Ghari Neiat. Crowdsourcing energy as
a service. In Service-Oriented Computing, pages 342–351. Springer International Publishing,
2018.*

[11] *Xiao Lu, Ping Wang, Dusit Niyato, Dong In Kim, and Zhu Han. Wireless charging technolo-
gies: Fundamentals, standards, and network applications. IEEE Communications Surveys
Tutorials, 18(2):1413–1452, 2016.*

[12] *Antônio Sá Barreto Neto, Felipe Farias, Marco Aurélio Tomaz Mialaret, Bruno Cartaxo, Prís-
cila Alves Lima, and Paulo Maciel. Building energy consumption models based on smartphone
user’s usage patterns. Knowledge-Based Systems, 213:106680, 2021.*

[13] *Stephen Romansky, Neil C. Borle, Shaiful Chowdhury, Abram Hindle, and Russ Greiner. Deep
green: Modelling time-series of software energy consumption. In 2017 IEEE International
Conference on Software Maintenance and Evolution (ICSME), pages 273–283, 2017.*

[14] *Vu H Tran, Archan Misra, Jie Xiong, and Rajesh Krishna Balan. Wiwear: Wearable sensing
via directional wifi energy harvesting. In PerCom, pages 1–10. IEEE, 2019.*

[15] *Jessica Yao and et al. Wireless iot energy sharing platform. In PerCom Workshops, pages
118–120. IEEE, 2022*
