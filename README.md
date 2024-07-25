![image](https://github.com/user-attachments/assets/e36ed800-c6c2-4f10-8607-b22db28085ee)![image](https://github.com/user-attachments/assets/d9b520ee-6500-4012-8a04-020c3c1124c2)# Prediction of Covid-19 and its impact on Humanity. 
## OVERVIEW: 
 
Coronaviruses (CoV) are a large family of viruses that cause illnesses ranging from the common cold to more severe diseases. A novel coronavirus (nCoV) is a new strain that has not been previously identified in humans. 	 
Coronaviruses occur when one of the following occurs:

    •	COVID‑19 transmits when people breathe in air contaminated by droplets and small airborne particles containing the virus. 
    •	When people have less immunity system. 
    •	Observed more in people who are already diagnosed with other diseases such as respiratory system. 
 
Coronavirus disease 2019 (COVID 19) is a spreading ailment caused by severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2). The first known case was identified in Wuhan, China, in December 2019. The disease has since been transmitted worldwide, leading to an ongoing pandemic.  
Symptoms of COVID‑19 are variable, but often include: 

    •	Fever, cough, headache, fatigue, breathing difficulties, loss of smell and taste. 
    •	Symptoms may begin one to fourteen days after exposure to the virus.  
  
At least a third of people who are infected do not develop noticeable symptoms. Of those people who develop symptoms noticeable enough to be classed as patients:

    •	Most (81%) develop mild to moderate symptoms (up to mild pneumonia), 
    •	while 14% develop severe symptoms (dyspnoea, hypoxia, or more than 50% lung involvement on imaging),  
    •	5% suffer critical symptoms (respiratory failure, shock, or multi-organ dysfunction). 
 Older people are at a higher risk of developing severe symptoms. Some people continue to experience a range of effects (long COVID) for months after recovery, and damage to organs has   been observed. 

 ## Approach:
 1.RoadMap
 2.Data Extraction
 3.Data Cleaning
 4.Exploratory Data Analysis
 5.Pre-processing/Feature Engineering 
 6.Statistical Findings 
 7.Feature Selection 
 8.Evaluate and deploy Model 

 ## Problem understanding 
Model prediction for Total cases w.r.t. total test 
 
     o Analysis of total tests done and out of which confirmed cases have been discovered. 
Impact of Vaccination on the severity of COVID 19 pandemic 

    o Global vaccine development efforts have been accelerated in response to the devastating COVID-19 pandemic. 
      We evaluated the impact of a 2-dose COVID-19 vaccination campaign on   
      reducing the incidences, hospitalizations, and deaths.
## Proposed solution to the problem 
1.  The Dataset represents 2 years (2020-2022) of covid-19 data of the entire world. 
2.  It includes over 66 features representing the impact of covid-19 on human lives. 
3.	Impact of covid-19 vaccination & what is the positivity rate after vaccination. 
4.	Life expectancy for the people already diagnosed with another disease. 
5.	Hospital beds availability as per ICU patients.

** Data Cleaning: 
Originally, we had trashed data, So, we had flourish data by data cleaning procedures and optimized the original data by identifying and treating 
missing values and there were outliers present in our dataset. 
Since we have 4 problems and it was identified that for some features null value treatment was required essentially.
We have replaced missing values with zeroes as replacing the same with Mean or Median won’t be appropriate.

## Explanatory Data Analysis 
We then performed Explanatory Data Analysis on the data with different scenarios as follows:

#### Total cases & Total deaths w.r.t each continent 
<img src="https://github.com/sandhyasailakshmi/Portfolio/blob/main/Dashboard%20Views/KPI%20Page.png" class="center">
Inference: 
  1.Above plot shows the total number of covid-19 positive cases against the total population for the respective Continents. 
  2	Here blue graph covers the population and the orange graph covers the total number of Covid-19 positive cases. 
  3.Asia has the highest population and Europe and Asia have more Covid cases compared to other continents.
----------
#### Total Covid positive cases against each continent covering the median of all ages 
<img src="https://github.com/sandhyasailakshmi/Portfolio/blob/main/Dashboard%20Views/KPI%20Page.png" class="center">
Inference: 
  1.In the above scatter plot median age range refers to the age group of 20-40 years. 
  2.Above plot is showing the total number of covid cases of the above-mentioned age group and we have got the insight as Africa has less population as 
    compared to other continents in our dataset but still, we can see the number of covid cases is more. 
  3.As per the plot it seems like Europe has no or very few positive cases for the people who are below the age of 35. 
-------------
#### Analysis of Total Tests, Total Cases W.R.T Population For Each Continent
<img src="https://github.com/sandhyasailakshmi/Portfolio/blob/main/Dashboard%20Views/KPI%20Page.png" class="center">
Inference:
  1.North America has done the highest number of covid diagnoses and almost covered all the covid affected people but in South America, 
    it seems like the situation is worst and one-fourth part of the total affected people has been covered for diagnosis. 
  2.Asia & Europe has done a great job in terms of covid testing. these two continents have almost covered most of the affected people. 
-------------
#### Excess mortality w.r.t each continent 
<img src="https://github.com/sandhyasailakshmi/Portfolio/blob/main/Dashboard%20Views/KPI%20Page.png" class="center">
Inference:
  1.In the above plot Excess mortality rate is higher in Africa based on population as compared to other continents as we already saw the 
    population is less in Africa than in Asia despite the mortality rate being higher in Africa. 
  2.Oceania has less population than South America but the excess mortality rate is higher in Oceania. 
--------------
#### Impact of Vaccination on the severity of COVID 19 pandemic
<img src="https://github.com/sandhyasailakshmi/Portfolio/blob/main/Dashboard%20Views/KPI%20Page.png" class="center">
Inference:
  1.Asia: 283.7 % population was covered under the vaccination drive and positive cases were 19.83 and total deaths were 20.02 %. 
  2.South America: 114 % Vaccination done, 5.03 % Covid affected population and 23.67 % total deaths occurred due to covid. 
  3.North America: 76.1 % vaccination done, 21.01% Covid affected population and 24.41% total deaths occurred. 
  4.Europe: 55.6 % vaccination done, 13.77% Covid affected population and 27.94% total deaths occurred. 
  5.Oceania: 9.5% Vaccination done, 8.52% total positive cases, and 0.05% total deaths occurred. 
  6.Africa: 4.3% total vaccinations done, 31.83% total positive cases, 3.91% deaths occurred. 
  7.Africa and Oceania have done a very a smaller number of vaccinations.
---------------
#### Life expectancy w.r.t various factors
<img src="https://github.com/sandhyasailakshmi/Portfolio/blob/main/Dashboard%20Views/KPI%20Page.png" class="center">
Inference:
  1.Oceania has more diabetic patients and it shows the life expectancy rate is lower in Oceania. 
  2.Cardiovascular diseases also affect the life expectancy rate for covid affected people. Africa has fewer cardio-related suffering people. 
  3.Africa has higher extreme poverty which also affects the life expectancy rate of the same continent. 
----------------
#### Continent Life expectancy w.r.t cardiovascular death
![image](https://github.com/user-attachments/assets/7f2baec5-876c-463c-b5cb-80e04e7d131e)

<img src="https://github.com/sandhyasailakshmi/Portfolio/blob/main/Dashboard%20Views/KPI%20Page.png" class="center">
Inference:








 

