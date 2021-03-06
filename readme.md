# Registered Deaths, COVID Deaths and Excess mortality in Chennai

Uses data scraped from the [Greater Chennai Corporation](https://chennaicorporation.gov.in/gcc/online-services/death-certificate/) website.

Repository contains the following: 

1) Registered deaths in Greater Chennai Corporation from 2006 - May 2021.
	- [By date](https://flatgithub.com/gurmanbh/chennai-registered-deaths-excess-mortality?filename=data%2Fby-date.csv&filters=&sha=b5641e00448585cce53c902c872fc02fc79061b0&sort=date%2Cdesc&stickyColumnName=date)
	- [By month](https://flatgithub.com/gurmanbh/chennai-registered-deaths-excess-mortality?filename=data%2Fby-month.csv&filters=&sha=b5641e00448585cce53c902c872fc02fc79061b0&sort=month%28date%29%2Cdesc&stickyColumnName=month%28date%29)
	- [By day and sex](https://flatgithub.com/gurmanbh/chennai-registered-deaths-excess-mortality?filename=data%2Fby-date-sex.csv&filters=&sha=b5641e00448585cce53c902c872fc02fc79061b0&sort=month%28date%29%2Cdesc&stickyColumnName=month%28date%29)
2) Excess mortality calculated from registered deaths and compared with reported COVID deaths. [Data](https://flatgithub.com/gurmanbh/chennai-registered-deaths-excess-mortality?filename=data%2Fexcess-deaths.csv&filters=&sha=b5641e00448585cce53c902c872fc02fc79061b0&sort=Date%2Cdesc&stickyColumnName=Date)
3) Charts illustrating the extent

Note: All datasheets were last updated on June 16, 2021. As explained by [Rukmini S in this story](https://www.thehindu.com/opinion/op-ed/interpreting-deaths-in-chennai/article34645264.ece), the data for 2021 is likely to be an underestimate as people have up to an year to register deaths. I plan on updating this repository periodically.

The charts end at May 4, 2021 and are based on data pulled on June 9.

---------
## What is excess mortality?

Excess deaths are calculated by taking a historical average to borrow from a _normal year_ and comparing it with a _pandemic year_ to look the extent of deaths that are above the normal.

As the second wave of the pandemic sweeps through the country, and reported numbers are proven to be [underreported](https://www.indiaspend.com/covid-19/mortality-data-kerala-mumbai-too-soon-to-say-india-covid19-less-deadly-second-wave-737270) [time](https://twitter.com/deepakpatel_91/status/1393070596741734405?s=20) [and](https://twitter.com/deepakpatel_91/status/1397420984592908291?s=20) [again](https://twitter.com/deepakpatel_91/status/1397447291707875334?s=20), excess mortality figures can help us with better estimates of the true toll of the pandemic. This borrows from our experience of [previous pandemics](https://indianexpress.com/article/opinion/columns/why-excess-mortality-figures-for-covid-must-be-calculated-7330348/), where the recorded number of deaths was much lower than the actual number. 

----------

## Chennai's Factor
As per data pulled on June 9, for the period between April 27, 2020 and May 04, 2021, Chennai recorded the following numbers

- Registered Deaths: 83,153
- Reported COVID Deaths:  4,879

The 5 year average for the same period between 2015 - 2019 is 63,726 deaths.

Under-reporting factor = (Registered Deaths - Historical Avg) / Reported COVID Deaths

The brings the current under-reporting factor for the city at \~4.

If we compare the same numbers for April 2021: 
- Registered Deaths: 8,971
- Reported COVID deaths: 501
- Historical Avg: 4,675
- Under-reporting factor: 8.5

While my calculation is simplistic, Ariel Karlinsky's sophisticated model that accounts for growth, seasonality, other factors, says b/w Apr 4-May 16 - [deaths in Chennai were 6.2x of the reported figures](https://twitter.com/ArielKarlinsky/status/1402604339558969350?s=20). My simple math would place that time period at 7x.


![Registered deaths in Chennai (14-day rolling average)](charts/deaths.png)

Based on the Economist's Excess Mortality chart. See how to read the chart [here](https://www.economist.com/graphic-detail/coronavirus-excess-deaths-tracker).
![Excess deaths and COVID-related deaths in Chennai (14-day rolling average)](charts/excess-deaths.png)

----------

Another Chennai based doctor has also been [scraping the data](https://github.com/elseasama/covid19chennai). 
