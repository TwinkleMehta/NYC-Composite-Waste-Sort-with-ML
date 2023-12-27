### Improving Waste Sorting Efficiency in NYC using Machine Learning

**Author: Twinkle Mehta**

#### Executive summary
This report aims to increase the efficiency of waste item classification by implementing a machine learning model. The goal is to predict Material groups (Paper, Plastic, Glass, Metal, Organic, E-Waste, C&D, Special Waste, and Misc Inorganics) based on composition of an item being disposed of. Through an exploration of many models, the report will identify the most accurate model that can optimize the classification of composite or heterogeneous waste items.

#### Rationale
Why should anyone care about this question?

1. Environmental Impact: Precision in waste sorting directly contributes to reducing environmental strain. By recycling and repurposing materials, we mitigate the need for extensive resource extraction and energy-intensive production processes. This, in turn, curtails greenhouse gas emissions and lessens the burden on the natural environment. 

2. Resource Conservation: Recycling minimizes the demand for raw resources, thereby preserving forests, reducing water consumption, and lessening the strain on landfills.

3. Economic Viability: New York City, like many urban centers, faces substantial waste management costs. Enhancing sorting efficiency directly impacts municipal budgets. Diverting recyclable materials from landfills not only cuts waste disposal expenses but also presents opportunities for revenue generation through recycled material sales.

#### Research Question
What are you trying to answer?

How can we optimize the classification of composite waste items (i.e. items made up of different types of materials)? 

#### Data Sources
What data will you use to answer you question?

This analysis uses an NYC Open Data dataset. The datasource can be found here: https://data.cityofnewyork.us/Environment/DSNY-Waste-Characterization-Citywide-Subsort/phkb-tkts

#### Methodology
What methods are you using to answer the question?
This report explores the use of various models, including: Logistic Regression, KNN, Decision Trees, and SVM as well as hyperparameter optimization techniques such as KFoldCV and GridSearchCV to validate viability of and improve the models. 

#### Results
What did your research find?
The KNN model with N=5 is the most performant overall, considering accuracy of predictions and model runtime tradeoffs.

#### Next steps
What suggestions do you have for next steps?

To extend the impact of this research, I propose creating an API endpoint for the prediction model. This can be integrated into an application, enabling Waste Collection facilities in NYC to better identify and sort specific waste items. Additionally, developing a user-friendly mobile application allowing end-users to scan items would enable the model to recommend how to classify the item - whether it's recyclable, compostable, etc. — by mapping it to a composition database.

#### Outline of project

- [Introduction](intro.ipynb)
- [Analysis](analysis.ipynb)
- [Results](results.ipynb)


##### Contact and Further Information
Twinkle Mehta (twinklemehta8@gmail.com)
