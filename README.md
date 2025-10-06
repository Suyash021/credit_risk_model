# credit_risk_model

A credit risk modeling application built in Python, designed to help financial institutions assess and predict the risk associated with lending to borrowers.

## Features

- **Streamlit Web App**: Interactive user interface for inputting borrower details and visualizing credit risk results.
- **Predictive Modeling**: Utilizes a trained machine learning model to estimate the probability of default, credit score, and risk rating.
- **Customizable Inputs**: Users can enter borrower demographics, financial, and loan-related information.
- **Automated Feature Engineering**: Calculates ratios and transforms input data for model compatibility.

## Getting Started

### Prerequisites

- Python 3.8+
- Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```

### Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Suyash021/credit_risk_model.git
   cd credit_risk_model
   ```

2. Ensure the trained model artifact is present at `artifacts/model_data.joblib`.

3. Run the Streamlit app:
   ```bash
   streamlit run main.py
   ```

4. Open the local web app in your browser to input borrower details and get risk predictions.

## How It Works

- The app collects borrower attributes such as age, income, loan amount, credit utilization, delinquency ratios, account details, and more.
- It prepares feature vectors, applies scaling, and feeds the input into a pre-trained predictive model.
- Outputs include:
  - Default Probability
  - Credit Score
  - Risk Rating

## File Structure

- `main.py`: Streamlit web interface for user interaction.
- `prediction_helper.py`: Model loading, input preparation, prediction, and scoring logic.
- `artifacts/model_data.joblib`: Serialized model and scaler (must be generated separately).

## License

This project is licensed under the [MIT License](LICENSE).

---

For more details, see the [GitHub repository](https://github.com/Suyash021/credit_risk_model).
