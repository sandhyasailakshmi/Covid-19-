# Prediction of Covid-19 and its impact on Humanity. 
## OVERVIEW: 
 
Coronaviruses (CoV) are a large family of viruses that cause illnesses ranging from the common cold to more severe diseases. A novel coronavirus (nCoV) is a new strain that has not been previously identified in humans. 	 
Coronaviruses occur when one of the following occurs:
1. COVID‑19 transmits when people breathe in air contaminated by droplets and small airborne particles containing the virus. 
2. When people have less immunity system. 
3. Observed more in people who are already diagnosed with other diseases such as respiratory system. 
 
Coronavirus disease 2019 (COVID 19) is a spreading ailment caused by severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2). The first known case was identified in Wuhan, China, in December 2019. The disease has since been transmitted worldwide, leading to an ongoing pandemic.  
Symptoms of COVID‑19 are variable, but often include: 
  1. Fever, cough, headache, fatigue, breathing difficulties, loss of smell and taste. 
  2. Symptoms may begin one to fourteen days after exposure to the virus.  
  
At least a third of people who are infected do not develop noticeable symptoms. Of those people who develop symptoms noticeable enough to be classed as patients:

   1. Most (81%) develop mild to moderate symptoms (up to mild pneumonia), 
   2. while 14% develop severe symptoms (dyspnoea, hypoxia, or more than 50% lung involvement on imaging),  
   3. 5% suffer critical symptoms (respiratory failure, shock, or multi-organ dysfunction). 
   4. Older people are at a higher risk of developing severe symptoms. Some people continue to experience a range of effects (long COVID) for months after recovery, 
      and damage to organs has been observed. 

 ## Approach:
 1. RoadMap
 2. Data Extraction
 3. Data Cleaning
 4. Exploratory Data Analysis
 5. Pre-processing/Feature Engineering 
 6. Statistical Findings 
 7. Feature Selection 
 8. Evaluate and deploy Model 

## Problem understanding 
Model prediction for Total cases w.r.t. total test 
 1. Analysis of total tests done and out of which confirmed cases have been discovered. 
Impact of Vaccination on the severity of COVID 19 pandemic 
 1. Global vaccine development efforts have been accelerated in response to the devastating COVID-19 pandemic. 
    We evaluated the impact of a 2-dose COVID-19 vaccination campaign on   
    reducing the incidences, hospitalizations, and deaths.
   
## Proposed solution to the problem 
1. The Dataset represents 2 years (2020-2022) of covid-19 data of the entire world. 
2. It includes over 66 features representing the impact of covid-19 on human lives. 
3.	Impact of covid-19 vaccination & what is the positivity rate after vaccination. 
4.	Life expectancy for the people already diagnosed with another disease. 
5.	Hospital beds availability as per ICU patients.

## Data Cleaning: 
Originally, we had trashed data, So, we had flourish data by data cleaning procedures and optimized the original data by identifying and treating 
missing values and there were outliers present in our dataset. 
Since we have 4 problems and it was identified that for some features null value treatment was required essentially.
We have replaced missing values with zeroes as replacing the same with Mean or Median won’t be appropriate.

## Explanatory Data Analysis:
We then performed Explanatory Data Analysis on the data with different scenarios as follows:

#### Total cases & Total deaths w.r.t each continent 
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Total%20cases%20%26%20Total%20deaths%20w.r.t%20each%20continent.png" class="center">
Inference:

1. Above plot shows the total number of covid-19 positive cases against the total population for the respective Continents. 
2.	Here blue graph covers the population and the orange graph covers the total number of Covid-19 positive cases. 
3. Asia has the highest population and Europe and Asia have more Covid cases compared to other continents.
  
  -------
#### Total Covid positive cases against each continent covering the median of all ages 
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Total%20Covid%20positive%20cases%20of%20all%20ages%20.png" class="center">
Inference:

  1. In the above scatter plot median age range refers to the age group of 20-40 years. 
  2. Above plot is showing the total number of covid cases of the above-mentioned age group and we have got the insight as Africa has less population as 
     compared to other continents in our dataset but still, we can see the number of covid cases is more. 
  3. As per the plot it seems like Europe has no or very few positive cases for the people who are below the age of 35. 
  
-------
#### Analysis of Total Tests, Total Cases W.R.T Population For Each Continent
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Analysis%20of%20Total%20Tests%2CCases%20W.R.T%20Population%20For%20Each%20Continent.png" class="center">
Inference:

  1. North America has done the highest number of covid diagnoses and almost covered all the covid affected people but in South America, 
     it seems like the situation is worst and one-fourth part of the total affected people has been covered for diagnosis. 
  2. Asia & Europe has done a great job in terms of covid testing. these two continents have almost covered most of the affected people. 
  
-------
#### Excess mortality w.r.t each continent 
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Excess%20mortality%20w.r.t%20each%20continent.png" class="center">
Inference:

  1. In the above plot Excess mortality rate is higher in Africa based on population as compared to other continents as we already saw the 
     population is less in Africa than in Asia despite the mortality rate being higher in Africa. 
  2. Oceania has less population than South America but the excess mortality rate is higher in Oceania. 
  
-------
#### Impact of Vaccination on the severity of COVID 19 pandemic
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Impact%20of%20Vaccination%20on%20the%20severity%20C-19.png" class="center">
Inference:

  1. Asia: 283.7 % population was covered under the vaccination drive and positive cases were 19.83 and total deaths were 20.02 %. 
  2. South America: 114 % Vaccination done, 5.03 % Covid affected population and 23.67 % total deaths occurred due to covid. 
  3. North America: 76.1 % vaccination done, 21.01% Covid affected population and 24.41% total deaths occurred. 
  4. Europe: 55.6 % vaccination done, 13.77% Covid affected population and 27.94% total deaths occurred. 
  5. Oceania: 9.5% Vaccination done, 8.52% total positive cases, and 0.05% total deaths occurred. 
  6. Africa: 4.3% total vaccinations done, 31.83% total positive cases, 3.91% deaths occurred. 
  7. Africa and Oceania have done a very a smaller number of vaccinations.
  
--------
#### Life expectancy w.r.t various factors
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Life%20expectancy%20w.r.t%20various%20factors.png" class="center">
Inference:

  1. Oceania has more diabetic patients and it shows the life expectancy rate is lower in Oceania. 
  2. Cardiovascular diseases also affect the life expectancy rate for covid affected people. Africa has fewer cardio-related suffering people. 
  3. Africa has higher extreme poverty which also affects the life expectancy rate of the same continent.
  
--------
#### Continent Life expectancy w.r.t cardiovascular death
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Continent%20Life%20expectancy%20w.r.t%20cardiovascular%20death.png" class="center">
Inference:

 1. From the plot mentioned above, we can infer that the cardiovascular death rate is inversely proportional to the life expectancy of Covid affected people. 
 
--------
#### Life expectancy w.r.t diabetes prevalence 
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Life%20expectancy%20w.r.t%20diabetes%20prevalence.png" class="center">
Inference:

 1. If the diabetes prevalence is between 5 to 15 the life expectancy can be seen between 70 to 85. 
 2. We can see that as per continent the life expectancy for diabetes prevalence changes.
 
--------
#### Availability of Hospital Beds w.r.t Total ICU Patients 
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Availability%20of%20Hospital%20Beds%20w.r.t%20Total%20ICU%20Patients%20.png" class="center">
Inference:

 1. Availability of beds in Europe is 23.78 % but total ICU patients is 48.38% which is quite a higher number. 
 2. In North America is also the same as Europe and even worse as 15% of total beds availability and 49.12% of 
    ICU patients were there which is the worst scenario for the continent. 

-------
## Base Model
#### Total Cases w.r.t Total Tests 
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Total%20Cases%20w.r.t%20Total%20Tests%20.png" class="center">
Inference:

  1. The value of Durbin-Watson test is 2.007. It signifies that there is no auto-correction. 
  2. As the CN (Condition Number) Value are 6.12. We can say that there is no no-multicollinearity. 
  3. Adj. R Square Value is 0.76 or 76% we can say that 76% Model is Correct
  
 -------
#### Availability of ICU Beds and Hospital Beds
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Availability%20of%20ICU%20Beds%20and%20Hospital%20Beds.png" class="center">
Inference:

  1. The value of Durbin-Watson test is 1.990. It signifies that there is no auto-correction as the value is near to 2. 
  2. As the CN (Condition Number) Value are 5.33. We can say that there is no-multicollinearity as the value is less than 100. 
  3. Adj. R Square Value is 1005 we can say that Model is over fitted because R-Square Value is 1. The value 1 tells us that the Model is over fitted. 
  4. Also, all the P- values are less than 0.05 
  
 -------
#### Impact of Vaccination on the severity of COVID 19 pandemic 
## Moedel Before Transformation
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Impact%20of%20Vaccination%20on%20the%20severity%20of%20COVID%2019%20pandemic%20(before).png" class="center">
Inference:
 
  1. The value of Durbin-Watson test is 1.988. It signifies that there is no auto-correction as the value is near to 2. 
  2. As the CN (Condition Number) Value are 8.63. We can say that there is no-multicollinearity as the value is less than 100.   
  3. Adj. R Square Value is 1% we can say that Model is over fitted because R-Square Value is 1. The value 1 tells us that the Model is overfitted.
  
## Model After Tramformation
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Impact%20of%20Vaccination%20on%20the%20severity%20of%20COVID%2019%20pandemic%20(after).png" class="center">
Inference:
 
  1. The previous model was over fitted. 
  2. Now in this model we can see that this model is preforming better. 
  3. The value of Durbin-Watson test is 2.002. It signifies that there is no auto-correction as the value is near to 2. 
  4. As the CN (Condition Number) Value are 3.64. We can say that there is no-multicollinearity as the value is less than 100. 
  5. Adj. R Square Value is 0.134 we can say that Model is best fitted because R-Square Value is 0.134. The value 0.134 tells us that the Model is best or normally fitted. 
  
-------
#### Impact of Vaccination on the severity of COVID 19 pandemic
## Model with Logistic regression
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Impact%20of%20Vaccination%20on%20the%20severity%20of%20COVID%2019%20pandemic%20(LR).png" class="center">
Inference:

  1. Pseudo R-square value is 0.072  
  2. Log-Likelihood is the maximum value of the log-likelihood function. 
  3. LL-Null is the maximum value of the log-likelihood. 
  4. The LLR p-value is less than 0.05, implies that the model is significant.
  
## Model after performing recursive feature elimination
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Impact%20of%20Vaccination%20on%20the%20severity%20of%20COVID%2019%20pandemic%20(LR-RFE).png" class="center">
Inference:

  1. The LLR p-value is greater than 0.05, implies that the model is not significant. 
  2. Pseudo R-square value is -0.3898 negative, so this model is not a good fit model.
  
-------

#### Model Metrics
<img src="https://github.com/sandhyasailakshmi/Covid-19-/blob/main/widget%20views/Model%20metrix.png" class="center">
Inference:

  1. For Decision Tree the Accuracy is 0.98, ROC-Score is 0.97, Precision is 0.960, F1-Score is 0.95, and Recall value is 0.95. 
  2. For Random Forest the Accuracy is 0.98, ROC-Score is 0.97, Precision is 0.967, F1-Score is 0.96, and Recall value is 0.95. 
  3. For Adaboost the Accuracy is 0.82, ROC-Score is 0.60, Precision is 0.63, F1-Score is 0.34, and Recall value is 0.23. 
  4. For Gradient boost the Accuracy is 0.86, ROC-Score is 0.64, Precision is 0.82, F1-Score is 0.52, and Recall value is 0.38. 
  5. For XgBoost the Accuracy is 0.85, ROC-Score is 0.63, Precision is 0.85, F1-Score is 0.42, and Recall value is 0.28. 
  6. There was overfitting in our model as we can see that from decision tree and random forest by using ensembled techniques like Adaboost, 
     Gradient and XGboost we dealt with accuracy   paradox and overfitting among the ensembled techniques w.r.t to gradient boosting we got 
     better accuracy compared to other ensembled techniques. 
















 

