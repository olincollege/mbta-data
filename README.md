# MBTA Ridership Analysis by  Demographic Factors
**Explore the impact of demographic factors on the ridership of public transit (light rail and subway(T)) in the Boston area.** 

By Becca Flach, Camille Kawabata, Sally Lee, Sherry Li, Noah Woosley

*Published Apr. 25, 2024*

# Introduction

In the bustling, hectic cityscape of Boston, public transit should be the network that connects everyone. Instead of acting as the great connector, the rapid transit lines in Boston perpetuate racial and class divides. This works directly against the United Nation’s Sustainable Development Goals, specifically target 11.2; “By 2030, provide access to safe, affordable, **accessible and sustainable transport systems for all**, improving road safety, notably by expanding public transport, with special attention to the needs of those in vulnerable situations, women, children, persons with disabilities and older persons”.

## Region of Focus

### Suffolk County

Suffolk County is composed of four cities:

- Boston
- Revere
- Chelsea
- Winthrop

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/165708e3-3274-4ef5-838c-75648529fa28/Untitled.png)

Within the four cities above, we used a block group, the smallest geographic unit that the census uses with 250-550 houses for each unit, to analyze our census and compare it to the ridership data. 

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/3b6910f8-0032-4331-992c-5e1c17cfe365/Untitled.png)

## Demographic Factors Affecting Ridership

### Median Income

One of the key demographic factors we hypothesized to impact transit usage is income level. We assumed that lower-income individuals may heavily rely on public transportation due to limited access to private vehicles or the high cost of car ownership. 

### Race

Race is another important demographic factor that influences public transit usage patterns. In Boston, as in many other cities, we assumed that there would be disparities in transit access and usage among the differential racial and ethnic groups. We expected to see variations in transit ridership based on racial demographics, with certain communities showing higher levels of public transit usage compared to others. 

# Methodology

To measure public transit usage, we used the data published by the MBTA about the number of entries to each gated station. We combined this with census data by finding which station was closest to each census block. Using the population, income, and demographic information for each census block group, we investigated the relationship between transit usage and demographic factors. 

# Key Insights on Ridership and Demographics

![uasge.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/b9504b7f-c8b8-4dad-a85f-ae5348109d40/uasge.png)

Figure 1: choropleth map depicting the percentage of the population that uses either the light rail or subway to get to work in Suffolk County in 2016 and 2022 with the station locations overlaid.

Looking at this, people that live closer to stations tend to be more likely to use the subway or the light rail to get to work. This makes their commutes both more sustainable and more economic. However, it is important to note that there are communities in the area that are both far from stations and have a low percentage of people that use the subway or light rail to commute to work. 

![TF Normalized Usage Increase.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/09b184b7-4163-47b0-9eca-0ff259818106/c10e401e-fb8f-4495-87de-683869b70b47.png)

![Diff Normalized Usage.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/a2f32b7c-7334-4670-96b5-368332a8ace4/817b1fbf-d9cc-4a19-8ccd-632345b10f84.png)

[]()

Figure 2: 

## Ridership and Median Income

![income.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/7dbdde40-0975-4879-9129-c33565d19fec/income.png)

Figure 3: a choropleth map illustrating the changes in median household income between 2016 and 2022 in Suffolk County with light rail and subway station locations overlaid.

Looking at this, for both 2016 and 2022, there appears to be higher median income along the lines of stations than far away from stations. This means that there tends to be less access to public transportation in areas that have a lower median income.

### Linear Regression on Gated Entries vs. Income

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/4801d274-9edf-4ddb-bd15-e436c12aefd3/Untitled.png)

Figure 4: a scatterplot and the line of best fit showing as the median household income increases, the more gated entries to the public transit.

In analyzing the dynamics of public transit ridership, we were able to find a correlation between median household income and the utilization of public transit systems. As observed from the scatterplot and line of best fit, we visually depicted how the number of gated entries to public transit tends to increase as median household income rises. This finding suggests a significant relationship between socioeconomic status and transit accessibility, with implications for urban planning and transportation policy. As median household income climbs, so does the likelihood of individuals utilizing public transit—a trend that sheds light on the complex interplay between economic factors and transportation preferences.

## Ridership and Race

![racial demographics.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/ff3250e6-18a2-4e3d-9149-a764ee24a89c/racial_demographics.png)

Figure 5: choropleth map illustrating the distribution of racial group in the Suffolk County

In areas where there are high concentrations of communities of color, the ridership of public transit sees increased usage between 2016 and 2022. Even in a post-COVID world, people of color are relying on public transit to get to work. This reliance enforces the economic disparity between racial groups in Boston because entire communities are losing out on job opportunities. When looking at the location of MBTA stations, it is clear that white and wealthy communities have the easiest access to stations.

![redline locations.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/5410a571-f361-4107-a520-ab81394264a9/redline_locations.png)

Figure 6: choropleth map of the percentage of the population that identifies as black or African American overlayed with red line station locations in 2022.

From this mapping of station locations, we can see that rapid transit lines do not run through areas where there are higher concentrations of non-white groups. This is supported by the following linear regression models.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/5afe265e-c4c0-4fdb-8f69-6d2867bcee3d/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/0c199a7d-594d-4637-895c-7b102846679a/e77f218e-4531-4491-a979-6a699654fb53/Untitled.png)

Figure 7 (*left*), 8 (*right*): scatter plot and line of best fit showing the relevance between the race and the gated entries. The figure on the left side shows that the more white the demographic is, the more gated entries to the public stations, and the figure on the right shows that the more black the demographic is, the fewer gated entries to the public stations. 

Even though black communities are more likely to utilize public transit in getting to work (likely because of economic barriers), these models show that when an area is “whiter”, they use gated stations at a higher rate because of how accessible the station locations are to them.

# Implications

Understanding the inverse relationship between median income and public transit ridership yields critical insights for transportation planners and policymakers:

- **Equitable Access:** Initiatives aimed at enhancing public transit accessibility should prioritize underserved communities and mitigate disparities stemming from income inequality. By bolstering service coverage and improving connectivity, public transit can emerge as a viable mobility solution for all residents, irrespective of socio-economic status.
- **Fare Structures and Affordability**: Crafting fare structures that align with the financial realities of diverse demographics is imperative. Implementing income-based fare programs or offering discounted rates for low-income individuals can foster inclusivity and promote transit equity, ensuring that economic barriers do not impede access to essential transportation services.
- **Urban Development and Transit-Oriented Design**: Urban planners must integrate public transit considerations into development projects, fostering transit-oriented communities that prioritize pedestrian-friendly infrastructure and seamless transit connections. By fostering vibrant, accessible urban environments, cities can incentivize public transit usage and promote sustainable modes of transportation.

# Conclusion

### Towards Equitable Mobility Solutions

In Boston, the rapid transit system serves as both a vital connector and clear example of inequity. While the the light rail and subway can be used to link various parts of the city together, this benefit is not felt equally among all residents. The T predominantly caters to wealthier and white residents and leaves behind low-income communities and people of color.

As cities grapple with the complexities of urbanization and transportation, addressing the intricate interplay between ridership and median income is paramount. By prioritizing equity, accessibility, and sustainability in transportation planning endeavors, interested parties can forge a path towards inclusive transportation solutions that empower communities and foster socio-economic prosperity for all.

## Appendix

### Blog Post

[MBTA Ridership Analysis by  Demographic Factors](https://github.com/olincollege/mbta-data)

## Data Sources
[Station Location Data](https://github.com/singingwolfboy/MBTA-GeoJSON)
[Station Entry Data](https://mbta-massdot.opendata.arcgis.com/datasets/7859894afb5641ce91a2bb03599fdf5b/about)
