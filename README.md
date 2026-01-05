# Will Pigeon Eat Bun?

A Machine Learning project to predict whether a pigeon will eat a bun based on various environmental and bun characteristics.

## Description

This project analyzes pigeon eating behavior using Machine Learning techniques. We compare three supervised classification algorithms to predict whether a pigeon will eat a given bun.

**Dataset:** [Will Pigeon Eat Bun?](https://www.kaggle.com/datasets/devanshbesain/will-pigeon-eat-bun) (Kaggle)

- 2000 training observations
- 500 test observations
- 12 features (bun size, temperature, humidity, etc.)

## Objectives

1. Explore and analyze data to identify key factors
2. Train and compare 3 classification models
3. Evaluate performance with appropriate metrics
4. Identify the best model for prediction

## Implemented Models

| Model                       | Accuracy | Precision | Recall | F1-Score  |
| --------------------------- | -------- | --------- | ------ | --------- |
| **KNN (k=5)**               | 0.830    | 0.807     | 0.924  | 0.861     |
| **Decision Tree (depth=5)** | 0.770    | 0.794     | 0.808  | 0.801     |
| **Naive Bayes**             | 0.858    | 0.836     | 0.936  | **0.883** |

**Best model:** Naive Bayes (F1-Score: 0.883)

## Installation and Usage

### Prerequisites

- Python 3.8+
- pip

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the notebook

```bash
jupyter notebook project.ipynb
```

Or open `project.ipynb` directly in VS Code with the Jupyter extension.

## Project Structure

```
WillPigeonEatBun/
├── project.ipynb          # Main notebook with complete analysis
├── train_bun.csv         # Training data
├── test_bun.csv          # Test data
├── requirements.txt      # Python dependencies
├── Dockerfile           # Docker configuration
├── docker-compose.yml   # Docker orchestration
└── README.md            # This file
```

## Methodology

1. **Data Exploration**

   - Target variable distribution analysis
   - Correlation visualization
   - Feature distribution analysis

2. **Preprocessing**

   - Feature standardization (for KNN)
   - Train/test split (70/30)
   - Fixed random state for reproducibility

3. **Training and Validation**

   - 5-fold cross-validation
   - Test set evaluation
   - Metrics: Accuracy, Precision, Recall, F1-Score

4. **Model Comparison**
   - Confusion matrices
   - Performance analysis
   - Best model selection

## Key Results

- **Naive Bayes** achieves the best overall performance (F1: 0.883)
- Excellent **recall** (0.936) for identifying pigeons that will eat
- **KNN** also performs well (F1: 0.861)
- **Decision Tree** weaker but fast and interpretable

## Technologies Used

- Python 3.13
- scikit-learn (ML algorithms)
- pandas (data manipulation)
- numpy (numerical computing)
- matplotlib & seaborn (visualizations)
- jupyter (interactive notebooks)

## Author

Project completed as part of the Machine Learning course - HEG Geneva (2026)

## License

This project is for educational purposes only.
