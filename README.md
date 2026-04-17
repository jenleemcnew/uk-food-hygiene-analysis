# UK Food Hygiene Analysis

## Overview
A NoSQL database analysis project using MongoDB to evaluate UK food establishment 
hygiene ratings on behalf of the fictional food magazine *Eat Safe, Love*. The 
project involves database setup, data cleaning, and exploratory analysis to help 
identify the best and worst rated establishments across the UK.

---

## Process

### Part 1 — Database Setup
- Imported `establishments.json` into MongoDB as the `uk_food` database
- Configured PyMongo connection and verified data load

### Part 2 — Database Updates
- Added a new unrated halal restaurant (Penang Flavours, Greenwich)
- Looked up and assigned the correct `BusinessTypeID`
- Removed all Dover Local Authority establishments per magazine request
- Converted latitude, longitude, and `RatingValue` fields from strings to 
  appropriate numeric types

### Part 3 — Exploratory Analysis
Answered the following questions for the magazine editors:
- Which establishments have a hygiene score of 20?
- Which London establishments have a `RatingValue` of 4 or higher?
- What are the top 5 establishments with a `RatingValue` of 5, sorted by 
  lowest hygiene score, nearest to Penang Flavours?
- How many establishments in each Local Authority have a hygiene score of 0?

---

## Tech Stack
- Python (PyMongo, Pandas, pprint)
- MongoDB
- Jupyter Notebook

---

## Repository Contents
| File | Description |
|------|-------------|
| `NoSQL_setup_starter.ipynb` | Database setup and update notebook |
| `NoSQL_analysis_starter.ipynb` | Exploratory analysis notebook |
| `establishments.json` | Source dataset from UK Food Standards Agency |

---

## Data Source
[UK Food Standards Agency](https://ratings.food.gov.uk/open-data/en-GB) — 
UK food hygiene rating data, licensed under the Open Government Licence v3.0.
