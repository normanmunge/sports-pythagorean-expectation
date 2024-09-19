# Pythagorean Expectation on Sports Data

Pythagorean expectation is used in sports analytics to make data driven analytics and predictive modelling

This is a concept that comes from baseball. It was developed by the baseball analyst, (Bill James)[https://en.wikipedia.org/wiki/Bill_James], one of the great analysts of sports. It's basically about a relationship between winning and the success of teams as measured by points, goals, runs, score, depending on which sport we happen to be talking about.
The formula basically states that the percentage of games a professional sports team will win across a given season should be proportional to the ratio of the square of the points/runs/goals scored by the team in the season, divided by the sum of squares of the points/runs/goals scored by the team and its opponents across the whole season:

wpc % = runs**2 / sum(home_runs ** 2 + conceeded_runs ** 2)

𝑤𝑖𝑛 𝑟𝑎𝑡𝑖𝑜(𝑏𝑎𝑠𝑒𝑏𝑎𝑙𝑙)=𝑟𝑢𝑛𝑠 𝑠𝑐𝑜𝑟𝑒𝑑𝑘𝑟𝑢𝑛𝑠 𝑠𝑐𝑜𝑟𝑒𝑑𝑘 + 𝑟𝑢𝑛𝑠 𝑎𝑙𝑙𝑜𝑤𝑒𝑑𝑘

This is a concept which can help to explain why teams are successful and can also be used as the basis for predicting results in the future. It’s a relationship that we can measure with data. We can actually calculate the Pythagorean Expectation for each team and then we can test whether it truly is related to the win percentage of the team.

#### Why is pythagorean expectation useful in Sports?

* Pythagorean winning percentage can help to identify teams that have either overachieved or underachieved. When looking at a club with a surprisingly poor or surprisingly strong record early in the season, using the theory to determine a team's "expected" winning percentage for the remainder of the year can paint a more accurate picture of how things will play out than merely looking at actual winning percentage. (mlb.com)[https://www.mlb.com/glossary/advanced-stats/pythagorean-winning-percentage]

* The pythagorean ratio can tell us how many wins a team was meant to get.

* Winning more games than your Pythagorean Expectation tends to mean a team will decline the following season, while falling short of expectations in the cirrent year tends to mean a team will improve the following season.


### About the repository

This repository contains 2 notebooks showing how to calculate the pythagorean expectation and evaluating the accuracy of a team winning a game based on the R squared Score. The leagues explored are the MLB (Major League Baseball) and the English League between 2017-2018 including all the division in the U.K from the English Premier League, English Football Championship, Division 1 and Division 2.
It is useful for any data scientist hoping to learn about feature engineering and any sports analytics enthusiast pursuing how sports and data combine.

The datasets include:
 * (MLB)[datasets/gl2023.txt]
 * (English League 2017-18)[datasets/Engsoccer2017-18.xlsx]

It showcases my journey venturing into sports analytics and is only meant for educational purposes.

### Steps Included

1. Importing necessary libraries
2. Loading the datasets
3. Data Wrangling & Exploratory Data Analaysis
4. Feature Engineering - To get features with the total wins, scores, conceeded goals, pythagorean expectation, win percentage calculation etc
5. Evaluating the Pythagorean Expectation Performance

### Running the notebook

The instructions below show how to run the notebooks on a mac terminal.

To run the notebook. Follow the instructions below on a terminal:

#### A. Create a virtual environment

A virtual environment is recommended to install the necessary libraries needed to run the notebook. A virtual environment separates your local projects libraries and the global machine's libraries reducing the chances of conflicts.

`python -m venv [path/to/environments/name-of-env]`

#### B. Activate your virtual environment

`source [path/to/environment]/bin/activate`

#### C. Install necessary libraries

`pip install numpy pandas matplotlib seaborn statsmodels jupyterlab`

#### D. Running the notebook

`jupyter lab`

#### E. Saving and closing your virtual environment

To save your projects, `Cmd + S` will do the trick. Afterwards, on your terminal, enter `deactivate`


### Further Resources

For further reading, you can explore the links below:

1. [Coursera Sports Analytics Foundation](https://www.coursera.org/learn/foundations-sports-analytics)
2. [Guide to estimating win probabilities in sports](https://medium.com/@cricketscience/pythagorean-expectation-a-guide-to-estimating-win-probabilities-in-any-sport-c470280381bc)
3. [Pythagorean Expectation](https://en.wikipedia.org/wiki/Pythagorean_expectation)

