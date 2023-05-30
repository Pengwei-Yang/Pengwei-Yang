---
title: 物联网能源服务中的能量损失预测
summary: 面向服务计算研究项目
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
## 研究方向
电池限制作为一个重要的缺陷，阻碍了物联网设备的发展。因此，众包能源服务(CES)被提出作为解决上述问题的新方法[1]。然而，据我们所知，尽管最近的研究基于使用合成数据集的模拟分析取得了实质性进展[2][3][4][5]，但几乎没有现有研究利用真实世界的数据。[6]是一个例外，提出了一个CES能量共享平台，尽管其可行性仅通过背靠背反向充电得到了证明。此外，正如[1]所提到的，移动性是CES目前面临的一个挑战。为了解决移动性问题，需要一种距离无线能量传输(WTP)技术。因此，有一个呼吁建立一个实际的CES平台，允许距离能量传输。这是我们的第一个研究问题：我们如何扩展现有的CES平台，实现距离上的能量共享？

此外，正如[2]所示，能量损失估计是CES领域的一个重要研究方向。我们基于逻辑推断将能量损失的研究问题转化为基于能量消耗的问题。实际上，有一系列关注能量消耗领域的研究。它们大多集中于识别IoT设备上的耗能模块，而有些研究者开始研究使用机器学习算法来预测能耗[7][8]。因此，我们计划研究第二个研究问题：如何构建机器学习模型，分析给定IoT设备能量消耗数据的无线能量传输损失？

## 研究背景
在CES领域，大部分研究集中在开发算法来分配公平、吸引人的众包能源服务，以及建立一个自我可持续的CES生态系统。在现有的文献中，[2]提出了一种利用能量收集、无线能量传输和众包的自我可持续模型。[3]、[4]、[5]分别提出了解决能量波动问题、允许部分消耗和间歇性服务的再调用以及利用用户时空偏好的想法。此外，[9]提出了一种奖励的概念，以激励服务提供者的参与。接着，[6]提出了一种更进一步的方法，考虑到服务提供者和消费者两个方面。此外，[10]展示了建立能源共享平台的想法。然而，研究人员只进行了背靠背反向充电的实验，而不是基于距离的无线能量共享。

在WPT领域，目前的研究可以分为近场充电和远场充电两类[11]。由于其保证安全性，近场无线能量传输技术广泛应用于IoT设备[11]。同时，[12]展示了远场无线能量传输技术的可行性。

关于IoT设备的能量消耗，根据一项综述[7]，传统的研究方法可以分为基于硬件和基于软件的分析。除此之外，还有研究人员基于能耗来分析用户模式[13][14]。一些研究人员开始使用机器学习算法来估计能耗[7][8]。此外，[8]展示了时间序列机器学习模型（例如LSTM）相比于传统模型如MLP的更好性能。因此，我们计划集中于构建时间序列模型。

## 研究动机

- 目前没有一种众包能源服务能量共享平台可以允许用户通过距离共享能源。
- 在CES领域中，目前没有研究集中于预测能量充电带来的能量损失问题。

## 研究目标

- 要扩展现有的CES能源共享平台，以实现跨距离能量传输。
- 利用机器学习算法预测无线能量传输过程中带来的能量损失

## 研究方法

我们的第一个目标是建立一个能够实现距离能量传输的CES平台。如第2节所介绍的，我们计划使用近场无线能量传输技术。简单来说，这是两个线圈之间的能量传输过程。因此，我们计划使用不同类型的线圈进行实验，以最大化平台的移动性。

我们的最终目标是构建机器学习模型来预测能量损失。然而，直接检测损失是很困难的。因此，我们想到了一个逻辑推理，将这个问题转化为研究能量消耗。我们采取的方法如上图所示。

据我们所知，总能量损失包括服务提供者和消费者的实际能量损失和能量自我消耗。考虑到同时检测电流的难度，我们计划在两种状态下异步收集数据，即充电和非充电状态。如图所示，我们可以分别获取服务提供者传输、消费者获取、服务提供者使用和消费者使用的数据。充电状态下服务提供者的损失能量包括服务提供者使用电力和实际传输。此外，消费者实际接收到的能量包括消费者获得和自我消耗。因此，总损失可以通过实际传输减去实际接收的能量来计算。

基本上，我们可以通过使用从能量消耗收集的数据来获取损失。在我们收集的数据方面，它们是时间序列数据。正如在第2节中提到的，我们计划集中于构建时间序列模型（例如RNN）来估计能量消耗。此外，在特征选择过程中，电池电量是我们的首要关注点。我们可能会添加其他变量，如电池温度、CPU使用等，以提高模型的准确性。

至于我们的评估指标，我们计划使用下面的公式，其中Y表示时间序列中每个时间窗口的能量观察值，Y hat表示每个时间步长的能量预测。

- $f(\hat{Y},Y) = |\frac{\sum{ \hat{y}} - \sum{y}}{\sum{y}}|$

我们的贡献如下：

- 建立一个可以实现距离能量传输的CES平台。
- 该平台可以自动显示可能源自众包能源服务过程的能量损失信息。

### 参考文献

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
