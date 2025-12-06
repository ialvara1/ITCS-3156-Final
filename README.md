Predicting Vehicle Fuel Efficiency (MPG) Using Machine Learning

This project was created for ITCS 3156.
The goal of the project is to predict a car’s fuel efficiency (MPG) using linear regression methods on the Auto MPG dataset.

I used two regression models:
Ordinary Least Squares (OLS)
Least Mean Squares (LMS) gradient descent

The project explores how preprocessing, feature scaling, and feature correlations affect the performance of each model.

Project Structure
ITCS-3156-Final/
│
├── notebooks/
│   └── final_project.ipynb     → Main Jupyter notebook (data prep, training, plots)
│
├── figures/
│   ├── mpg_hist.png
│   ├── weight_vs_mpg.png
│   ├── horsepower_vs_mpg.png
│   ├── correlation_heatmap.png
│   └── lms_loss_curve.png
│
├── report/
│   └── final_project_report.pdf → Final written report
│
└── README.md

Dataset

Auto MPG Dataset (Kaggle)
https://www.kaggle.com/datasets/uciml/autompg-dataset

Features include:
cylinders
displacement
horsepower
weight
acceleration
model year
origin

Target variable: mpg
Missing horsepower values were filled using the median.

Models Used
Ordinary Least Squares (OLS)
Uses the closed-form regression equation.

Least Mean Squares (LMS)
Uses gradient descent with a learning rate and number of iterations.

LMS performed better in this project, likely due to multicollinearity in the dataset.

Results Summary
Model	Train RMSE	Test RMSE
OLS	  22.99	      20.65
LMS	  3.37	      2.89

LMS achieved the lowest error after tuning and preprocessing.

Report
The full written report (PDF) is included in the /report folder.

Author
Isaiah Alvarado-Ramirez
UNC Charlotte – ITCS 3156-001
