# Bank Marketing Analysis

This repository contains an analysis of a Bank Marketing dataset using three regression models:
1. Decision Tree Regressor
2. Random Forest Regressor
3. Linear Regression

## Dataset

The dataset used in this analysis is the Bank Marketing dataset. The data includes customer details such as age, profession, marital status, education, and their interactions with the bank's marketing campaigns. The target variable is whether the customer subscribed to a deposit (1) or not (0).

### Columns in the Dataset
- **Age**: Age of the customer
- **Profession**: Profession category
- **Marital_Status**: Marital status of the customer
- **Education**: Educational qualification
- **Defaulter**: Whether the customer is a defaulter
- **Average_Balance**: Average account balance
- **Own_House**: Whether the customer owns a house
- **Loans**: Whether the customer has loans
- **ContactBy**: Communication type
- **CDay**: Contact day
- **CMonth**: Contact month
- **Duration**: Duration of the last contact
- **Campaign**: Number of contacts during this campaign
- **Pdays**: Number of days since the customer was last contacted
- **Previous**: Number of previous contacts
- **Poutcome**: Outcome of the previous campaign
- **Deposit**: Target variable (1 for subscription, 0 otherwise)

## Regression Models and Results

### 1. Decision Tree Regressor
- **Model Parameters**: 
  - Criterion: Mean Squared Error (MSE)
  - Random State: 0
- **Performance**:
  - Coefficient of Determination (Train): 1.0
  - R-squared (Test): N/A due to fitting error

### 2. Random Forest Regressor
- **Model Parameters**:
  - Number of Estimators: 100
  - Criterion: Mean Squared Error (MSE)
  - Random State: 42
- **Performance**:
  - Coefficient of Determination (Train): 0.9999
  - R-squared (Test): 0.8654
  - Mean Absolute Error: 0.034
  - Mean Squared Error: 0.013
  - Root Mean Squared Error: 0.113

### 3. Linear Regression
- **Model Parameters**:
  - Fit Intercept: True
- **Performance**:
  - Coefficient of Determination (Train): 0.274
  - R-squared (Test): 0.270
  - Intercept: 0.392
  - Mean Absolute Error: 0.369
  - Mean Squared Error: 0.183
  - Root Mean Squared Error: 0.428

## Usage

### Prerequisites
1. Python 3.x
2. Required Libraries: 
   - pandas
   - numpy
   - matplotlib
   - scikit-learn

### Steps to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Monish-Nallagondalla/Agentic_Ai_Practice.git
   ```
2. Navigate to the project directory and activate your virtual environment if necessary.
   ```bash
   cd Agentic_Ai_Practice
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebook or Python scripts in the repository.

## File Structure
- **Bank_Marketing.csv**: Dataset used for training and testing the models.
- **notebook.ipynb**: Contains the Python code for preprocessing, training, testing, and evaluating the models.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---
