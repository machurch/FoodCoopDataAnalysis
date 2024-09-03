# Analyzing Food Cooperative Sales Data

Author: Marguerite Church

## Overview

This is an independent project done for the UCSD Food Cooperative during the summer of 2024 with
sales data from the 2023-2024 school year. The goal is to explore what recipes sell best and what ingredients they contain.

# Introduction

![UCSD Food Coop Logo](https://pbs.twimg.com/profile_images/1451337247194640385/XKvNbnGe_400x400.jpg)

## What is the UCSD Food Cooperative?

The UCSD Food Cooperative is a non-hierarchical student run organization that serves cheap vegan meals daily to the greater UCSD community. The vegan meals are self-serve and priced per scoop. Scoops range from $2.50-$2.75. Alongside vegan meals made in the space, we serve food from vendors such as sambusas, drinks such as kombucha and coconut water, and basic needs supplies. All of the work is volunteer based, so any profits we make go right back into the space. We are open on weekdays from 11-3, and serve free food on fridays. If you are interested in learning more, here is our [Instagram](https://www.instagram.com/ucsdfoodcoop/?hl=en).

## Project Introduction

As a member of the food coop, I am interested in the ways we can boost our sales so that we can offer a greater variety of foods and goods. Knowing what items sell best and what days we profit on can help us grow and be able to better serve our community. 

## Data Introduction

I created this dataset, `recipes` myself by going through our archived menu documents and sales data from Square. We create our menus at the beginning of each week since we receive produce from the Food Rescue program and don't know what we will have until we pick it up. At our weekly meetings, we choose one recipe per day then write out instructions on how to prepare them. Here is a bit of a menu document from week 3 of spring quarter:
![UCSD Food Coop Menu Example](menuExample.png)
`recipes` contains a row for every day we were open in the 2023-2024 school year, which amounts to 136. `recipes` has 13 columns, described below.
| Column                | Description                                    |
| :-------------------- |:---------------------------------------------- |
| `'date'`              | Day the recipe was served                      |
| `'dish'`              | Name of the recipe                             |
| `'ingredients'`       | Minutes to prepare recipe                      |
| `'price'`             | Price per scoop                                |
| `'rice'`              | If the recipe was served with rice             |
| `'week_of_qtr'`       | Week of the quarter, 1-10                      |
| `'quarter'`           | Quarter of the school year                     |
| `'meals_sold'`        | Number of meals sold                           |
|  `'money_from_meals'` | Money made solely from meals                   |
| `'total_income'`      | Money made from meals, drinks, and vendor food |
| `'day'`               | Day of the week                                |
| `'price_per_meal'`    | `'money_from_meals'` divided by `'meals_sold'` |
| `'chickpeas'`         | If the recipe contains chickpeas|

# Data Cleaning and Exploratory Data Analysis
