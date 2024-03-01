---
title: 'Household displacement after disasters'
summary: '*Supervised by Prof. Carmine Galasso and Prof. Jack Baker*'
tags:
  - household displacement
date: '2022-09-26T00:00:00Z'
show_date: False

# Custom parameter for icons
title_icon: True
icon_pack: fa
icon_name: person-shelter

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: ''

links:
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

---

{{% callout note %}}
For a review on household displacement and return after disasters, please refer to my <a href="https://doi.org/10.1061/NHREFO.NHENG-1930" target="_blank">open access paper<i class="ai ai-open-access ml-1"></i></a>
{{% /callout %}}


### Overview

Over 265 million people were displaced due to disasters between 2008 and 2018[^1]. In the forthcoming years, the annual number displaced is expected to increase, driven by poorly-managed urban growth in hazard-prone areas[^2] and potentially exacerbated by climate change[^3]. Despite this scale of human impact, most disaster risk assessments focus on direct economic losses, a metric that often highlights the wealthiest as the most at-risk. However, the reality of disasters is that the poor are disproportionately affected[^4], and mitigations informed primarily by economic loss may deepen existing inequalities. This research proposes to quantify disaster-induced displacement; a more equitable risk metric to depict the human toll of disasters.

### Research themes

{{< spoiler text=" The importance of duration" >}}
Most statistics regarding population displacement following a disaster event provide single snapshot values, often representing a peak estimate during the emergency phase. However, the duration of displacement is essential for understanding the human impact. For example, large- scale displacement in the form of evacuations before a storm can save lives and be followed by mass return shortly afterward. In contrast, a devastating event such as an earthquake could damage or destroy a significant proportion of the residential building stock, causing occupants to seek alternative accommodations for months to years. Not only does this type of protracted displacement pose a significant disruption to the livelihoods of affected households (e.g., lost income, interrupted education), but the consequences can ripple out into the larger community (e.g., outmigration and urban blight, lost economic production). Therefore, a key objective of this research is to refine our understanding of household displacement duration in disasters.

![Timeline representing displacement duration alongside key phases of disaster management and recovery.](project/household-displacement/timeline.png "Timeline representing displacement duration alongside key phases of disaster management and recovery.")
{{< /spoiler >}}

{{< spoiler text=" Determinants of household return" >}}
Disasters are life events that can subject households to key decision points, such as: whether to evacuate, where to seek shelter, whether to return/wait/relocate, and whether to stay or resettle. From a [literature review](/publication/journal-article/2024-household-displacement-in-disasters-review/) of household return after disasters, the following categories of determinants have been identified.

|   | Category | Determinants of return |
|---|----------|------------------------|
| <i class="fa-solid fa-house-chimney-crack"></i> | Physical damage to the built environment | <ul><li>Habitability of housing (damage, weather, utilities)</li><li>Housing type</li><li>Community damage</li><li>Reconstruction progress</li></ul> |
|  <i class="fa-solid fa-users"></i> | Psychological & social phenomena| <ul><li>Acceleration of ongoing trends</li><li>Attachment to place</li><li>Social capital (networks, family and friends)</li><li>Perceived risk</li></ul> |
| <i class="fa-solid fa-id-card"></i>  | Household demographics| <ul><li>Socioeconomic status (e.g., income level)</li><li>Housing and land tenure</li><li>Race/ethnicity/caste</li><li>Age</li></ul>|
|  <i class="fa-solid fa-building-columns"></i> | Pre- and post-disaster policies          | <ul><li>Pre-existing housing conditions (e.g., vacancies)</li><li>Housing reconstruction approach</li><li>Other disaster assistance policies</li></ul> |
{{< /spoiler >}}

{{< spoiler text=" The role of housing damage" >}}
Disaster literature offers a clear consensus that housing damage is a primary driver of household displacement of disasters, at least in the emergency phase. However, additional factors (e.g., place attachment and housing tenure) have more recently been proposed as highly influential for household return in the recovery phase. Despite the range of factors beyond damage that have been proporsed to influence household return, standard practice in disaster risk analysis is to solely consider housing damage. That is, the number of destroyed homes is multiplied by the average household size to yield an estimate of the displaced population.

In an initial study, I benchmarked predictions of household displacement based solely on housing damage to understand the extent to which such simplified models can explain the phenomenon. The results of the benchmarking study are available in a [conference paper](/publication/conference-paper/2023-benchmarking-displacement-earthquakes/).

![Benchmarking results for displacement estimates using a scenario risk analysis that only considers housing damage (green) versus official reports and mobile location data-based estimates.](project/household-displacement/benchmarking.png "Benchmarking results for displacement estimates using a scenario risk analysis that only considers housing damage (green) versus official reports and mobile location data-based estimates.")
{{< /spoiler >}}


### Acknowledgments

This research is partly funded by the University College London Overseas Research Scholarship (ORS) and the Willis Towers Watson Research Network.


[^1]: IDMC. 2019. “Disaster Displacement - A Global Review, 2008-2018.” https://www.internal-displacement.org/publications/disaster-displacement-a-global-review.
[^2]: IDMC. 2017. “Global Disaster Displacement Risk - A Baseline for Future Work.” https://www.internal-displacement.org/publications/global-disaster-displacement-risk-a-baseline-for-future-work.
[^3]: IPCC, ed. 2012. “Summary for Policymakers.” In Managing the Risks of Extreme Events and Disasters to Advance Climate Change Adaptation, 1st ed. Cambridge University Press. https://doi.org/10.1017/CBO9781139177245.
[^4]: Hallegatte, Stéphane, Adrien Vogt-Schilb, Julie Rozenberg, Mook Bangalore, and Chloé Beaudet. 2020. “From Poverty to Disaster and Back: A Review of the Literature.” Economics of Disasters and Climate Change 4 (1): 223–47. https://doi.org/10.1007/s41885-020-00060-5.
[^5]: IDMC. 2018. “GRID Methodological Annex.” https://www.internal-displacement.org/global-report/grid2018/downloads/report/2018-GRID-methodological-annex.pdf.