# Phishing Website Detection Using Machine Learning

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Overview

This project leverages machine learning techniques to detect phishing websites, one of the most common social engineering and cyber attacks. Phishers target online users by creating deceptive websites that mimic legitimate ones, tricking users into revealing sensitive information. This project aims to automatically identify such phishing attempts using various ML models and feature extraction techniques.

## Features

- **Multiple Feature Categories**: Extracts 17 distinctive features from URLs including:
  - Address Bar Based Features (URL length, domain, IP address, '@' symbol, etc.)
  - Domain Based Features (DNS record, website traffic, age of domain, etc.)
  - HTML & JavaScript Based Features (iframe redirection, right-click disabling, etc.)

- **Machine Learning Models**: Implements and compares various algorithms:
  - XGBoost
  - Multilayer Perceptrons
  - AutoEncoder Neural Network
  - Random Forest
  - Decision Tree
  - Support Vector Machines

- **High Accuracy**: Achieves up to 85.7% accuracy in detecting phishing websites

## Dataset

The dataset contains 10,000 URLs:
- 5,000 legitimate URLs from the University of New Brunswick dataset
- 5,000 phishing URLs from PhishTank (an open-source service)

## Approach

1. **Data Collection**: Gathering legitimate and phishing URLs from reliable sources
2. **Feature Extraction**: Extracting 17 key features from URLs and website content
3. **Data Preprocessing**: Analyzing and cleaning data using EDA techniques
4. **Model Training**: Training multiple machine learning models on the prepared dataset
5. **Evaluation**: Comparing model performance using accuracy metrics
6. **Model Selection**: Selecting the best-performing model (XGBoost) for deployment

## Results

| ML Model | Train Accuracy | Test Accuracy |
|----------|----------------|---------------|
| XGBoost | 0.868 | 0.857 |
| Multilayer Perceptrons | 0.866 | 0.854 |
| AutoEncoder | 0.810 | 0.810 |
| Random Forest | 0.820 | 0.809 |
| Decision Tree | 0.816 | 0.803 |
| SVM | 0.806 | 0.786 |

## Future Work

- Develop a browser extension to provide real-time phishing detection
- Create a user-friendly GUI for URL verification
- Expand the feature set to improve detection accuracy
- Implement active learning to continuously improve model performance

## Requirements

- Python 3.6+
- scikit-learn
- XGBoost
- TensorFlow/Keras
- pandas
- numpy
- matplotlib
- requests (for URL fetching)
- BeautifulSoup (for HTML parsing)

## Installation

```bash
git clone https://github.com/yourusername/phishing-detection.git
cd phishing-detection
```


## License

This project is licensed under the GPL 3.0 - see the LICENSE file for details.

## Acknowledgments

- University of New Brunswick for the legitimate URL dataset
- PhishTank for providing phishing URL data

## Contributors

- [Your Name](https://github.com/SahilBane2002)

---

*Note: This project is for educational purposes only. Always use proper cybersecurity practices and tools to protect against phishing attacks.*
