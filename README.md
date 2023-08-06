# European Football Database Data Analysis
<p align="center">
  <img src="https://github.com/awazbhujel/European-Football-Database-Analysis-Using-Python-SQL/blob/main/Football.png"  title="hover text">
</p>

## Table of Contents

1. [Introduction](#introduction)
2. [Data Wrangling](#data-wrangling)
3. [Exploratory Data Analysis](#exploratory-data-analysis)
    - [Number of Matches in Each League in the 2016 Season](#matches-in-each-league-2016)
    - [League with the Most Draws in the 2016 Season](#league-most-draws-2016)
    - [League with the Most Wins or Not Draws in the 2016 Season](#league-most-wins-2016)
    - [Team with the Fewest Losses in the 2016 Season](#team-fewest-losses-2016)
    - [League with the Most Goals in the 2016 Season](#league-most-goals-2016)
    - [Teams with the Most Wins in the 2016 Season](#teams-most-wins-2016)
    - [Teams' Improvement Over the Time Period](#teams-improvement-over-time)
    - [Players with the Most Penalties](#players-most-penalties)
    - [Team Attributes Leading to the Most Victories](#team-attributes-most-victories)
    - [Number of Players with Overall Rating > 90](#players-overall-rating-90)
    - [Attributes Contributing to Players' Overall Rating](#attributes-contributing-players-overall-rating)
4. [Limitations](#limitations)
5. [Conclusions](#conclusions)

## Introduction

This repository contains a data analysis project using the European Football Database. The dataset provides a comprehensive collection of football-related data, including match details, player information, team attributes, and more. The dataset covers matches from 11 European countries, spanning the seasons from 2008 to 2016.

## Dataset

The European Soccer Database used in this analysis is available on Kaggle:

[European Soccer Database on Kaggle](https://www.kaggle.com/hugomathien/soccer)

- +25,000 matches: Detailed information on individual soccer matches, including match events, goal types, possession, corner kicks, fouls, cards, and more.
- +10,000 players: Comprehensive details about soccer players, such as player attributes, height, weight, and other statistics.
- 11 European countries with their lead championship: Soccer data from major European leagues, providing insights into team performance across different countries.
- Seasons 2008 to 2016: The dataset covers several soccer seasons, allowing for historical analysis and trend exploration.

*Note: The analysis in this repository focuses on exploring the data, creating visualizations, and gaining insights from the European Soccer Database.*

## Requirements

- Jupyter Notebook
- Python
- pandas
- numpy
- matplotlib
- sqlite3

## Data Wrangling

Data wrangling is a critical step in the data analysis process to prepare the dataset for exploration and analysis. During the data wrangling process of the European Soccer Database, the following actions were taken:

### Handling Missing Players and Match Data

Some players' and match data were found to be missing from their respective tables. To address this, strategies like imputation or exclusion were employed to handle missing data while considering potential biases that may arise from these missing values.

### Resolving Duplicated and Incomplete Players' Names

The players' names were identified to appear duplicated and incomplete in some instances, which could result in inaccurate matching and affect the overall analysis. Efforts were made to identify and resolve such naming issues to ensure accurate player-related insights.

### Dealing with Missing Values in Player Attributes

The "buildUpPlayDribbling" column in the Player Attributes table had a significant number of missing values. Due to the high percentage of missing data, this column was temporarily removed from the analysis until a suitable method for imputing the missing values was identified.

### Converting Date Format

All dates in the dataset were provided as strings. To facilitate temporal analysis, the date columns were converted to datetime format.

### Addressing Data Integrity Challenges

The dataset may contain duplicated records and other data integrity challenges. Efforts were made to identify and address these discrepancies to ensure the accuracy of statistical results.

Efficient data wrangling ensured that the European Soccer Database was ready for in-depth exploration and analysis, enabling valuable insights into team and player performance and trends across different leagues.


## Limitations

During the analysis of the European Soccer Database, the following limitations and challenges were identified:

1. Missing Players and Match Data: Some players' and match data are missing from the respective tables, leading to incomplete information. This could impact the accuracy and completeness of the analysis. Appropriate strategies will be employed to handle missing data, such as imputation or exclusion, while considering potential biases.

2. Duplicated and Incomplete Players' Names: The players' names may appear duplicated and incomplete in some instances, which can result in inaccurate matching and affect the overall analysis. Efforts will be made to identify and resolve such naming issues to ensure accurate player-related insights.

3. Missing Values in Player Attributes: The "buildUpPlayDribbling" column in the Player Attributes table has a significant number of missing values. Due to the high percentage of missing data, this column will be temporarily removed from the analysis until a suitable method for imputing the missing values is identified.

4. Date Format: All dates in the dataset are provided as strings. To facilitate temporal analysis, the date columns will be converted to datetime format.

5. Data Integrity Challenges: The dataset may contain duplicated records and other data integrity challenges. Such discrepancies can impact the accuracy of statistical results and require thorough data cleaning and validation procedures.

Efforts will be made to address these limitations during the data analysis process to ensure that the conclusions drawn from the European Soccer Database are meaningful and reliable.

## Conclusions

Based on the analysis of the European Soccer Database, the following conclusions were drawn:

1. Variability in Matches Across Leagues: Each league had a different number of matches in the 2016 season, with England Premier League, France Ligue 1, Italy Serie A, and Spain LIGA BBVA having the most games (380 matches).

2. Draws in Leagues: France Ligue 1 had the most draw games with 108 matches, closely followed by England Premier League with 107 matches.

3. Wins and Losses: Spain LIGA BBVA had the most win or lose games with 288 matches, followed by Italy Serie A with 285 matches.

4. Fewest Losing Matches: Paris Saint-Germain had the fewest losing matches in the 2016 season, losing only 2 games.

5. Most Goals Scored: England Premier League scored the most goals in the 2015/2016 season with 1026 goals, followed by Spain LIGA BBVA with 1043 goals.

6. Most Wins by a Team: Paris Saint-Germain had the most wins in the 2015/2016 season, winning 30 games.

7. Most Improved Teams: From 2010 to 2016, the most improved teams in terms of average wins and goals were 'Paris Saint-Germain', 'Sporting CP', 'AZ', 'BSC Young Boys', and 'Napoli'.

8. Penalty Scorers: Rickie Lambert, Mario Balotelli, Xavi Hernandez, and Andrea Pirlo were the top penalty scorers in total.

9. Team Attributes for Wins: The most important team attributes that lead the teams to victory include Change Creation Passing, Defense Pressure, Defense Aggression, Build-Up Speed, and Build Dribbling. These attributes played a significant role in the analysis of the top 10 winning teams.

10. Players with Overall Rating > 90: There are 12 players with an overall rating of more than 90.

11. Top Player Attributes: The attributes that contribute most to players' overall rating include balanced play speed, shot power, dribbling, and strength.

These conclusions provide valuable insights into team and player performance, contributing factors to victories, and trends across different leagues. It is essential to consider these findings when interpreting and making use of the data.



11. Top Player Attributes: The attributes that contribute most to players' overall rating include balanced play speed, shot power, dribbling, and strength.

These conclusions provide valuable insights into team and player performance, contributing factors to victories, and trends across different leagues. It is essential to consider these findings when interpreting and making use of the data.

