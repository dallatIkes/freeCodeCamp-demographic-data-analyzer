# Demographic Data Analyzer

This repository contains my solution to freeCodeCamp’s **Demographic Data Analyzer** project (Data Analysis with Python).

The project implements the function `calculate_demographic_data(print_data=True)` which reads the census file `adult.data.csv` and computes several demographic statistics using **pandas**.

## What it computes

- Number of each race represented in the dataset
- Average age of men
- Percentage of people with a Bachelor's degree
- Percentage of people with and without advanced education (`Bachelors`, `Masters`, `Doctorate`) that earn more than 50K
- Minimum number of hours a person works per week
- Percentage of rich people among those who work the minimum number of hours
- Country with the highest percentage of people earning >50K (and that percentage)
- Most popular occupation for those who earn >50K in India

## Files

- `demographic_data_analyzer.py` — implementation containing `calculate_demographic_data`
- `test_module.py` — unit tests
- `main.py` — entry script that calls `test_module.py` to run the tests and print results
- `requirements.txt` — Python dependencies
- `adult.data.csv` — input dataset (must be present in the repo root)

## Example

```python
from demographic_data_analyzer import calculate_demographic_data

result = calculate_demographic_data(print_data=False)
print(result['average_age_men'])  # e.g. 39.4
```

## How to run

```bash
# install dependencies
pip install -r requirements.txt

# run the tests / main script
python3 main.py
```

`main.py` invokes the test suite (`test_module.py`) so running `python3 main.py` will print the computed statistics and run the unit tests.

## Requirements

See `requirements.txt`
