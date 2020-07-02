## Sliding SIR Model for Epidemic Modelling

This repository contains code to perform estimation of effective reproductive number Rt of COVID epidemic based on [public data][CountryData]. This code accompanies the following publications:

* Petrova, T.; [Soshnikov, D.](http://soshnikov.com); Grunin, A. Estimation of Time-Dependent Reproduction Number for Global COVID-19 Outbreak. Preprints 2020, 2020060289 (doi: [10.20944/preprints202006.0289.v1][pp]).
* Blog post: [Sliding SIR Model for Rt Estimation during COVID Pandemic][blog]
<!-- (on [Towards Data Science][TDS]) -->

## Citation

If you use any portion of this code in your research, please cite the following:

> Petrova, T.; [Soshnikov, D.](http://soshnikov.com); Grunin, A. Estimation of Time-Dependent Reproduction Number for Global COVID-19 Outbreak. Preprints 2020, 2020060289 (doi: [10.20944/preprints202006.0289.v1][pp]).

The code is distributed under [MIT License](LICENSE)

## Running the Code

The easiest way to run the code is to [clone the repository](https://notebooks.azure.com/import/gh/shwars/SlidingSir) in [Azure Notebooks])https://soshnikov.com/azure/8-reasons-why-you-absolutely-need-azure-notebooks/), or use [Visual Studio Codespaces](https://code.visualstudio.com/docs/remote/codespaces/?WT.mc_id=personal-github-dmitryso) to open the code.

<a href="https://notebooks.azure.com/import/gh/shwars/SlidingSir"><img src="https://notebooks.azure.com/launch.png" /></a>
<a href="https://mybinder.org/v2/gh/shwars/SlidingSir/master"><img src="https://mybinder.org/badge_logo.svg"/></a>
<!-- ?filepath=notebooks%2FSlidingSIR.ipynb -->

## Provided Files

* `notebooks/EpiModelling.ipynb` is the notebook that describes the basics of SIR epidemic modelling, and applies our *Sliding SIR* idea to the epidemic in Moscow
* `notebooks/SlidingSIR.ipynb` contains the code that applies *Sliding SIR* to many countries based on publicly available data, and ties this to *Apple Mobility Index* 
* `data` directory contains the snapshot of datasets used in our modelling. The code uses online publicly available datasets, but should they become unavailable - you would still be able to test the code with the data provided there

## Some Results

The methodology is described [in this blog post][blog]. Here are a few obtained results:

#### Rt Dynamics in Russia
![](http://soshnikov.com/images/blog/SIR/Rt_Russia_Events.png)

#### Rt Dynamics vs. Daily Infected Population Worldwide
![](http://soshnikov.com/images/blog/SIR/Country_Plot.png)

#### Rt Dynamics for Different Countries
![](http://soshnikov.com/images/blog/SIR/Country_Compare_All.png)


[CountryData]: https://github.com/CSSEGISandData/COVID-19
[blog]: https://soshnikov.com/science/sliding-sir-model-for-rt-estimation
[pp]: https://www.preprints.org/manuscript/202006.0289/v1
