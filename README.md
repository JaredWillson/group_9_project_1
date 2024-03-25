# group_9_project_1
## Project Title and Summary Statement
This repo contains analysis of the California EV market for the years 2020 to 2022 including census data, DMV registration data, historical California gas prices, and the buildout of public infrastructure (charging stations) to support the use of electric vehicles. Authors of the project are Gina Barragan, Mo Dai, Jim Haugen, Aram Keledjian, and Jared Willson. The intent of the analysis is to determine the current adoption rate of EV's within California, how that adoption rate is changing over time, whether that adoption rate is different for urban vs rural geographies, whether that adoption rate varies by household income level, whether the buildout of infrastructure to support EV's is matching the adoption rate, and whether EV adoption rate correlates with fluctuations in gas prices.

The Jupyter notebook containing all analysis is called Group_9_submission.ipynb

There are two API calls contained within the notebook that will require API keys. To receive a key for collectapi.com, go to collectapi.com, choose to “sign in” using the menu option at the top of the screen. Then, you can create an account sing an email and password. Once your account is created, you can retrieve your key by navigating to account/profile and clicking on the API token tab. This key is used for learning about gas prices over time. To receive a key for the US Census API, navigate to https://api.census.gov/data/key_signup.html and request a key. You will receive it via email. The variable names for the two keys are collect_api_key and census_api_key. These should be stored in a config.py file in the same working directory as the Jupyter notebook. You will also need to have installed Pypi census and Pypi us using "pip install census" and "pip install us".

## Questions To Be Answered by the Analysis
- What is the adoption rate for EV in both urban vs rural areas? 
- Do higher income neighborhoods have a higher adoption rate vs middle and lower income neighborhoods? 
- How has the adoption rate changed over the last 3 years in California compared to other types of vehicles?
- Are charging stations increasing at the same rate as the EV adoption rate?
- Is there a correlation between EV adoption rate and gasoline prices?

## Results

![Overall Califoornia Adoption(Resources/Car_Registrations_Urban_v_Rural.png)

We found that, while there is some difference in adoption rates between urban and rural counties, the differences were quite small and were diminishing. On average over the three year period, rural counties lagged by just 7% vs. urban counties and that gap had decreased to 4% as of 2022. 

![Adoption by Income Level (Resources/EV_Income.png)

We also found that adoption rates were significantly higher in the top quartile of household income and were extremely low in the lowest quartile. This is likely due to a combination of factors including higher prices for new EV vehicles, and the relative scarcity of used EV's at the present time.
