## Smart Grid Energy Forecasting using Neural Architecture Search (NAS)
**Project Overview**

This project implements a robust time series forecasting pipeline using deep learning models — LSTM, CNN, and Transformer architectures.  
The key feature is hyperparameter tuning with Optuna, which automatically finds the best model configurations to minimize forecasting error.  
The models are trained and evaluated on a multivariate time series dataset, and the best-performing models are saved for later use.

**Dataset Used**

The dataset used in this project is "Household Load and Solar Generation" dataset from kaggle. Due to its large size, the dataset could not be uploaded in the repository. We have specifically used household_data_15min_raw.csv.

Link to access  the dataset: https://www.kaggle.com/datasets/mexwell/household-load-and-solar-generation

**Team Project -**
Dhanya Prabhu

Diya D Bhat- https://github.com/PES2UG23CS183/ML_C_PES2UG23CS183_Diya/tree/main/ML_Project_23

**Features**

- **Models:**  
  - Long Short-Term Memory (LSTM)  
  - 1D Convolutional Neural Network (CNN)  
  - Transformer-based model

- **Hyperparameter Optimization:**  
  - Optuna framework to optimize hyperparameters like number of units, layers, dropout rates, learning rate, batch size, etc.  
  - Early stopping to prevent overfitting.

- **Preprocessing:**  
  - Data normalization/scaling.  
  - Windowing time series data for supervised learning.

- **Model Saving & Loading:**  
  - Models saved using the Keras native format (.keras) for best compatibility.

- **Evaluation:**  
  - Mean Absolute Error (MAE) used to assess model validation performance.

## Running the project
**REQUIRES GPU ACCESS AS THE TRAINING PART TAKES VERY LONG TO COMPLETE DUE TO THE DATASET BEING TOO VAST**
- Step 1: 
Clone the repository.(Alternately you can even download the entire folder as zip)
git clone https://github.com/pes2ug23cs169/ML_C_PES2UG23CS169_Dhanya.git
cd ML_C_PES2UG23CS169_Dhanya/Assignment

- Step 2:
If you have clean data (e.g., household_data_15min_clean.csv), place it in the project folder. 
If using raw data, run the preprocessing cells in the notebook to clean and format it.

- Step 3:
Open Optuna NAS.ipynb to train and evaluate models (LSTM, CNN, Transformer) using Optuna. 
Run Hyperband approach.ipynb for comparison of optimization methods.

- Step 4: 
VIew Results
