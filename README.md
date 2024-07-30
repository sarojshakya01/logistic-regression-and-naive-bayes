# Logistic Regression and Naive Bayes

This repository contains implementations and comparisons of Logistic Regression and Naive Bayes classifiers on various datasets. The primary goal is to demonstrate the performance and applications of these fundamental machine learning algorithms.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Logistic Regression](#logistic-regression)
- [Naive Bayes](#naive-bayes)
- [Evaluation](#evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Logistic Regression and Naive Bayes are two popular machine learning algorithms used for classification tasks. This project aims to implement both algorithms from scratch and evaluate their performance on a range of datasets.

## Dataset
The datasets used for this project include:
1. **Sentiment140**: A dataset for binary sentiment classification.
2. **20 Newsgroups**: A dataset for multi-class text classification.

## Installation
To get started, clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/sarojshakya01/logistic-regression-and-naive-bayes.git
cd logistic-regression-and-naive-bayes
pip install -r requirements.txt
```

## Usage
### Preprocess Data
Prepare the data for training and testing:

```bash
python preprocess_data.py --data_dir path_to_data
```

### Train Models
Train the Logistic Regression and Naive Bayes models:

```bash
python train_logistic_regression.py --config config.yaml
python train_naive_bayes.py --config config.yaml
```

### Evaluate Models
Evaluate the models on test data:

```bash
python evaluate_model.py --model logistic_regression --data_dir path_to_test_data
python evaluate_model.py --model naive_bayes --data_dir path_to_test_data
```

## Logistic Regression
Logistic Regression is a linear model for binary classification. The implementation includes:
- Gradient Descent for parameter optimization.
- Regularization to prevent overfitting.

## Naive Bayes
Naive Bayes is a probabilistic classifier based on Bayes' theorem. The implementation includes:
- Multinomial Naive Bayes for text classification.
- Laplace smoothing to handle zero probabilities.

## Evaluation
The models are evaluated using standard metrics such as accuracy, precision, recall, and F1-score. Cross-validation is used for hyperparameter tuning.

## Results
The results of the models are documented in the `results` directory. Detailed performance metrics and visualizations are available in the evaluation reports.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes. Ensure that your code adheres to the project's coding standards and includes appropriate tests.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
