# Daily AFAB births in California #

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jofaval/daily-california-births/blob/master/notebook.ipynb)

## Table of contents

1. [📁 Data](#-data)
1. [📓 Description](#-description)
1. [✔️ Objective](#-objective)
1. [🧱 Tech stack](#-tech-stack)
1. [💹 Algorithms](#-algorithms)
1. [📊 Visualization](#-visualization)
1. [🤓 Conclusions](#-conclusions)
1. [©️ Credits](#-credits)

## 📁 Data
[↑ Back to the table](#table-of-contents)

The data is available at the following link (not the official one, nor that I could find one):\
[https://raw.githubusercontent.com/jbrownlee/Datasets/master/daily-total-female-births.csv](https://raw.githubusercontent.com/jbrownlee/Datasets/master/daily-total-female-births.csv)

## 📓 Description
[↑ Back to the table](#table-of-contents)

It is an analysis of the daily AFAB (Assigned Female At Birth) born in California in the year 1959. There's barely any information reachable out there about this dataset other than it is from California and the year (mostly because it's a timeseries dataset).

## ✔️ Objectives
[↑ Back to the table](#table-of-contents)

- Use darts as the main python library for Timeseries
- Explore a little bit the data and analyze some of it's patterns.

## 🧱 Tech stack
[↑ Back to the table](#table-of-contents)

Python, that's it! R is a programming language that, as for the moment being, I have no experience with, even though it's powerful and broadly used, but I'd dare to say that no more than Python.

And one of the strongest points, if not the most, about Python, are it's libraries, so... the libraries I've used are:

- Pandas, data manipulation with an ease of use and exploration data analysis.
- Numpy, a really strong linear algebra library, used in the project for it's statistics utilities, SciPy may be an alternative, but I have no experience at all with it.
- Matplotlib and Seaborn, both fantastic libraries for data visualization, and they complement each other.
- Scikit-Learn, the library used for Machine Learning and statistics models: Linear Regression, SVR, Lasso, Ridge, etc.
- Tensorflow and Keras, the industry standard for Deep Learning, the way to go, not really, it's just that for now I don't have that many experience with PyTorch
- Kats and Facebook Prophet, Kats is the lightweight "version" of Facebook Prophet, which is an statistical library created by Facebook/Meta for timeseries.

## 💹 Algorithms
[↑ Back to the table](#table-of-contents)

As aforementioned I've used Kats and I also tried it out with Tensorflow, but with a different approach, it was copy and paste from [Time Series Forecasting using TensorFlow and Deep Hybrid Learning](https://towardsdatascience.com/time-series-forecasting-using-tensorflow-and-deep-hybrid-learning-5088ad76dd55) by [Aditya Bhattacharya](https://adib0073.medium.com/).

Darts didn't work on Google Colab, but at least I tried, it seems like a powerful library, but so is Karts, it was the fastest to set up and performed kind of well given the circumstances.

## 📊 Visualization
[↑ Back to the table](#table-of-contents)

I discovered the existence of confidence plots, which makes sense, but I mostly used lineplots, which is what I feel works best for timeseries visualizations, based on almost every timeseries visualization, I'd also like to try out the circular/vortex time visualization, but I feel it is far beyond my current skill level.

For this project, visualizations was just something extra, but they were mostly used to assert the model's performance

## 🤓 Conclusions
[↑ Back to the table](#table-of-contents)

Not many conclusions were found, but I feel that it is hard to properly predict it's pattern, but there sort of is one, it's spiky, but in a consistent manner, and some increase could be observed towards the end of the year, but wether it's something that belongs to the year or to California, can't be asserted with such a small sample of data.

Also, python libraries for timeseries are whole in and on itself, there's plenty to use, and I wanted to try darts (I might try it out locally) because I read somewhere (or it may have been a talk) I believe it was from: [Kishan Manani - Feature Engineering for Time Series Forecasting | PyData London 2022](https://www.youtube.com/watch?v=9QtL7m3YS9I).

## ©️ Credits
[↑ Back to the table](#table-of-contents)

At this point in time, I don't know who donated this data, or which organization. The strongest lead I found was from kaggle [Daily total female births in California, 1959](https://www.kaggle.com/datasets/dougcresswell/daily-total-female-births-in-california-1959) that said _originally published by Newton in 1988 at [https://datamarket.com/](https://datamarket.com/)_

Then to [Jason Brownlee](https://github.com/jbrownlee/) the author of the incredible [Machine Learning Mastery](https://machinelearningmastery.com/).

I'd also like to properly credit [Aditya Bhattacharya](https://adib0073.medium.com/) for it's great work at presenting RNN applied to Timeseries.
And to [Kishan Manani](https://github.com/KishManani) for this talk [Kishan Manani - Feature Engineering for Time Series Forecasting | PyData London 2022](https://www.youtube.com/watch?v=9QtL7m3YS9I)