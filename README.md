# Solar Power Prediction: ANN vs. ARIMA

## Overview

This repository contains a comparative analysis of solar power generation prediction using two models:

1. **Artificial Neural Networks (ANN)**
2. **ARIMA (AutoRegressive Integrated Moving Average)**

The project evaluates the performance of these models in forecasting solar power generation using metrics such as Mean Squared Error (MSE) and Root Mean Squared Error (RMSE).

---

## Features

- **Data Preprocessing**: Handling missing values, normalizing the data, and preparing it for training.
- **ANN Model**: Implementation of a feedforward neural network for solar power prediction.
- **ARIMA Model**: Time series analysis and forecasting using ARIMA.
- **Model Comparison**: Evaluation using statistical metrics (MSE, RMSE) and visualization of predictions.
- **Visualization**: Graphical representation of actual vs. predicted solar power values.

---

## Dataset

The dataset used for this analysis contains historical solar power generation data, including:

- Timestamps
- Power output (in kilowatts)
- Weather parameters (optional for ANN)

### Data Source:

- Publicly available solar generation datasets or simulation-generated data.

### Preprocessing Steps:

1. Handling missing timestamps.
2. Normalizing the power output to [0, 1] range.
3. Splitting into training and testing sets.

---

## Requirements

Install the following dependencies before running the project:

```bash
pip install numpy pandas matplotlib scikit-learn statsmodels tensorflow
```

---

## Usage

### 1. Clone the Repository

```bash
git clone https://github.com/username/solar-power-prediction.git
cd solar-power-prediction
```

### 2. Prepare the Dataset

Place your dataset in the `data/` directory. Ensure the file is named `solar_power_data.csv` or modify the file paths in the scripts.

### 3. Run Models

#### ARIMA Model

```bash
python models/arima_model.py
```

#### ANN Model

```bash
python models/ann_model.py
```

### 4. Visualize Results

Use the `notebooks/analysis.ipynb` to generate plots comparing actual vs. predicted values and evaluate model performance.

---

## Results

### Metrics Comparison:

| Model | MSE     | RMSE   |
| ----- | ------- | ------ |
| ANN   | 0.00045 | 0.0212 |
| ARIMA | 0.00049 | 0.0221 |

### Sample Visualization:



---

## Key Insights

- ANN outperforms ARIMA in terms of accuracy due to its ability to capture nonlinear patterns in the data.
- ARIMA is faster and simpler for time series forecasting but struggles with nonlinear relationships.

---

## Future Work

- Experiment with hybrid models combining ARIMA and ANN.
- Incorporate additional features like weather conditions.
- Test with larger datasets for scalability.

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

---

