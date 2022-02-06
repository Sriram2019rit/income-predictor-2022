# Income Predictor 

# Aim
To deploy income predictor model using Azure ML.

# Summary of the Model
As our predictive method we will use logistic regression, which is a binary classification algorithm.

# Description of the Model
Many businesses would like to personalize their offer based on customer’s income. High-income customers could be, for instance, exposed to premium products. As a customer’s income is not always explicitly known, predictive model could estimate income of a person based on other information. Our goal is to create a predictive model that will be able to output a single decision - i.e. whether the income of given person exceeds 50k per year - based on other information about the individual. First, we will split our dataset into two parts - training set and validation set. Then, we will train a logistic regression model on samples from the training set and finally evaluate its accuracy based on validation dataset.

# Attribute Description
1)	age: continuous.
2)	workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.
3)	fnlwgt: continuous.
4)	education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.
5)	education-num: continuous.
6)	marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.
7)	occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.
8)	relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.
9)	race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.
10)	sex: Female, Male.
11)	capital-gain: continuous.
12)	capital-loss: continuous.
13)	hours-per-week: continuous.
14)	native-country: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands.

# Description of Final Weight
The weights on the CPS files are controlled to independent estimates of the civilian noninstitutional population of the US.  These are prepared monthly for us by Population Division here at the Census Bureau.  We use 3 sets of controls. These are:
1.  A single cell estimate of the population 16+ for each state.
2.  Controls for Hispanic Origin by age and sex.
3.  Controls by Race, age and sex.
We use all three sets of controls in our weighting program and "rake" through them 6 times so that by the end we come back to all the controls we used.
The term estimate refers to population totals derived from CPS by creating "weighted tallies" of any specified socio-economic characteristics of the population.
People with similar demographic characteristics should have similar weights.  There is one important caveat to remember about this statement.  That is that since the CPS sample is actually a collection of 51 state samples, each with its own probability of selection, the statement only applies within state.

# Azure Machine Learing (Studio)
Azure ML Studio is used as Web Portal.

# Algorithm
This model follows an algorithm called "logistic regression", it predicts multiple linear regression.

![azure](https://user-images.githubusercontent.com/75660704/152693054-93c44625-45cc-47cb-b688-de4dcd383f57.png)

# API KEY
AHPTB9MrzpzzgKRZ24IUBWEZvqsa32zXE/pQbBLgQLI2cLrPO2CLQSoiwi14SufMHETMCgwnCYZKjZZtX5WZJQ==

# Predictive Experiment (Testing)

![azure1](https://user-images.githubusercontent.com/75660704/152693205-12e4422a-a0cf-493c-aabe-054b511b2b4d.png)

![azure5](https://user-images.githubusercontent.com/75660704/152693311-fda2b10a-90a0-4871-a24e-12e59f06b89a.png)

![azure6](https://user-images.githubusercontent.com/75660704/152693425-55624854-f1eb-46a4-b840-792a1d52e7aa.png)

# Data Collected

![azure2](https://user-images.githubusercontent.com/75660704/152693544-b8101b66-b97a-4b81-8ff0-336756d73f7e.png)

![azure3](https://user-images.githubusercontent.com/75660704/152693616-773d8fa6-a286-4c17-b91d-f8d4cdc756c3.png)

# Project IDE
Visual Studio Code is used to work this model.

![azure4](https://user-images.githubusercontent.com/75660704/152693658-cae463b4-4e70-4470-a333-bc3c0dd0a64b.png)

# Azure AI Gallery
Final deployment of the project is save in Azure AI Gallery.
https://gallery.azure.ai/Experiment/Income-Predictor-2








