### Improving Waste Sorting Efficiency in NYC using Machine Learning

**Author: Twinkle Mehta**

#### Executive summary

In this report, I will make the process of waste item classification highly efficient by leveraging an
ML model to predict Material group (Paper, Plastic, Glass, Metal, Organic, E-Waste, C&D, Special Waste, and Misc Inorganics).
I explore various models and then will identify the one which yields the highest accuracy and can be used to optimize 
classification of composite / heterogeneous waste items. 

#### Rationale
Why should anyone care about this question?

The correct sorting of waste, especially in the city of New York, is extremely valuable. Sorting waste correctly can save 
money for the city of New York as materials that could be recycled are being given a second life. If all waste were simply
put in landfills, I would waste money in re-creating materials that could have been made from recycled materials. Compost
or organic waste is also a good example of this. Compost is valuable in providing nutrients to plants and is also giving 
what seems like waste, a purpose. 

#### Research Question
What are you trying to answer?

How can we optimize the classification of complex waste items (i.e. items made up of different types of materials)? 

#### Data Sources
What data will you use to answer you question?

I am using an NYC Open Data dataset - which includes data collected from the city of New York.
Here is a link to the datasource: https://data.cityofnewyork.us/Environment/DSNY-Waste-Characterization-Citywide-Subsort/phkb-tkts

#### Methodology
What methods are you using to answer the question?
This model explores the application of various model types such as Logistic Regression, KNN, Decision Trees, and SVM and then uses hyperparameter 
optimization methods such as KFoldCV and GridSearchCV to improve the models. 

#### Results
What did your research find?
The KNN model with N=5 is the most performant overall, considering accuracy of predictions and model runtime tradeoffs.

#### Next steps
What suggestions do you have for next steps?

I would recommend making an API endpoint for this prediction model and making it available in an application for either folks
at the Waste Collection facilities in NYC to better identify if a particular waste item can be further sorted, or as a phone 
application for an end-user to scan an item and (with mapping the item to a database with its composition) my model can then 
recommend the classification of the object and, therefore, how to sort it (whether it can be recycled, composted, etc). 

#### Outline of project

- [Introduction](intro.ipynb)
- [Analysis](analysis.ipynb)
- [Results](results.ipynb)


##### Contact and Further Information
Twinkle Mehta (twinklemehta8@gmail.com)