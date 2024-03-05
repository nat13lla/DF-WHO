# Project: WHO - Life Expectancy Prediction

## Team Line Masters:
- Natalie Coyle
- Hasan Cokgezici
- George Brignell-Cash
- Iqra Finiin

## Project Overview:
The task was to provide an estimate prediction of life expectancies across countries worldwide. The dataset has been provided by the World Health Organization (WHO), containing records between 2000 and 2015 across (179) countries. 

Some of the primary focuses of this project is data integrity and ethical considerations. Several countries expressed concerns regarding sharing sensitive data, such as medical records, which could lead to unwanted financial implications and hinder social developments. As such,we were assigned to construct two models: one using the least information necessary for prediction and another more elaborate model that can be utilized if states decide to share more sensitive data.

We were asked to produce a function that takes in relevant population statistics (features) and predicts the average life expectancy. The function should prompt the user to decide which model is to be used.

## Ethical Considerations:
When creating our minimalistic model we decided to immediately remove the columns we though to be the most ‘sensitive’. In our initial assessment we focused on medical sensitivity immediately removing columns such as ‘Infant_deaths’ , ‘Under_five_deaths’  and the thinness columns. We immediately though that medical data relating to children would be the most sensitive so removed this from our model completely

Next we removed the other medical related data for example ‘Hepatitis_B’ , ‘Measles’ , ’Polio’ , ‘Diphtheria’ , ’Incidents_HIV ‘ and ‘BMI’. In terms of vaccination data, these values could be related to the varying vaccine availability across different countries and regions. Using such data to model the life expectancy could bring the ‘unwanted financial implications‘ mentioned  that we are avoiding in this simplified model.

Another note we made was that although it may not seem sensitive the alcohol consumption statistic could be seen as sensitive in some religions or for cultural reasons, so we also removed that.

From here we tried a variety of models to find the best combination of columns for our minimalistic model within our requirements. These are : Adult mortality, schooling, economy status developing 

* We considered the adult mortality to be vital to our models success - although sensitive data it was a better column to use than for example the infant deaths or other child- related data that we considered more sensitive. It was also the column that showed the highest correlation with life expectancy.
* We noted that the gdp could be considered sensitive information but trialed our models using it as we initially found that it had a strong correlation with the life expectancy in our analysis. However interestingly we found that this did not benefit the final model enough to justify using this data 

## Repository Contents:

1. **EDA_WHO-2.ipynb**: This Colab Notebook file contains the Exploratory Data Analysis (EDA) conducted on the provided dataset (life Expectancy Data.csv). It provides insights into the structure and characteristics of the data.

2. **Modelling_WHO-2.ipynb**: This Colab Notebook file contains the modeling work conducted by the team. It implements machine learning, linear regression models to predict average life expectancies across countries, including data processing, model selection, training, and evaluation.

3. **Model_Interface.ipynb**: This Colab Notebook file contains the interface for the predictive model. It prompts the user to input relevant population statistics and consent to using advanced population data for better accuracy. Based on the user's response, it selects the appropriate model and provides a prediction on the average life expectancy.

4. **life Expectancy Data.csv**: This CSV file contains the dataset provided by WHO, consisting of records between 2000 and 2015 across 183 (179) countries. It includes relevant population statistics and life expectancy measurements.

5. **WHO Dataset - MetaData.ipynb**: This Colab Notebook file contains the metadata given about the WHO dataset. It documents the features included in the dataset and their descriptions.

## Contact:
For any inquiries or concerns regarding this project, please contact Team Line Masters:
- Natalie Coyle
- Hasan Cokgezici
- George Brignell-Cash
- Iqra Finiin
