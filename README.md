# Job-a-Thon-April-2022

## Problem Statement
ABC is a car rental company based out of Bangalore. It rents cars for both in and out stations at affordable prices. The users can rent different types of cars like Sedans, Hatchbacks, SUVs and MUVs, Minivans and so on.

In recent times, the demand for cars is on the rise. As a result, the company would like to tackle the problem of supply and demand. The ultimate goal of the company is to strike the balance between the supply and demand inorder to meet the user expectations. The company has collected the details of each rental. Based on the past data, the company would like to forecast the demand of car rentals on an hourly basis.

## Objective
The main objective of the problem is to develop the machine learning approach to forecast the demand of car rentals on an hourly basis.

## Approach
The data given had no features except date and hour. This was clearly a time series problem, so first thing I did is to reduce this problem to a regression problem. In order to reduce it to a Regression, I tried to capture the temporal dynamics of the data like things that affect every object in the data. So I extracted time based features like day of week, week of month, week of year, is the day is weekend, or is it start of the month or end of month because maybe people prefer to go out around payday or on public holidays.
After extracting all these features, I could approach it like simple Machine Learning problem.

## ML Approach
Before building an ML model, feature engineering was done. Basic time related features such as day, month, hour, weekofyear, dayofyear, weekday were created.I have tried some tree based model for this problem like Catboost, XGboost and LightGBM, out of these, LightGBM was working best, so I did some parameter tuning and checked the results for best parameter combination.The evaluation metric was 'RMSE'. This model gave a public leaderboard score of 33.88 and a private leaderboard score of 33.928.

## Final Result
Private Leaderboard Rank - 70

Public Leaderboard Rank - 127
