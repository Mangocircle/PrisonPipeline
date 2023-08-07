# Investigating the Prison Pipeline
## Understanding the Factors Influencing Arrests and Policing Disparities in Lancaster, CA

## Contributors
* Adina Raizen
* Henry Luken
* Patrick Aubry 

## Introduction
The main goal of this project is to investigate the factors that influence policing and incarceration, with a particular focus on the city of Lancaster, CA. The project aims to explore the prison pipeline and understand why certain demographics, especially Black men in their 20s and 30s, are disproportionately affected by encounters with police and subsequent arrests. By examining relevant data and leveraging machine learning, the project seeks to develop a predictive model that can determine the likelihood of an individual's arrest based on basic demographics.

By shedding light on the factors influencing arrests and policing disparities in Lancaster, CA, this project aims to raise awareness about systemic issues and contribute to evidence-based policy-making. The findings and predictive model can be used to guide law enforcement practices, promote social justice, and develop intervention strategies aimed at reducing incarceration rates and fostering a fairer criminal justice system.

## Methodology
The project focuses on Lancaster, CA, examining data related to police encounters and arrests. Factors that were considered include race, gender, homelessness, and disability. 

The primary data source used is the 2019 [Los Angeles County Sheriff’s Deputy Contacts in Lancaster dataset](https://www.propublica.org/datastore/dataset/los-angeles-county-sheriffs-deputy-contacts-in-lancaster) from propublica.org. Additional demographic data was pulled from (**ADD SOURCE!**).

This project is comprised of two parts:
1. Data Analysis
2. Predictive Model

### Data Analysis
First, the dataset was analyzed to find patterns and themes related to the factors that are involved in the outcomes of police interactions. Tableau was used to create visualizations demonstrating these themes. The data regarding police encounters in Lancaster, CA was combined with demographic information from the city in order to draw additional conclusions about disparities in policing.

### Predictive Model
Next, machine learning models were applied to the police encounters data in an effort to create a predictive model. In order to do this, the data was first cleaned, maintaining fields with demographic information and combining fields to create a target field indicating whether an encounter resulted in an arrest. 

Several types of models were tested, including logistic regression, random forest, and neural network. Each model was analyzed for accuracy, with each model maxing out around 62% accuracy overall. A great deal of testing was employed when designing the neural network, including trying various combinations of numbers of neurons and layers, types of activation layers used, drop-out rates, and optimizer types. 

In the process of model optimization, various manipulations of the data were tested as well, including binning ages into groups of 5-year spans, binning gender and race categories to simplify the data, and removing the disability category. Through trial and error, the group incorporated the changes that led to the highest accuracy of the model, taking care to not over-fit the model to the data. 

Once the most optimized model was found, using a Keras sequential neural network model in TensorFlow, an app was created using Python to allow a user to input several demographics and receive a result indicating whether they are likely or unlikely to be arrested in Lancaster, CA following an encounter with the police.

## Current Conclusion
In analyzing the data, several themes emerge:

(**ADD HERE, WITH VISUALIZATIONS**)

Additionally, using machine learning, a predictor app was created that predicts whether a person is likely to be arrested if they encounter the police, based on demographic information provided. While the model was only able to achieve about 62% accuracy, a more accurate app could be developed in the future with more data. (**ADD SOMETHING HERE ABOUT THE RECALL/PRECISION STATS AND WHY IT'S MORE IMPORTANT TO HAVE FALSE POSITIVES THAN FALSE NEGATIVES?**)

## Future State
Moving forward, the group aims to expand this analysis to encompass the entire incarceration process. This includes investigating the factors that increase an individual's likelihood of being incarcerated and understanding the drivers of recidivism. The objective is to create a comprehensive model that highlights the complexities of the criminal justice system, with a focus on addressing and mitigating disparities and systemic biases.
