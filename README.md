# Multi-platform streaming service

Users from a streaming company can watch streams from both its app and website. We are given a dataset containing the following user information:
- ``Time on App``: average time spent on application, in hours/week;
- ``Time on Website``: average time spent on the website, in hours/week;
- ``Length of Membership``: how long a client is subscribed to service, in years;
- ``Yearly Amount Spent``: average yearly expenditure, in dollars.

Understanding that the company wants to take action on maximizing profits, some questions arise from the dataset:
- Is the length of membership important?
- Should the company focus its investments on the app or the website?
- What other insights should be taken into consideration?

# Contents

The [dataset](userInformation.csv) contains 500 non-null observations of the 4 user features. You can find the complete exploratory data analysis (EDA) notebook [here](multi_plataform.ipynb).

I also used the same dataset to explore _Spark_ functionalities from reading and modifying the dataset to proposing a linear regression model. You can find this reference notebook [here](pyspark_exploration.ipynb).

# Libraries

Solving the question:

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original-wordmark.svg" width="60" height="60"/> <img src="https://seaborn.pydata.org/_images/logo-tall-lightbg.svg" width="60" height="60"/> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" width="60" height="60"/> <img src="https://www.statsmodels.org/dev/_images/statsmodels-logo-v2.svg" width="60" height="60"/>

Learning a new technology:

<img src="https://upload.wikimedia.org/wikipedia/commons/f/f3/Apache_Spark_logo.svg" width="60" height="60"/>

# Conclusion

By analyzing the given data, one can arrive at the following conclusions, followed by some suggestions that might increase revenue:
- `Length of membership` is an important feature when determining `Yearly Amount Spent`. It implies that if the company had to focus on either creating new customers or retaining customers, the latter would be advisable because long-time users spend more on the service. On the same note, it might be interesting to display more advertisements for the same population strata.
- The company should focus its investments on the app, seem that `Time on App` has a much stronger correlation to our target.