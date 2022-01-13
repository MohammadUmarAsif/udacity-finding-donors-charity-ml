
# Udacity Project: Finding Donors Charity-ML
## Nanodegree (Intro to Machine Learning with Pytorch)

### Description
Udacity project to identify potential donors for a fictitious organization (Charity-ML) using different supervised learning algorithms on the U.S. census data.

### Steps Performed -
1. Data exploration
2. Transformation of skewed continuous features
3. Normalization of numerical features
4. Data preprocessing
5. Evaluation of Naive Model's performance
6. Selection of 3 supervised-learning techniques (Decision Tree, AdaBoost, Bagging)
7. Creation of training & prediction pipeline
8. Evaluation of performance & selection of best model
9. Description of the workings of the best model
10. Tuning of the model using GridSearchCV
11. Evaluation of final model
12. Extraction of feature importance
13. Conduct feature selection and observe its effects on model performance

### Install
This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

Also requires a software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)

### Files
This project contains three files:

- `finding_donors.ipynb`: Main file with my implementation.
- `report.html`: HTML file of the ipynb notebook.
- `census.csv`: The U.S. census dataset.
- `visuals.py`: A Python file containing visualization code that is run behind-the-scenes. Do not modify.

### Code
Template code & implementation is provided in the `finding_donors.ipynb` notebook file. `visuals.py` Python file and the `census.csv` dataset file are required to complete the work. While some code has already been implemented, additional functionality is implemented where requested to successfully complete the project. Code included in `visuals.py` is meant to be used out-of-the-box and not intended for students to manipulate.

### Run
Run one of the following commands:

```bash
ipython notebook finding_donors.ipynb
```  
or
```bash
jupyter notebook finding_donors.ipynb
```

This will open the iPython Notebook software and project file in your browser.

### Data
The modified census dataset consists of approximately 32,000 data points, with each datapoint having 13 features. This dataset is a modified version of the dataset published in the paper *"Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid",* by Ron Kohavi. You may find this paper [online](https://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf), with the original dataset hosted on [UCI](https://archive.ics.uci.edu/ml/datasets/Census+Income).

**Features**
- `age`: Age
- `workclass`: Working Class (Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked)
- `education_level`: Level of Education (Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool)
- `education-num`: Number of educational years completed
- `marital-status`: Marital status (Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse)
- `occupation`: Work Occupation (Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces)
- `relationship`: Relationship Status (Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried)
- `race`: Race (White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black)
- `sex`: Sex (Female, Male)
- `capital-gain`: Monetary Capital Gains
- `capital-loss`: Monetary Capital Losses
- `hours-per-week`: Average Hours Per Week Worked
- `native-country`: Native Country (United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands)

**Target Variable**
- `income`: Income Class (<=50K, >50K)
