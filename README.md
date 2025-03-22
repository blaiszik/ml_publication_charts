# Charting ML Publications in Science

As machine learning has grown in popularity and domain of applicability, charts showing the growth have popped up in review articles, presentations, and more.
Many of these charts seem to have different numbers (though showing the same trend!), and are often without provenance. Thus, this repository was made to act as a resource for those looking to dig into the numbers further, to quickly customize our existing plots, or to simply find a ready-made chart for their own usage. 

# 2024 Results
Table showing the count and Compound Annual Growth Rate (CAGR) on the raw number of articles published over different periods for each domain. CAGR-N represents the CAGR over N years. 

| Domain            | year | count | CAGR-1 (%) | CAGR-2 (%) | CAGR-5 (%) |
|-------------------|------|-------|------------|------------|------------|
| Materials Science | 2024 | 9295  | 20.9       | 21.0       | 44.2       |
| Chemistry         | 2024 | 11562 | 11.9       | 13.9       | 29.0       |
| Physics           | 2024 | 9231  | 12.4       | 15.2       | 37.4       |

# The Charts
Note that the charts come in two forms, normalized and count. Normalized plots take into account the relative size of the domain of interest (i.e., the number of matching articles / the total number of articles in a domain).

## Normalized Line Plot
![All domain overlay line](./output/2024-normalized.png)

## Raw Count Line Plot
![All domain overlay line](./output/2024-count.png)


## The Domains
* Materials Science
* Chemistry
* Physics


## Methodology
* Web of Science topic matching and matching of domain. Exact queries are provided in the data directory.

| ID      | Service |Query |
| ----------- |----| ----------- |
| 1           |Web of Science| TS=("machine learning" OR "informatics" OR "deep learning" OR "cheminformatics" OR "artificial intelligence" OR "chemoinformatics" OR "QSAR" OR "QSPR") AND WC="{Domain}"  |


## Customization
* All routines to create the plots are provided in the repo notebooks. 
* Customize the figure closest to your heart, and it will be saved out to the output directory.
* Don't like the queries used? Simply output your data to the same format used in /data/1.csv and re-use the plotting tools.

## TODO (Pull requests welcome)
* Automate data pull through Web of Science API
* Consider a Google Scholar implementation
* Improve plot consistency and styling
* Add statistics for other domains
* Consider adding other common plots
* Fix plots now that there are more domains in the data

## Cite
Ben Blaiszik, “2021 AI/ML Publication Statistics and Charts”. Zenodo, Sep. 07, 2022. doi: 10.5281/zenodo.7057437.

```
@software{ben_blaiszik_2023_7713954,
  author       = {Ben Blaiszik},
  title        = {{blaiszik/ml\_publication\_charts: AI/ML Publication 
                   Statistics for 2022}},
  month        = mar,
  year         = 2023,
  publisher    = {Zenodo},
  version      = {2023.03},
  doi          = {10.5281/zenodo.7713954},
  url          = {https://doi.org/10.5281/zenodo.7713954}
}
```
