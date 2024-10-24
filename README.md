# Health Insurance Cross-Sell Prediction

## Project Overview

This project aims to predict whether a customer will buy vehicle insurance in the following year based on the data provided. The model is built using a dataset that includes customer demographic information, previous insurance history, and vehicle details. By predicting cross-sell opportunities, insurance companies can target marketing efforts more effectively and improve customer acquisition.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Building](#model-building)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset contains information about potential customers, including:
- **Demographic data**: Age, gender, driving license status, etc.
- **Vehicle information**: Vehicle age, type, etc.
- **Insurance history**: Claims and policy details.
  
The target variable is whether a customer will purchase vehicle insurance (`Response`: 0 = No, 1 = Yes).

### Feature Overview:
- `ID`: Unique identifier for each customer.
- `Gender`: Gender of the customer.
- `Age`: Age of the customer.
- `Driving_License`: Whether the customer holds a valid driving license (1: Yes, 0: No).
- `Region_Code`: Code for the customer's region.
- `Previously_Insured`: Whether the customer already has vehicle insurance (1: Yes, 0: No).
- `Vehicle_Age`: Age of the vehicle.
- `Vehicle_Damage`: Whether the customer has experienced vehicle damage in the past.
- `Annual_Premium`: The amount paid by the customer as the insurance premium.
- `Policy_Sales_Channel`: Code for the sales channel through which the customer was acquired.
- `Vintage`: Number of days the customer has been associated with the company.
- `Response`: The target variable (1: Will buy insurance, 0: Will not buy insurance).

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/health-insurance-cross-sell-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd health-insurance-cross-sell-prediction
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Open the Jupyter Notebook (`HEALTH_INSURANCE_CROSS_SELL_PREDICTION.ipynb`) to explore the data, preprocess it, and train the predictive models.
2. Run the notebook cells to perform the following tasks:
   - Data exploration and preprocessing
   - Feature engineering
   - Model selection and training
   - Model evaluation

3. The notebook includes code to evaluate multiple machine learning models, including decision trees, random forests, and gradient boosting classifiers.

## Model Building

The predictive model is built using the following steps:
1. **Data Preprocessing**: Handling missing values, encoding categorical variables, and scaling numerical features.
2. **Feature Engineering**: Creating new features to capture important customer characteristics.
3. **Model Training**: Various machine learning algorithms are used for prediction:
   - Logistic Regression
   - Decision Trees
   - Random Forest
   - Gradient Boosting Machines (GBM)
   - XGBoost
   
   Hyperparameter tuning is conducted to improve model performance.
   
4. **Evaluation**: The models are evaluated based on accuracy, precision, recall, and AUC-ROC.

## Results

The final model achieved high accuracy and a strong AUC-ROC score, indicating its effectiveness in predicting cross-sell opportunities. Detailed results can be found in the notebook.

## Contributing

Contributions to improve the model, dataset, or overall project structure are welcome. To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add some feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-branch
   ```
5. Submit a pull request.

## License

This project is licensed under the MIT License.
