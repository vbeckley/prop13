## California Proposition 13
### Background

Established in 1978 with the intention to protect homeowners from paying too high of property taxes as statewide home values increased at a rapid rate.

The law created a base year value for home, a restricted rate of increase of no greater than 2% a year, and a limit on property taxes to 1% of the assessed value (plus any local additional taxes)

In San Francisco the current property tax rate is 1.18%

As a result property taxes increase at the Consumer Price Index each year, while home values, especially in San Francisco, increase at a rate closer to 6% a year.

This can result in properties like the one below where the property taxes paid are much less than 1% of the actual home value.

<img src="https://victoriabeckley.github.io/prop13/Screen Shot 2022-05-09 at 10.43.21 PM.png" alt="Sample Home" style="width:150px;height:150px;">
<img src="https://victoriabeckley.github.io/prop13/Screen Shot 2022-05-09 at 10.43.37 PM.png" alt="NPR Map" style="width:600px;height:200px;">
<a href="https://projects.scpr.org/prop-13/">Project from NPR, 2018</a>

### Questions

<ul>
  <li>What does the impact of prop 13 look like in San Francisco?</li>
  <li>How do market rate housing costs, years of occupancy, and property taxes interplay?</li>
  <li>Does prop 13 deepen inequality by further subsidizing wealth accumulation for homeowners? Especially multi-generational wealth?</li>  
  <li>Does prop 13 challenge local governments’ ability to have accurate home value data?</li>  
</ul>

### Analysis

<iframe src="https://victoriabeckley.github.io/prop13/zillow_chart.html" width="100%" height=500 title="Zillow Market Rate Home Value Estimate by Neighborhood"></iframe>
This chart shows <a href="https://www.zillow.com/research/data/">Zillow's Market Rate Estimate</a> of the "Typical Home Value" by neighborhood in San Francisco by month from 2000 to 2022. This helps us see the large discrepancy across neighborhoods in the city.

<iframe src="https://victoriabeckley.github.io/prop13/assessed_chart.html" width="100%" height=500 title="Assessed Home Value by Neighborhood"></iframe>
This chart shows us the assessed home value averaged by neighborhood in San Francisco from 2007 to 2019. This helps us see how the values increase at the consumer price index instead of market rates. We again see a large discrepancy across neighborhoods.

<img src="https://victoriabeckley.github.io/prop13/Screen Shot 2022-05-09 at 11.54.05 AM.png" alt="Difference">
Here we see the two charts combined to show the difference by neighborhood between market rate and assessed home value. This is our best attempt to generate a "tax subsidy" based on Prop 13.

<img src="https://victoriabeckley.github.io/prop13/Screen%20Shot%202022-05-09%20at%2011.55.20%20AM.png" alt="Presidio Heights">
Some neighborhoods benefit more than others from this tax subsidy. Presidio Heights is the most egregious example of this due to the combination of high home values, averaging 4.9 million in 2019, and long term homeownership making average assessed home values in 2019 only 1.8 million. This creates an average subsidy in Presidio Heights of 3.1 million in 2019.

<img src="https://victoriabeckley.github.io/prop13/Screen Shot 2022-05-09 at 11.55.13 AM.png" alt="The Tenderloin">
Meanwhile the Tenderloin experienced a very different experience in this same time in which the assessed value tended to be higher than the Zillow estimate home value. Here the home value estimate in 2019 averaged $819,000, while the assessed value was an average of 1 million, somehow creating a negative average subsidy!

<iframe src="https://victoriabeckley.github.io/prop13/difference.html" width="100%" height=500 title="Assessed Home Value by Neighborhood"></iframe>
Here we see that tax subsidy by neighborhood to see that some neighborhoods benefit disproportionately more than others, with Presidio Heights and Cow Hollow way above all other neighborhoods in the city.



### Data Sources

<ul>
  <li><a href="https://data.sfgov.org/Housing-and-Buildings/Assessor-Historical-Secured-Property-Tax-Rolls/wv5m-vpq2">SF Assessor’s Office Property Tax Roll:</a> GEOJSON - points (2.3 million)</li>
  <li><a href="https://www.zillow.com/research/data/">Zillow Home Value Index:</a> CSV - by neighborhood</li>
  <li><a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Realtor-Neighborhoods/5gzd-g9ns">SF Realtor Neighborhoods:</a> GEOJSON - polygons</li>
  <li><a href="https://data.census.gov/cedsci/table?q=B25077%3A%20MEDIAN%20VALUE%20%28DOLLARS%29&g=0500000US06075%241500000&y=2019&tid=ACSDT5Y2019.B25077">ACS MEDIAN VALUE DOLLARS (Table B25077):</a> CSV - by blockgroup</li>
</ul>
