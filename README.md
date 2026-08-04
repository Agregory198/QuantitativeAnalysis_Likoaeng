# Late Holocene riverine resource intensification and its effect on hunter-gatherer technological strategies at Likoaeng, Lesotho



## Folder structure

- `data/`: contains input data for all R quarto documents
- `code/`: all analysis scripts required to re-run the project provided as quarto documents
- `results/`: figures, tables, and other output files produced inside and outside R

## Instructions to reproduce this study
To reproduce this study, please pull this repository into a new R project and restore the environment via _renv::restore()_ install _renv_ if not installed already. This will load the package versions used during this study. You can then render each of the files in the _'code'_ folder. This will run the script and export the figures according to this repository's folder structure (_'/results/figures'_). The images are already provided in _'results/figures'_ directory. The quarto documents will also pull the data in according to this repository's folder structure (_'/data'_), which take the form of comma-separated-values and one xlsx file with multiple saved sheats.


## Overview
This is a multivariate project that examines whether hunter-gatherer technological strategies changed when they increased shellfish consumption at Steenbokfontein Cave. I use Bayesian models to evaluate the relationship of several stone tool variables including utility, length, mass, and raw material. I use gt_summary and ggplot2 to develop publish-quality tables and figures.

I first describe the composition of hunter-gatherer toolkits, including the raw stone material, types, and frequencies of their stone technology. I describe these data in tabular and graphical representations. I then construct a Bayesian model with catgeorical and Bernoulli families to evaluate whether there are significant trends in raw material and toolkit composition as hunter-gatheres focused on coastal resources.

I then evaluate three specific artifact classes most commonly found in archaeological contexts to evaluate whether there are technological shifts sensitive to increased coastal resource exploitation. Namely, I examine stone flakes, cores, and scrapers. I use attributes I recorded from the tools to evaluate shifts in tool utility, reduction, and retouch intensity. To do this, I modeled several Bayesian GLMs composed of simple, hierarchical, and second order polynomials. I then evaluate which model fit the data best using a leave-one-out analysis. I then visualize and compute the rate of change between tool utility, reduction, and retouch intensity for the three stone tool classes.

See the links for a sample of flakes, cores, and scrapers.
- ![flakes](results/plates/flakes_silcrete.pdf)
- ![cores](results/plates/cores_quartz.pdf)
- ![scrapers](results/plates/scraper_silcrete.pdf)

## Hypothesis
I expect shifts in toolkits as hunter-gatherers increased coastal resource use. If my models show significant shifts in toolkit composition and rates of change between tool utility, reduction, and retouch intensity, then there is evidence to support this hypothesis.

## Results


### Toolkit Composition
Though there are visible trends in toolkit and material composition (**FIgure 1**), a proportional model conducted with a categorical and bernoulli family show no significant differences. This contradicts previous observations that predicted hunter-gatherer toolkits shift in response to changing mobility and dietary patterns.
![Figure1](results/figures/Figure5.png)


### Flaked tools
There are clear trends in how hunter-gatherers managed their flaked tool utility and reduction intensity (**Figure 2**) as they increased coastal resource use. **Figure 2** and **Figure 3** show the slope estimate between flake utility and reduction intensity. There are clear shifts towards lower rates as hunter-gatherers focused on coastal resources. This result implies that hunter-gatherers focused on much slower shifts between flake utility and reduction intensity when focused on coastal resource use.
![Figure2](results/figures/Figure12a.png)
![Figure3](results/figures/Figure12b.png)

### Core tools
There are no visible trends in how hunter-gatherers managed their core tool utility to reduction intensity (**Figure 4**). This implies that core maintenance is not always sensitive to shifts in hunter-gatherer diets and mobility strategies.
![Figure4](results/figures/Figure13a.png)

### Scrapers
There are no visible trends in how hunter-gatherers managed scraper utility and retouch intensity as they increased coastal resource use(**Figure 5**). This suggests that we should expects shifts in every aspect of hunter-gatherer toolkits. Instead, a focus on coastal resources led to a shift in selective technologies.
![Figure5](results/figures/Figure14a.png)

## Conclusion


## Tools Used
- 'R'
- 'tidyverse', 'ggplot2', 'gt', 'brms'
- Quarto

## Author

Alex Gregory

PhD Candidate | Quantitative Analyst | Data Scientist | Bayesian | Archaeologist


arg9496@nyu.edu
