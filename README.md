# Time-Series Logistic Regression

This repository focuses on time series analysis using the Logistic Regression model applied to financial data. The goal is to develop predictive models for forecasting financial trends and price directions over time.

## Project Overview

Time series analysis is crucial for forecasting financial data. This project utilizes historical financial data for the EURUSD forex pair and applies the Logistic Regression model to predict future price directions. The project aims to be straightforward and replicable.

### Key Features

- **Data Retrieval**: Custom functions are used to fetch historical financial data from MetaTrader 5.
- **Data Processing**: The data is prepared for modeling, including standardization and feature engineering.
- **Model Development**: Logistic Regression models are developed and trained on the processed data.
- **Model Evaluation**: Model performance is assessed using appropriate metrics to ensure accuracy.
- **Visualization**: Key results and trends are visualized to provide insights into the data and model performance.

## Repository Structure

- **`data.py`**: Contains functions for data retrieval and manipulation, including:
  - `get_rates`: Fetches historical price data for a given symbol and timeframe.
  - `add_shifted_columns`: Adds lagged versions of columns to a DataFrame for time series prediction.
  - `split_data`: Splits data into training and testing sets.

- **`backtest.py`**: Provides functions for backtesting financial strategies, including:
  - `compute_strategy_returns`: Calculates returns for a given strategy.
  - `plot_returns`: Visualizes cumulative returns of a strategy.
  - `vectorize_backtest_returns`: Computes financial metrics such as Sortino, Beta, and Alpha ratios.
  - `compute_model_accuracy`: Calculates and visualizes the accuracy of model predictions.
  - `strategy_drawdown`: Computes and visualizes the drawdown of the strategy.

- **`Logistic Regression Model.ipynb`**: Jupyter Notebook containing the main code for data processing, model development, evaluation, and visualization.

- **`.gitignore`**: Specifies files and directories to be ignored by Git.

- **`LICENSE`**: The MIT License under which this project is distributed.

- **`README.md`**: This file.

## Installation

To run this project, you need Python installed along with the following packages:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `MetaTrader5`

## Getting Started

1. **Clone the Repository**: Clone this repository to your local machine using `git clone https://github.com/YarosInter/Time-Series-Logistic-Regression.git`.

2. **Install Dependencies**: Ensure all required Python packages are installed.

3. **Run the Notebook**: Open `Logistic Regression Model.ipynb` in Jupyter Notebook to explore the model and results.

4. **Data Retrieval**: Use `data.py` to fetch and preprocess financial data.

5. **Backtesting**: Use `backtest.py` to evaluate your strategy's performance.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or new features.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.