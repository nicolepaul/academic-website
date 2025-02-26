---
title: "A predictive model for household displacement duration after disasters"
authors:
- admin
- Carmine Galasso
- Jack Baker
- Vitor Silva
date: "2025-02-26T00:00:00Z"
doi: "10.1111/risa.17710"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-02-26T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*Risk Analysis*"
publication_short: ""

abstract: "According to recent Household Pulse Survey data, roughly 1.1% of households were displaced due to disasters in the United States in recent years. Although most households returned relatively quickly, 20% were displaced for longer than 1 month, and 14% had not returned by the time of the survey. Protracted displacement creates enormous hardships for affected households and communities, yet few disaster risk analyses account for the time component of displacement. Here, we propose predictive models for household displacement duration and return for practical integration within disaster risk analyses, ranging in complexity and predictive power. Two classification tree models are proposed to predict return outcomes with a minimum number of predictors: one that considers only physical factors (TreeP) and another that also considers socioeconomic factors (TreeP&S). A random forest model is also proposed (ForestP&S), improving the model's predictive power and highlighting the drivers of displacement duration and return outcomes. The results of the ForestP&S model highlight the importance of both physical factors (e.g., property damage and unsanitary conditions) and socioeconomic factors (e.g., tenure status and income per household member) on displacement outcomes. These models can be integrated within disaster risk analyses, as illustrated through a hurricane scenario analysis for Atlantic City, NJ. By integrating displacement duration models within risk analyses, we can capture the human impact of disasters more holistically and evaluate mitigation strategies aimed at reducing displacement risk."

# Summary. An optional shortened abstract.
summary: 'This study uses data from the United States Household Pulse Survey to fit predictive models for displacement duration and return after disasters. Three predictive models are proposed, which range in complexity and predictive power. The leading contributors to different duration and return outcomes are also explored. These models can be integrated within disaster risk analyses, as illustrated through a hurricane scenario analysis for Atlantic City, NJ.'

tags:
 - household displacement
featured: true

# links:
url_pdf: https://onlinelibrary.wiley.com/doi/epdf/10.1111/risa.17710
url_code: 'https://github.com/nicolepaul/hps-displacement'
url_dataset: 'https://hps.nicolepaul.io/'
url_poster: ''
url_project: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: ['household-displacement']

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""

# Other options
show_related: true

---
### Interactive dashboard

Explore trends related to property damage and displacement duration from the United States Household Pulse Survey at [**https://hps.nicolepaul.io/**](https://hps.nicolepaul.io/).

### Example figure
![A map of the United States where the percent of households displacement due to disasters is visualized state-by-state.](publication/journal-article/2025_hps_displacement.png "Percentage of households displaced by state according to the United States Household Pulse Survey (based on all available survey datawhere displacement is included through July 2024).")
