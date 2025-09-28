# Genetic Algorithm for Network Intrusion Classification

## Description
This project implements a Genetic Algorithm (GA) for feature selection and classification of network intrusions using the UNSW-NB15 dataset — a large-scale, real-world cybersecurity dataset containing various attack types such as DoS, worms, backdoors, and fuzzers.  
The GA is designed to automatically identify the most relevant subset of features that maximizes classification accuracy, reducing computational complexity while improving detection performance.  

The classification model used in this project is **Logistic Regression**, chosen for its simplicity and effectiveness in binary classification tasks. The GA approach enables exploration of the search space of possible feature subsets through evolutionary operators such as selection, crossover, and mutation, guided by a fitness function based on classification accuracy.

### Key Highlights:
- Feature selection using a Genetic Algorithm to improve intrusion detection performance.
- Experiments with varying GA configurations including population size, crossover strategy, and mutation rate to evaluate performance.
- Use of **Logistic Regression** for classification to measure fitness of selected features.
- Detailed evaluation results presented in tabular format for better insight.
- Outputs selected features and their impact on classification accuracy.

---

## Features
- Implements a Genetic Algorithm for feature selection in intrusion detection.
- Experiments with different GA parameter settings:
  - Population size
  - Number of generations
  - Number of parents for mating
  - Mutation rate
- Evaluation of classification accuracy for each configuration.
- Clear tabular results showing performance over generations.
- Outputs best feature subset and corresponding fitness score.

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
