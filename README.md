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

![income](https://user-images.githubusercontent.com/75660704/152497122-a55c36ad-5934-4399-b9fb-88fcd3a6a366.png)

# API KEY
AHPTB9MrzpzzgKRZ24IUBWEZvqsa32zXE/pQbBLgQLI2cLrPO2CLQSoiwi14SufMHETMCgwnCYZKjZZtX5WZJQ==

# Predictive Experiment (Testing)
https://studio.azureml.net/Home/ViewWorkspaceCached/03ae087c6dcd412eb60eff9a968a34c9?#Workspaces/WebServiceGroups/WebServiceGroup/80b8ces92125fdc4f54b3903d3933007b7b/dashboard

![income1](https://user-images.githubusercontent.com/75660704/152497649-42c4ab9f-b420-4aa2-bf2e-63f2e69912f6.png)

![income2](https://user-images.githubusercontent.com/75660704/152497762-bce14a83-42f5-40fb-807c-bcd4045dd0ea.png)

![income3](https://user-images.githubusercontent.com/75660704/152497890-057a2cf3-dcaf-4151-b379-76d77b0ca673.png)

# Project IDE
Visual Studio Code is used to work this model.

![income4](https://user-images.githubusercontent.com/75660704/152498199-5f007f33-4365-437b-bcca-1b1f909d5fa4.png)

# Consumption details in Web Services:
https://services.azureml.net/workspaces/03ae087c6dcd412eb60eff9a968a34c9/webservices/80b892125fdc4f54b3903d3933007b7b/endpoints/default/consume

# Azure AI Gallery
Final deployment of the project is save in Azure AI Gallery.
https://gallery.azure.ai/Experiment/Income-Predictor-2








