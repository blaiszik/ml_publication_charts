# Charting ML Publications in Science

As machine learning has grown in popularity and domain of applicability, charts showing the growth have popped up in review articles, presentations, and more.
Many of these charts seem to have different numbers (though showing the same trend!), and are often without provenance. Thus, this repository was made to act as a resource for those looking to dig into the numbers further, to quickly customize our existing plots, or to simply find a ready-made chart for their own usage. 

# The Charts
## Scatter Plots
![All domain grid scatter](./output/1-grid.png)
![All domain overlay scatter](./output/1-all-scatter.png)

## Line Plots
![All domain grid line](./output/1-grid-line.png)
![All domain overlay line](./output/1-all-line.png)

## The Domains
* Materials Science
* Chemistry
* Physics


## Methodology
* Web of Science topic matching and matching of domain. Exact queries are provided in the data directory.

| ID      | Service |Query |
| ----------- |----| ----------- |
| 1           |Web of Science| TS=("machine learning" OR "informatics" OR "deep learning") AND WC="{domain}"  |


## Customization
* All routines to create the plots are provided in the repo notebooks. 
* Customize the figure closest to your heart, and it will be saved out to the output directory.
* Don't like the queries used? Simply output your data to the same format used in /data/1.csv and re-use the plotting tools.

## TODO (Pull requests welcome)
* Automate data pull through Web of Science API
* Consider a Google Scholar implementation
* Improve plot consistency and styling
* Add statistics for other domains
* Update for 2019 when full data are available
* Consider adding other common plots

## Cite
No citation yet, check back soon.
