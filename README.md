# RoboAdvisor - A Portfolio Selection Recommendation System
A portfolio selection recommendation system based on Markowitz Mean-Variance Model and Black-Litterman Model implemented on the App "Navigator".

This is my first practical project during my internship at Asset Pro in Beijing. And the project is already implemented on the "Navigator" financial APP with thousands of users.


## About
Here are the presentation slides for the whole project.

>[RoboAdvisor - Presentation Slides](https://github.com/PeterQiu0516/RoboAdvisor/raw/master/01_13/%E5%9F%BA%E4%BA%8EMarkowitz%20Mean-Variance%E4%B8%8EBlack-Litterman%E7%90%86%E8%AE%BA%E7%9A%84%E8%B5%84%E4%BA%A7%E9%85%8D%E7%BD%AE%E6%A8%A1%E5%9E%8B%E2%80%94%E2%80%94%E6%9C%AA%E6%9D%A5%E8%88%AA%E6%B5%B7%E5%AE%B6RoboAdvisor%E6%96%B0%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D.pdf)

You may also take a glance at the sample portfolio report generated by the Roboadvisor.

>[Sample Portfolio Report - Risk Level 5 (most aggressive strategy, for risk-loving customers)](https://github.com/PeterQiu0516/RoboAdvisor/raw/master/Sample%20Portfolio%20Report%20-%20Risk%20Level%205.pdf)

>[Sample Portfolio Report - Risk Level 3 (neutral strategy, for risk-neutral customers)](https://github.com/PeterQiu0516/RoboAdvisor/raw/master/Sample%20Portfolio%20Report%20-%20Risk%20Level%203.pdf)

>[Sample Portfolio Report - Risk Level 1 (most convervative strategy, for risk-averse customers)](https://github.com/PeterQiu0516/RoboAdvisor/raw/master/Sample%20Portfolio%20Report%20-%20Risk%20Level%201.pdf)

### Programming Languages
***
>+ **Python 3**: For model implementation `(PyPortfolioOpt)` online data crawling `(selenium)`, project integrating `(rpy2)` and data processing `(pandas)`.
>+ **R**: For model implementation `(PortfolioAnalytics)` and online data crawling `(rvest)`.
>+ **Javascript**: For plotting related intuitive financial figures `(ECharts)` and online survey designing.
>+ **Html**: For online survey designing.

### Building
---

**Warnings: The repositories is still being uploaded to pip and now you can only use Method 2.**

#### Method 1:
>In terminal, run

```
pip install RoboAdvisor
```

#### Method 2:
Download the whole repository through [this link](https://github.com/PeterQiu0516/RoboAdvisor/archive/master.zip).


### Running
---
Access the `01_20` directory and make sure that the three input files `bloomberg.csv`、`filter.csv` and `newfund.csv` are present in the `01_20` directory.

Then run

```
.\python final.py
```

And access the following [survey page](localhost:9000) and finish all the questions on it.


After a while, the optimal portfolio generated by RoboAdvisor will automatically show up.


## Milestones

### Data Acquisition - Web Crawler
---
I first obtained the historical data for 800 selected funds from [iFund](https://www.ifund.com.hk/en/companies/) and Bloomberg terminal based on Python and R.

For more details, you may refer to my [Web Crawler repository](https://github.com/PeterQiu0516/WebCrawler).

### Investment Preferences Analysis - Online Survey Design
---
I designed a questionaire to investigate the customers' specific investment preferences (like risks and return rates requirements).



### Data Processing - Fund Filter and Classifier
---

Supported by `Javascript` and Bloomberg.

### Model Construction - Markowitz Mean-Variance Model and Black-litterman Model
---

Then I designed the specific funding recommendation system to satisfy each customer's specific investment preferences based on Python and R. 

I utilized the famous Markowitz and Black-Litterman model in the main body of the project by `PyPortfolioOpt` package

We also use [Time Series Model ARIMA](https://github.com/PeterQiu0516/GoogleCloud-ML-for-Trading/tree/master/Course%201%20-%20Introduction%20to%20Trading%2C%20Machine%20Learning%20%26%20GCP/Qwiklab%203%20-%20Build%20a%20Time%20Series%20Model%20(ARIMA%20Model)%20to%20Forecast%20Stock%20Price) to make better estimates of the expected return for the portfolio under the support of `statsmodels`.


### Generate Portfolio Report - Diagram Plotting
---
Supported by `EChart`.


## Explore more
+ [Web Crawler](https://github.com/PeterQiu0516/WebCrawler)
+ [Official Documentation for StatsModels](http://www.statsmodels.org/stable/index.html)
+ [Official Documentation for PyPortfolioOpt](https://pyportfolioopt.readthedocs.io/en/latest/)
+ [More about Time Series and ARIMA model](https://github.com/PeterQiu0516/GoogleCloud-ML-for-Trading/tree/master/Course%201%20-%20Introduction%20to%20Trading%2C%20Machine%20Learning%20%26%20GCP/Qwiklab%203%20-%20Build%20a%20Time%20Series%20Model%20(ARIMA%20Model)%20to%20Forecast%20Stock%20Price)
+ [Echarts](https://echarts.apache.org/zh/index.html)
