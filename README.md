# MBTA Ridership Analysis by  Demographic Factors
**Explore the impact of demographic factors on the ridership of public transit (light rail and subway(T)) in the Boston area.** 
By Becca Flach, Camille Kawabata, Sally Lee, Sherry Li, Noah Woosley

See our full write up and analysis [here](https://devjourney.notion.site/MBTA-Ridership-Analysis-by-Demographic-Factors-89e74d4050314f8ba22a46e1bb29838f)

## Use
All code for data processing and visualizations is contained in main.rmd. 

To run, you will need to obtain API keys for [Stadiamaps](https://docs.stadiamaps.com/tutorials/getting-started-in-r-with-ggmap/) and [Tidycensus](https://api.census.gov/data/key_signup.html), and substitute them into the code. 

## Data Sources & Packages
All necessary data has been downloaded and placed into this repository, and all packages are automatically installed by pacman. 

Data Sources: 
- [Station Location Data](https://github.com/singingwolfboy/MBTA-GeoJSON)
- [Station Entry Data](https://mbta-massdot.opendata.arcgis.com/datasets/7859894afb5641ce91a2bb03599fdf5b/about)

Packages:
- forcats
- dplyr
- readr
- ggplot2
- sfheaders
- geojsonsf
- sf
- purrr
- ggmap
- ggthemes
- tidycensus
- scales
- patchwork
- tidyverse