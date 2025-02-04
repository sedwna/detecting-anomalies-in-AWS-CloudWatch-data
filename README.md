# Anomaly Detection in AWS CloudWatch Data

This project demonstrates how to detect anomalies in AWS CloudWatch request count data using Python, Pandas, Seaborn, and the Isolation Forest algorithm. The dataset is sourced from the [Numenta Anomaly Benchmark (NAB)](https://github.com/numenta/NAB/tree/master/data/realAWSCloudwatch).

## Dataset
The dataset used in this project is `elb_request_count_8c0756.csv`, which contains timestamped request counts from an AWS Elastic Load Balancer (ELB). The dataset is available in the [NAB repository](https://github.com/numenta/NAB/tree/master/data/realAWSCloudwatch).

## Requirements
To run this project, you need the following Python libraries:
- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `scikit-learn`

You can install the required libraries using pip:
```bash
pip install pandas numpy seaborn matplotlib scikit-learn