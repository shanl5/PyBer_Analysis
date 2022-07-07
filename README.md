# Pyber_Analysis
Charting of merged CSV text file data via Matplotlib pyplot library add-in with Jupyter Notebook, augments Python and Pandas DataFrame and DataSeries coding to provide two-dimensional data visualization for this analysis.

## Project Overview
Pyber, a Python-based ride-sharing app company<sup>i</sup> supporting operations in three types of cities -- Urban, Suburban, and Rural -- has hired the project for an exploratory analysis of a set of "very large"<sup>ii</sup> CSV file data. Two files, one for city-oriented data and one for ride-oriented, will be merged into a single data set to perform the analysis, the goal of which is to aid company management {CEO V. Isualize has background in programming and is an expert in creating data visualizations}<sup>iv</sup> make decisions on how to:
	"improve access to ride-sharing services and determine affordability for underserved neighborhoods.",<sup>iii</sup>

<sup>i, ii, iii</sup> Module 5.0.4 video
<sup>iv</sup> Module 5.1.2

In support of this, the following visuals have been developed (aided by *Omar*, and *Sasha* -- for the Bubble Chart):
	
	A.  A Bubble Chart of Average USD Fare versus Total Number of Rides Per City *(see Fig1.png below)*
	B.  Three Box-and-Whisker Plots
	      (1)  Number of Rides for Each City Type *(Fig2.png, below)*
	      (2)  USD Fare for Each City Type *(Fig3.png, below)*
	      (3)  Number of Drivers for Each City Type *(Fig4.png, below)*
	C.  Three Pie Charts
	      (1)  Percentage of Total Fares by City Type *(Fig5.png, below)*
	      (2)  Percentage of Total Rides by City Type *(Fig6.png, below)*
	      (3)  Percentage of Total Drivers by City Type *(Fig7.png, below)*

**Fig1:** Average USD Fare v Total Number of Rides Per City ![Fig1](/analysis/Fig1_paint.png)\n

**Fig2:** Number of Rides for Each City Type ![Fig2](/analysis/Fig2_paint.png)

**Fig3:** USD Fare for Each City Type ![Fig3](/analysis/Fig3_paint.png)

**Fig4:** Number of Drivers for Each City Type ![Fig4](/analysis/Fig4_paint.png)

**Fig5:** Percentage of Total Fares by City Type ![Fig5](/analysis/Fig5_paint.png)

**Fig6:** Percentage of Total Rides by City Type ![Fig6](/analysis/Fig6_paint.png)

**Fig7:** Percentage of Total Drivers by City Type ![Fig7](/analysis/Fig7_paint.png)

### Results Analysis
A takeaway for each of the seven figures presented above is summarized herein...

  A.<sup>Fig1 (above)</sup> Bubble Chart of Average USD Fare versus Total Number of Rides Per City

>With two additional dimensional factors presented by the size and color of the bubbles, the chart is rendered that much more useful: we see that the average urban driver count is largest, followed next by that for suburban cities, and then for rural; as well, we see that the bubbles' sizes taken overall show a general negative trend for fares as the number of drivers per city goes up. Also, the city-type color information shows that while number of rides *does **not*** seem for urban cities to correlate with either higher or lower (so, no correlation) fare prices, for both suburban- and rural-type cities the more the rides *does seem* to correlate with higher fares.


  B.  Three Box-and-Whisker Plots  (chosen to show data distribution and outliers<sup>as noted in table in Module 5.1.10</sup>)
  B(1).<sup>Fig2 (above)</sup> Number of Rides for Each City Type

>Median number of city rides goes up as type goes from rural to suburban to urban, so with increasing city size the number of rides goes up as well. Note, too, that Urban-type cities have an outlier (at 39) for number of rides.	


  B(2).<sup>Fig3 (above)</sup> USD Fare for Each City Type

>Median fare for an urban-type city is lower than that for a suburban-type city which is in turn lower than that for a rural-type city,
but many of the fare values overlap for all the city types; and suburban-type cities have the lowest dispersion (most consistent) of fare amounts while rural-city fares have the highest dispersion of the fare amounts.


  B(3).<sup>Fig4 (above)</sup> Number of Drivers for Each City Type

>Number of drivers has both the lowest dispersion (most consistent), and the lowest median for rural cities; and number of drivers measurements for both median and dispersion increases with city-type population (i.e. goes up as city-type size increases). Note that, the median number of drivers for rural cities is below the 25th percentile for the next highest city type (suburban cities), the median of drivers for which is also below the 25th percentile for the next highest city type (urban cities).


  C.  Three Pie Charts (chosen to compare dataset values and show relationship of parts making up a whole category<sup>Mod 5.1.10</sup>)
>For all three pie charts (ie. C1, C2, and C3), the percentage relationship can be summarized as follows:
                       		    ***Urban  >  Suburban  >  Rural***
However, note also that although for C3 (% of Total Drivers by City Type), Rural Driver count is 2.6% but for C2 (% of Total Rides by City Type) the percentage for Rural cities -- that contribute to rural driver count -- rises to 5.3%, and again for C1 (% of Total Fares by City Type) the rural city percentage contribution rises to 6.8% of total fares.  So, the smallest percentage of overall drivers by city type (rural drivers) are contributing bigger than their representative number towards the total rides count and towards the total fares amount. This matches that the rural-type cities have the largest USD fare median value.

- C(1).<sup>Fig5 (above)</sup> Percentage of Total Fares by City Type (see notes at C. above)
- C(2).<sup>Fig6 (above)</sup> Percentage of Total Rides by City Type (see notes at C. above)
- C(3).<sup>Fig7 (above)</sup> Percentage of Total Drivers by City Type (see notes at C. above)

The observations concluded by reviewing the seven charts above were able to be identified much more quickly than would be possible by scanning through the "very large" sets of data alone. This supports the reasoning of adding annotated plots to analyses as the visualizations enable patterns, trends, and potential correlations, and outliers to be spotted at a glance. (Module 5.0.1 video)

These conclusions will be revisited for the upcoming Challenge Analysis section.


## Challenge Overview
A growing skill set with Python, Pandas and Jupyter Notebook is able to be exercised with creating an additional set of decision-making aids, which are *Challenge Deliverables*:
  - a summary DataFrame of ride-sharing data by city type <sup>(see Table 1 below)</sup>
  - a multiple-line graph of weekly total fares for each city type<sup>(Fig. 8 below)</sup>

**Table 1:** Ride-sharing DataFrame showing summary by city type ![Table 1](/Resources/Images/Screenshot_2022-07-06__ride-sharing-summary-DataFrame-by-city-type.png)


**Fig. 8:** Multi-line graph of weekly total fares for each city type ![Fig. 8](/analysis/Pyber_fare_summary.png)


### Challenge Analysis
For the ride-sharing DataFrame summary^Table 1 above^ ...
>These relationships hold for the *Totals* (i.e., Total Rides, Total Drivers, Total Fares) by city type:

                		Rural  <  Suburban  <  Urban

>Whereas the reverse relationships hold for the *Averages* (i.e. Average Fare per Ride, Average Fare per Driver) by city type:

                 		Rural  >  Suburban  >  Urban
		
For the multiple-line graph (Fig. 8 above) of weekly total fares for each city type, each city type contributes to the overall fare amount according to relative size, i.e. suburban cities in the middle between rural, which are the lowest, and urban cities, the highest.  As for the timing of the line peaks, all of the lines have a local peak in fare total amount in the last week of February, dipping notably in the first week of March.

And this is where we revisit conclusions of the analysis above...

The addition of annotated data visualizations to the analysis enables patterns, trends, and potential correlations, and outliers to be spotted at a glance (Mod 5.0.1 video). A well-designed and annotated data visualization allows an audience to absorb information quickly, engaging all viewers / stakeholders (Mod 5.0.1 video) by helping make prominent many significant data relationships in an analysis.

For instance, (whereas) considering the DataFrame table summary (Table 1 above) *number* figures alone, any pattern might be difficult to pinpoint, the chart (Fig. 8 above) depicting the total fares by city type permits a viewer to quickly compare results among the three types. According to a well-known adage: *a picture is worth a thousand words* ... or at least in this case, many thousands of rows of data. 


## Summary
Through reviewing primarily the data visualizations that accompany this analysis, an analyst may see data relationships much more readily than via solely reviewing tables of numbers. A number of recommendations may be made as a result of this analysis:

>	- If resources are to be invested, e.g. funding for additional drivers, determine which would take priority:
>	  (a) contribution to overall fare totals ==> would look to find urban drivers;
	  (b) contribution to per driver fare amounts ==> would look to hire rural drivers;
	  (c) keeping fare rates relatively steady ==> hire drivers to drive in suburban areas(vi)

>	- May want to conduct a survey or another study to determine cause for the increase in
	  fare totals for all city types ending week of February 2019.

>	- As the number of drivers is smallest and average fare rate highest for rural cities, could look to hire
	  more drivers in rural cities (regardless of first recommendation priority), as data indicates those city
	  areas may be underserved (indicated by a number of different measures).(vii, viii, ix)

>	- What is definition of rural city?  Is it by income, population density, a combination? May need to
	  fund additional or otherwise incentivize drivers in rural cities in order to provide lower fare rates
	  to riders there; may result in additional total fare

- (vi) Smallest IQR (interquartile range) - Fig. 3., and median fare in the middle (Goldilocks' baby bear?)
- (vii) Smallest IQR - Fig. 2, so number of rural rides relatively steady (less dispersion than for suburban, urban city types, may indicate room to grow there).
- (viii) Fig. 1 shows despite (or maybe since?) having low number of drivers (smallest bubbles) relative to other city types, rural cities have highest average fare (over $40 for four cities) -- *supply-demand issues?*.
- (ix) Fig. 4 (or analysis for B-3.) shows number of drivers consistent (lower IQR dispersion than other city types) for rural cities, so the fewer rural drivers relatively consistently needed for rides.


## Resources
- Data Sources: city_data.csv, ride_data.csv
- Software: Python 3.7.13, Jupyter Notebook 6.4.8, Pandas and Matplotlib 3.5.1 pyplot libraries in PythonData environment
- Coding template framework: PyBer_Challenge_starter_code.ipynb


**Notes**:
- Other students in cohort have been aiding the understanding of categorical differences between libraries (Pandas, Matplotlib pyplot), application software (Microsoft Excel, Jupyter Notebook), and APIs; e.g. Slack message notice with R Sikha on July 5, 2022.

- Using tight_layout() to produce Fig1.png as discussed during class to avoid text being cut-off when image saved to file (see code snip below)...

<img src="/Resources/Images/Screenshot_2022-07-06__Code_Snip_Tight_Layout.png" width="65%">
