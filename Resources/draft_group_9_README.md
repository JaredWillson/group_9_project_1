# Adoption of Electic Vehicles in California

## Presented by Project 1, Group 9
* Gina Barragan
* Mo Dai
* Jim Haugen
* Aram Keledkian
* Jared Wilson

## Background

## The presence of Electric Vehicles (EVs) is ubiquitous in California as Californians have adopted the use of EVs.  A recent article published on California.gov titled “California EV Sales Have Skyrocketed in the Last Decade” dated February 22, 2024 by Governor Gavin Newsom, “[o]ne in four new cars sold in California are zero-emission (battery, electric, plug-in hybrid or fuel cell electric).   More ZEVs were sold in California in 2023 than at any point in history[.]”
## Group 9 has challenged itself to make a presentation which answers the following questions:
* What is the adoption rate for usage of EVs between urban areas and rural areas?
* Do high-income level neighborhood have a higher adoption rate of EVs than middle-and lower-income neighborhoods?
* Has the adoption rate increased over the past three years?
* What impact, if any, has the end of Clean Vehicle Rebate Program application impacted the adoption rate of EVs?
* Has the increase in gas prices increased the adoption rate of EVs?   


## Data Resources
The following data sources have been employed in the project:
* Unites States Census Bureau;
* Graphical Information Systems Stack Exchange (Geo-Data);
* California Department of Motor Vehicle (DMV);
* California Alternative Fuels Data Center; and
* California Energy Commission.

There are two API calls contained within the notebook that will require API keys. To receive a key for collectapi.com, go to collectapi.com, choose to “sign in” using the menu option at the top of the screen. Then, you can create an account sing an email and password. Once your account is created, you can retrieve your key by navigating to account/profile and clicking on the API token tab. This key is used for learning about gas prices over time. To receive a key for the US Census API, navigate to https://api.census.gov/data/key_signup.html and request a key. You will receive it via email. The variable names for the two keys are collect_api_key and census_api_key. These should be stored in a config.py file in the same working directory as the Jupyter notebook. You will also need to have installed Pypi census and Pypi us using "pip install census" and "pip install us".

### Adoption Rate for Usage of EVs between Urban Areas and Rural Areas
Firstly, Unites States Census Bureau data sets were employed from which two data frames were defined with the following parameters.
* First data frame: County, Zip Code, Year, Population, Household Income, State, and City.
* Second data frame: County, Year, Population, and Household Income.
Both data frames were made available for use by all contributors.  Th second data frame would be employed to answer this question presented.

Secondly, geographic areas comprised of area (square miles) and density were added to the second data frame so that urban and rural areas are defined by counties.

Thirdly, DMV data was merged into second data frame so that vehicles are defined as being in either a urban area or rural area.   

Fourthly, DMV data was merged into second data frame so that vehicles are defined as being in either a urban area or rural area.   

Fifthly, the second data frame was aggregated to prepare the data for a visualization.

Lastly, the visualization was generated:

Total California EV Car Registrations, Urban and Rural, were plotted to present a time series of car registrations for urban and rural areas



### Adoption Rates of High-Income, Middle-Income, and Lower-Income Neighborhoods 

An analysis of average scores per school spending indicates a clear inverse proportional relationship between the two.  The overall average passing rate of 90.37% was enjoyed by those schools spending less than $585 per student, a rate of 81.41% for schools spending $585-$630 per student, a rate of 62.86% for schools spending $630-$645, and 53.53% for schools spending more than $645 per student.   

Given these metrics, it may be concluded that (1) charter schools outperform district schools when measured by math scores, reading scores, and a combined math and reading scores, and (2) the amount of spending per student does not reflect a better result in better math, reading, and a combined math and reading scores. 

It should be noted that the preceding conclusions are based on a very minimal amount of metrics.  The ability to attend charter schools could be determined as a function of a family’s ability to pay tuition.  Measurements inclusive of a family’s income level for each student as well as the addresses and zip codes of the student’s home could indicate neighborhoods that could be characterized as low-, middle-, a high-income neighborhoods which could indicate an ability to pay tuition. 

![Adoption by Income Level](Resources/EV_Income.png)