# Genetic Algorithm for Network Intrusion Classification

## Description
This project implements a Genetic Algorithm (GA) for feature selection and classification of network intrusions using the UNSW-NB15 dataset.  
The GA aims to select an optimal subset of features to maximize classification accuracy using logistic regression.

**Key Highlights:**
- Feature selection with GA
- Experiments with different GA configurations
- Evaluation and insights from results

---

## Features
- Implements GA with feature selection for intrusion detection
- Experiments with varying parameters: population size, crossover type, mutation rate
- Reports results in tabular format
- Outputs selected features and classification accuracy

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/raffay464/Genetic-Algorithm.git
2. Navigate to project folder:
   cd Genetic-Algorithm
3. Install Dependencies:
   pip install pandas pyarrow scikit-learn numpy
4. Run the Code:
   python Genetic-Algorithm.py

## Evaluation Summary

| Generation | Best Fitness Score | Selected Features Count |
| ---------- | ------------------ | ----------------------- |
| 1          | 0.9043             | proto, service, state   |
| 2          | 0.9024             | proto, service, state   |
| 3          | 0.8971             | proto, service, state   |


## Methodology

Fitness Function: Classification accuracy with logistic regression.
Selection: Roulette wheel selection.
Crossover: Single-point crossover.
Mutation: Random bit-flip mutation.
Classifier: Logistic Regression.

## Insights

The Genetic Algorithm improved classification accuracy across generations, consistently selecting certain features important for intrusion classification.
This demonstrates GA’s capability for feature selection in cybersecurity datasets.
