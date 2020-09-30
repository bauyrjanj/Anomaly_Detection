# Anomaly Detection in Time Series Sensor Data

## Problem Identification

#### Problem Statement: 
 XYZ company operates a manufacturing plant and makes household cleaning supplies such as detergents, shampoo etc. for over 50 customers across 4 different countries with the revenue of USD800 million per year. Their operations heavily depend on over 30 industrial pumps across their manufacturing plant to make their products. In the last 6 months, one of their pumps failed 7 times unexpectedly resulting in an estimated USD500,000 in production loss and additional USD300,000 in environmental damage due to the spilled toxic chemicals.  To avoid this problem in the future, they want to be able to detect anomalies in the pump behaviour and be able to stop the pump before it goes down hard.
        
#### Context:

 Manufacturing industry is considered a heavy industry in which they tend to utilize various types of heavy machinery such as giant motors, pumps, pipes, furnaces, conveyor belts, haul trucks, dozers, graders, and electric shovels etc. These are often considered as the most critical assets for their operations. Therefore, the integrity and reliability of these equipment is often the core focus of their Asset Management programs.
The prime reason why they care so much about these assets is that the failure of these equipment often results in production loss that could consequently lead to loss of hundreds of thousands of dollars if not millions depending on the size and scale of the operations. So this is a pretty serious deal for a Maintenance Manager of a manufacturing plant to run a robust Asset Management framework with highly skilled Reliability Engineers to ensure the reliability and availability of these critical assets.
Therefore, the ability to detect anomalies in advance and be able to mitigate risks is a very valuable capability which further allows to prevent unplanned downtime, unnecessary maintenance (condition based vs mandatory maintenance) and will also enable more effective way of managing critical components for these assets. The production loss from unplanned downtime, the cost of unnecessary maintenance and having excess or shortage of critical components translate into serious magnitudes in terms of dollar amount.


#### Criteria For Success:
A model that detects the anomalies with at least 75% accuracy and generalizes well on other samples with zero rework.

#### Scope of the Solution Space:
 The scope of this project is limited to detecting anomalies in the 53 sensors of the selected pump and excludes other pumps and predicting the failures of the pump. 

#### Contraints:
 Data set is limited to the sensor readings from a single pump hence may not be the best representation of all the pumps. Computing power might become a constraint for effectively visualizing all 53 features at the same time.

#### Stakeholders:
Samwell Tarly - Maintenance Manager of the XYZ Company

#### Data:
 The data set is sourced from https://www.kaggle.com/nphantawee/pump-sensor-data and consists of 51 numerical features 
    and a categorical label. 51 numerical features contain raw sensor readings from 51 different sensors that are used to 
    do condition monitoring of the pump.The label contains string values that represent normal, broken and recovering 
    operational conditions of the pump. The data set represents 219,521 readings from 51 sensors.   

#### Solution Approach: 

   I will first build a benchmark model using IQR technique and then I will implement two other unsupervised learning algorithms to compare their resulting performances and accuracies. In doing so, I will follow the following steps:

* Data sourcing and loading

* Data wrangling

* Exploratory Data Analysis (EDA)

* Pre-Processing and Feature Engineering

* Modeling

* Model Evaluation


#### Project Deliverables: 

* Final Project Report

* Final Presentation

* Jupyter Notebook that contains all of the Python code
 
* Published article on TowardsDataScience (https://towardsdatascience.com/anomaly-detection-in-time-series-sensor-data-86fd52e62538)


==============================

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
=======
# Capstone_Anomaly_Detection
>>>>>>> 4ed2992ddb94425c083c25f709cad1588586ff42
