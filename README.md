# Predicting Churn for Banks

*Binary Classification Using Tree-Based ML Methods*

<img src="always_has.png" alt="alt text" width="745" height="400">

### Project Summary

This client churn project consists of a binary classification model that predicts which bank customers are likely to exit.  Knowing it is generally more expensive to acquire a new customer than retain an existing one, the ultimate goal is to prevent churn by providing the bank with a list of at-risk customers. The model itself showcases tree-based methods like decision trees, random forests, and includes boosting methods such as AdaBoost and XGBoost. Additionally, there is a Deployment section that dicusses a few practicle MLOps ideas.  Finally, there is Business Value-Add section that covers cost savings and real world implications.

### Data Source

The following client churn data contains 11 feature columns and 1 target column, "Exited."  It can be found at:

https://www.kaggle.com/datasets/mathchi/churn-for-bank-customers


* churn.csv: Client churn data for bank customers. Contains variables:

    * CustomerId: contains random values and has no effect on customer leaving the bank
    * Surname: the surname of a customer has no impact on their decision to leave the bank.
    * CreditScore: can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank.
    * Geography: a customer’s location can affect their decision to leave the bank.
    * Gender: it’s interesting to explore whether gender plays a role in a customer leaving the bank.
    * Age: this is certainly relevant, since older customers are less likely to leave their bank than younger ones.
    * Tenure: refers to the number of years that the customer has been a client of the bank. Normally, older clients are more loyal and less likely to leave a bank.
    * Balance: also a very good indicator of customer churn, as people with a higher balance in their accounts are less likely to leave the bank compared to those with lower balances.
    * NumOfProducts: refers to the number of products that a customer has purchased through the bank.
    * IsActiveMember: active customers are less likely to leave the bank.
    * EstimatedSalary: as with balance, people with lower salaries are more likely to leave the bank compared to those with higher salaries.
    * Exited: whether or not the customer left the bank.

### Installation Prerequisites

  ```import random
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn import tree
import xgboost as xgb
from xgboost import XGBClassifier, plot_tree
from sklearn.tree import DecisionTreeClassifier
from imblearn.ensemble import BalancedRandomForestClassifier
from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
from sklearn.model_selection import train_test_split, StratifiedKFold, GridSearchCV
from sklearn.metrics import confusion_matrix, classification_report, ConfusionMatrixDisplay, make_scorer
  ```

### Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### License
Distributed under the MIT License. See `LICENSE.txt` for more information.

### Contact

Cole Fairbanks

* [Cole's Personal Website & Portfolio](https://colefairbanks.com)
* [Connect with Cole on LinkedIn](https://linkedin.com/in/colefairbanks/)
* [Cole's Github Repos](https://github.com/colefairbanks?tab=repositories)

© 2023 GitHub, Inc.
