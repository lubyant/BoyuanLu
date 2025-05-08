---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'>

Boyuan Lu is a Ph.D. in Civil and Environmental Engineering (with double major in Computer Science) the University of Wisconsin-Madison. I started my PhD program in 2018 and am expected to graduate in 2025. My current research fields include coastal morphology, wave climate, wave dynamics, artificial intelligence and software development. 


# 🔬 Research
- Coastal geomorphic change in Lake Michigan

<p float="center">
<img src="images/geomorphology.png" width="100%" />
<figcaption style="font-size: 1em;">Figure 1: geomorphology in Lake Michigan.</figcaption>
</p>
Coastal geomorphologies in Lake Michigan are diverse and include shorelines, beaches, bluffs, dunes, and other landforms. Two of the most common landforms among them are shoreline and bluff, which are shown in figure 1-1a. Shoreline is the natural boundary of water body and land , excluding areas modified by human structures such as revetments and ripraps. Natural shorelines are the mostly commonly found along the coast of Lake Michigan, comprising over 80 percent of the total coastline (see figure1-1b), with the exception of certain urbanized areas such as Chicago and Milwaukee. The second common coastal feature is glacial till bluff, a vertical landform which is formed by glacial movement. Bluffs typically rise behind the shoreline and beach, with heights ranging from one to forty meters. In Lake Michigan, bluffs are primarily distributed along the western and eastern coasts, as shown in Figure 1-1c, accounting for approximately 40 percent of the total lake coastline. Both shorelines and bluffs are not only common but also significant, as they are located in or near populated and developed areas such as Chicago and Milwaukee. These areas affect the lives of over 10 million people and protect properties valued at more than 1,000 billion dollars, with an estimated cost of $10,000 per linear foot of lakefront. Overall, coastal geomorphologies, especially coastal bluff and shoreline, are both prevalent and important in Lake Michigan coastal environments, necessitating comprehensive and detailed studies.

Reach-level bluff recession results aggregated at spatial averages are shown in Figure 2, and shoreline movement results are summarized in Table 3, respectively. Reaches 5, 6, 10, and 12, all reaches featuring high bluffs, consistently featured elevated recession rates compared to surrounding reaches, with the greatest long-term recession rate observed in Reach 5 of -0.85 m/year at the bluff crest from 1937-2015 and -0.53 m/year from 1995-2015. Most of reaches showed mitigations in terms of bluff crest and bluff toe recession rate. However, the bluff crest in reach 10 and 12 presented an accelerated erosion in the past two decades. 
<p float="center">
  <img src="images/erosion_rate.png" width="100%" />
  <figcaption style="font-size: 1em;">Figure 2: coastal change rate (reach scale)</figcaption>
</p>

Local bluff recession rates are presented as 100-meter erosion map in Figure 3. The maximum bluff recession over the 1995-2015 period occurred in northern Racine County, with localized recession rates of -1.8 and -2.2 m/year at the toe and crest, respectively. From 1937-2015, 52% of transects had bluff toe recession rates greater than -0.1 m/year, and 19% of transects recorded rates greater than -0.3 m/year. For the 1995-2015 period, 29% of transects eroded at rates greater than -0.1 m/year and 8% of transects had bluff toe recession rates greater than -0.3 m/year.
<p float="center">
<img src="images/erosion_rate2.png" width ="100%" />
<figcaption style="font-size: 1em;">Figure 3: coastal change rate (county scale).</figcaption>
</p>

The dataset of coastal morphology is available on [oblique viewer]("https://www.arcgis.com/apps/instant/minimalist/index.html?appid=c47ab45bb8c046e099a46df28837ca88")

- Wave climate in Lake Michigan

Wind-waves play a vital role in shaping coastal morphology, guiding structural design, and supporting ecosystem health, with wave climate—defined by parameters such as height, period, energy, and directionality—serving as a key descriptor across scientific and engineering applications. Among these, wave directionality is particularly important but often understudied, especially in freshwater systems. While uni-directional waves can cause consistent sediment transport, bi-directional waves may lead to sediment imbalances, structural instability, and navigation hazards. Although directionality has been examined in some marine regions, it remains insufficiently explored in Lake Michigan. Existing studies mainly focus on wave height trends, leaving gaps in the quantitative analysis of directional patterns. This research addresses those gaps by using historical hindcast data (1979–2023) to characterize spatial and temporal trends of wave directionality along the southeastern Wisconsin coast of Lake Michigan, including under extreme wave conditions, providing insights into its implications for coastal morphology and infrastructure.

<p float="center">
<img src="images/directionality.png" width ="100%" />
<figcaption style="font-size: 1em;">Figure 4: wave directionality</figcaption>
</p>
Wave directionality (figure 4) was characterized using both qualitative and quantitative methods. Qualitatively, wave rose maps were used to visualize wave direction and height, dividing wave angles into 16 spokes and aggregating wave heights in 0.4-meter intervals. Quantitatively, the Wave Height Directionality Index (WHDI) was applied to assess the relative dominance of northern (0°–90°) and southern (90°–180°) waves over the 1979–2023 period. WHDI compares the aggregated significant wave heights from the two directions, with values close to ±1 indicating strong uni-directionality and values near 0 suggesting bi-directionality. A threshold of 0.33 was used to distinguish between uni- and bi-directional patterns, and a sensitivity test was performed to evaluate this classification.

$$
WHDI = \frac{\sum Hs_1 - \sum Hs_2}{\sum Hs_1 + \sum Hs_2}
$$

<p float="center">
<img src="images/directionality_res.png" width ="100%" />
<figcaption style="font-size: 1em;">Figure 5: wave directionality in Lake Michigan</figcaption>
</p>

The directional characteristics of nearshore wave climates were analyzed across the entire shoreline of Lake Michigan using data from 490 WIS stations (figure 5). Two main wave patterns were identified: uni-directional waves, prevalent along the northern and southern shores, and bi-directional waves, common along the western and eastern coasts. Northern areas typically receive waves from the southwest, while southern areas receive waves from the north. In contrast, the western shoreline experiences waves from the northeast and southeast, and the eastern shoreline from the northwest and southwest. These patterns are consistent with offshore buoy data and are largely influenced by the lake’s elongated north-south shape, which creates longer wind fetch in that direction. Longer fetches generate larger waves, explaining the prevalence of uni-directional waves along the north and south shores and bi-directional waves along the east and west coasts.


# 📂 Projects
- Application of CUDA in CFD solver [github]("https://github.com/lubyant/CS759-HPC/tree/master/FinalProject759")

This project is motivated by my personal interest and is an extension of my course projects. The field of computational fluid mechanics is inextricably linked to high-performance computing.From a broader point of view, numerically solving NS equations requires a huge amount of computation, which can be accelerated by parallel computing. The goal of this project is to implement the three versions of Chorin’s fractional step
method (no parallel, OpenMP, and CUDA) and build a specific solver for two-dimensional incompressible Navier-Stokes equations with predefined initial and boundary conditions.

<p float="center">
  <img src="images/fig6.png" width="100%" />
</p>


# 📝 Publications 
1. Wave climate on the southwestern coast of Lake Michigan: Perspectives from wave directionality, Ocean Engineering [under review]

# 🎖 Honors and Awards
- *2020* Villemonte Award. 
- *2021* Villemonte Award.

# 📖 Educations
- *2012.09 - 2016.08*, Port Channel and Coastal Engineering, BA. Oceaning Univeristy of China. 
- *2017.09 - 2018.08*, Civil and Environment Engineering, MS. Univeristy of Wisconsin, Madison. 
- *2018.09 - 2025.05*, Computer Science, MS. Univeristy of Wisconsin, Madison. 
- *2018.09 - 2025.09*, Civil and Environment Engineering, PhD. Univeristy of Wisconsin, Madison. 


# 💻 Internships
- *2024.01 - 2024.05*, Software Engineer, Celonis, NYC