# Anomaly Detection in Time Series Data 🕵️‍♂️

This repository contains three different approaches for detecting anomalies in time series data:
1. **Density Estimation**: Uses multivariate Gaussian distribution to estimate the likelihood of data points.
2. **Isolation Forest**: An unsupervised algorithm that isolates anomalies using random forests.
3. **Local Outlier Factor (LOF)**: A density-based method that identifies outliers by comparing the local density of a point to its neighbors.

The dataset used is the `elb_request_count_8c0756.csv` from the **Numenta Anomaly Benchmark (NAB)**, which contains time-stamped request counts from an AWS Elastic Load Balancer.

---

## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Dataset](#dataset)
5. [Methods Overview](#methods-overview)
6. [Visualization](#visualization)
7. [Contributing](#contributing)

---

## Features ✨

- **Three Anomaly Detection Methods**:
  - **Density Estimation**: Based on multivariate Gaussian distribution.
  - **Isolation Forest**: An efficient algorithm for detecting anomalies in high-dimensional data.
  - **Local Outlier Factor (LOF)**: A density-based method for identifying local outliers.
- **Visualization**: Clear visualizations of time series data and detected anomalies.
- **Modular Code**: Each method is implemented in a separate Jupyter Notebook for easy understanding and extension.

---

## Installation 🛠️

### Prerequisites

- Python 3.7 or higher
- Required Python libraries (listed in `requirements.txt`)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/AnomalyDetection.git
   cd AnomalyDetection
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage 🚀

### Running the Anomaly Detection Methods

1. **Density Estimation**:
   - Open the `density_estimation.ipynb` notebook.
   - Run all cells to preprocess the data, estimate density, and detect anomalies.

2. **Isolation Forest**:
   - Open the `Isolation_Forest.ipynb` notebook.
   - Run all cells to preprocess the data, train the Isolation Forest model, and detect anomalies.

3. **Local Outlier Factor (LOF)**:
   - Open the `local_outlier_factor.ipynb` notebook.
   - Run all cells to preprocess the data, train the LOF model, and detect anomalies.

---

## Dataset 📊

The dataset used in this project is from the **Numenta Anomaly Benchmark (NAB)**. Specifically, it uses the `realAWSCloudwatch/elb_request_count_8c0756.csv` file, which contains time-stamped request counts from an AWS Elastic Load Balancer.

You can download the dataset from the [NAB GitHub repository](https://github.com/numenta/NAB/tree/master/data/realAWSCloudwatch).

---

## Methods Overview 🧠

### 1. Density Estimation

- **Description**: Uses a multivariate Gaussian distribution to estimate the likelihood of data points. Points with low likelihood are flagged as anomalies.
- **Steps**:
  1. Preprocess the data and create lagged features.
  2. Fit a multivariate Gaussian distribution to the data.
  3. Calculate the log-likelihood of each data point.
  4. Flag points with log-likelihood below a threshold as anomalies.

### 2. Isolation Forest

- **Description**: An unsupervised algorithm that isolates anomalies by randomly selecting features and splitting data points.
- **Steps**:
  1. Preprocess the data and create lagged features.
  2. Train an Isolation Forest model.
  3. Predict anomalies using the trained model.
  4. Visualize the results.

### 3. Local Outlier Factor (LOF)

- **Description**: A density-based method that compares the local density of a point to its neighbors. Points with significantly lower density are flagged as anomalies.
- **Steps**:
  1. Preprocess the data and create lagged features.
  2. Train an LOF model.
  3. Predict anomalies using the trained model.
  4. Visualize the results.

---

## Visualization 📈

Each method generates the following visualizations:

1. **Time Series Plot**:
   - A line plot of the time series data.
   - Anomalies are highlighted with red dots.

2. **Anomaly Distribution**:
   - A histogram or scatter plot showing the distribution of normal vs. anomalous data points.

### Example Plots

![Time Series Plot](time_series_plot.png)  
*Time series data with anomalies highlighted in red.*

![Anomaly Distribution](anomaly_distribution.png)  
*Distribution of normal vs. anomalous data points.*

---

## Contributing 🤝

We welcome contributions to this project! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeatureName`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push your changes to your fork (`git push origin feature/YourFeatureName`).
5. Open a Pull Request.

---

## Acknowledgments 🙏

- **Numenta**: For providing the Numenta Anomaly Benchmark (NAB) dataset.
- **Scikit-learn**: For the Isolation Forest and Local Outlier Factor implementations.
- **Seaborn and Matplotlib**: For data visualization.

---

## Contact 📧

For questions or feedback, feel free to reach out:
- **Email**: sajaddehqan2002@gmail.com
- **LinkedIn**: [[My LinkedIn Profile](https://www.linkedin.com/in/sajad-dehqan-189a0b258/)]

---

