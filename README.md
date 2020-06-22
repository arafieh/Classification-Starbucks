### Starbucks Capstone Project

This is my Capstone Project for Udacity's Machine Learning Engineer Nanodegree. Project use some Machin Learning algorithms to predict customer responce on campain marketing (specially different offer sent to customers).

#### Contents

1. [Installation](#installation)
2. [Project Overview](#project)
3. [File Descriptions](#filedes)
4. [Results Summary](#result)

<a id='installation'></a>
#### 1. Installation

To recreate this project you will need:
- Python 3.7 or above
- The following Conda and Pip files:

`conda install --file conda_requirements.txt`

`pip install pip_requirements.txt`

<a id='project'></a>
#### Project Overview

Udacity partnered with Starbucks to provide a real-world business problem and simulated data mimicking their customer behavior. This project is focused on tailoring the personalized offers sent as part of the Starbucks Rewards Program to the customers who are most likely to use them. The Machine Learning terminology for this is "propensity modeling".

We want to determine which kind of offer, if any, to send to each customer based on their purchases and interaction with the previously sent offers. Some customers do not want to receive offers and might be turned off by them, so we want to avoid sending offers to those customers.

<a id='filedes'></a>
#### File Descriptions

- **conda_requirements.txt** - The Conda packages required to run this program.
- **data/portfolio.json** - This was provided by Starbucks and contains the information about the offers. There are a total of 10 offers.
- **data/profile.json** - This was provided by Starbucks and contains demographic information about the customers. There are a total of 17,000 customer profiles.
- **data/transcript.json** - This was provided by Starbucks and contains information about a customer's purchases and their interaction with the offers. There are 306,534 events recorded.
- **pip_requirements.txt** - The Pip packages required to run this program.
- **starbucks proposal.pdf** - Initial proposal for this project.
- **Starbucks Final report.pdf** - Final report on this project.
- **Starbucksfinal.ipynb** - The Jupyter Notebook containing all data exploration, wrangling, model building, model improvement, and the results.

<a id='result'></a>
#### Results Summary

In project used 4 different classification models. following table shows their results:

| Models                 |**Accuracy**|**F1 Score**|**Improvement Model**|
|:-----------------------|:--------:|:--------:|:-----------------:|
|**Logistic regression** |          |          |                   |
|liblinear               |0.5573239 |0.5684475 |                   |
| lbfgs                  |0.5090369 |0.5102536 |                   |
| newton-cg              |0.6565956 |0.6610901 |                   |
| saga                   |0.3968168 |0.3974635 |                   |
| sag                    |0.4014027 |0.3999820 |                   |
|**GaussianNB**          |0.6118154 |0.6125202 |                   |
|**Decision Tree**       |**0.6679255**| 1.0   |***0.7178***       |
|**Support Vector Machine**|0.6679255|0.3630149|                   |
