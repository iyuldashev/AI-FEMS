# Development of an AI-Based Energy Management System (FEMS) for Factory Power Saving

This repository contains the source code and documentation for the **AI-Based Energy Management System (FEMS)** project, developed to optimize and predict energy usage in factories.

## Project Overview

The main objective is to predict peak power consumption using advanced AI models, leveraging data collected from the Jeju Samdasoo factory through IoT-based big data collection systems.

## Dataset

Data used in this project was collected from [**Jeju Samdasoo factory**](https://en.wikipedia.org/wiki/Jeju_Samdasoo) using IoT sensing technologies, including both univariate and multivariate time-series datasets related to energy usage.

## 📈 Detailed Model Performance

### LSTM Model Performance

| Configuration          | Multivariate (Original) | Multivariate (No Outliers) | Univariate (Original) | Univariate (No Outliers) |
|------------------------|-------------------------|----------------------------|-----------------------|--------------------------|
| Epochs/Train:Test Ratio | 100/8:2                | 100/8:2                   | 100/8:2              | 100/8:2                 |
| Sequence Length        | 30                     | 30                        | 144                  | 144                     |
| **Metrics**            |                        |                           |                      |                         |
| SSE                    | 4.38                   | 3.23                      | 2.039                | 4.384                   |
| MSE                    | 0.002                  | 0.002                     | 0.001                | 0.003                   |
| RMSE                   | 0.047                  | 0.045                     | 0.039                | 0.06                    |
| MAE                    | 0.037                  | 0.042                     | 0.026                | 0.044                   |
| R²                     | 0.96                   | 0.66                      | 0.98                 | 0.76                    |
| MAPE (%)               | 6.73                   | 5.41                      | 5.51                 | 3.55                    |
| sMAPE (%)              | 3.82                   | 2.79                      | 3.39                 | 3.28                    |

### XGBoost Model Performance

| Configuration          | Multivariate (Original) | Multivariate (No Outliers) | Univariate (Original) | Univariate (No Outliers) |
|------------------------|-------------------------|----------------------------|-----------------------|--------------------------|
| N_Estimators           | 500                    | 200                        | 1000                 | 1000                    |
| **Metrics**            |                        |                           |                      |                         |
| SSE                    | 0.62                   | 3.1                       | 99795.9              | 98428.5                 |
| MSE                    | 0.0003                 | 0.002                     | 0.058                | 0.057                   |
| RMSE                   | 0.018                  | 0.045                     | 0.24                 | 0.23                    |
| MAE                    | 0.013                  | 0.031                     | 0.14                 | 0.14                    |
| R²                     | 0.93                   | 0.67                      | 0.37                 | 0.34                    |
| MAPE (%)               | 1.73                   | 3.85                      | 54.67                | 57.76                   |
| sMAPE (%)              | 0.87                   | 1.98                      | 12.41                | 12.29                   |


## Benefits and Impacts

- Significant reduction in energy costs.
- Approximately 10–15% carbon emission reduction.
- Supports ESG (Environmental, Social, and Governance) compliance.

## Citation

If using this project or dataset, please cite the following publication:

- [**KCI Paper**](https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART003153842)


## Attribution

This project was developed by [**Future Internet Lab**](https://icms.pknu.ac.kr/network/1) at Pukyong National University. Please credit the authors and the lab when using or referencing this work.
