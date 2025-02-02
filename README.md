AI Predictive Methods for Credit Underwriting

This project is a Streamlit-powered application designed to predict loan approval outcomes using machine learning. It allows users to input various details and receive a prediction on whether their loan application will be approved or rejected. Additionally, the app generates a downloadable PDF report containing detailed insights and results.

Key Features

Interactive Web Interface: Developed with Streamlit for a user-friendly and responsive experience.
User Input Fields: Includes options for CIBIL score, income, loan amount, loan term, and more.
Prediction Model: Employs a pre-trained machine learning model to assess loan approval status.
Downloadable PDF Report: Produces a professional PDF summarizing predictions and user inputs.
EMI Calculator: Computes monthly EMI based on loan amount, interest rate, and term.
AI Chatbot: Offers financial advice and assists with loan-related questions.
Custom Styling: Enhanced with custom CSS for an improved user interface.

Technologies Utilized

Python: The primary programming language for the application.
Streamlit: Framework for building the interactive web interface.
FPDF: Library for creating downloadable PDF reports.
pandas: Used for data preparation and managing user inputs.
matplotlib: Optional for generating visualizations.
joblib: For loading the pre-trained machine learning model.
transformers: For NLP-based chatbot responses (using pre-trained models).
langdetect: For language detection (used in the chatbot).
Prerequisites

Ensure the following are installed on your system:

Python 3.7+
pip (Python package manager)
Install Dependencies

Run the following command to install all necessary libraries:

pip install -r requirements.txt
requirements.txt File Includes:

streamlit
pandas
matplotlib
joblib
fpdf2
transformers
langdetect
How to Run


Install Dependencies:

pip install -r requirements.txt
Run the Application:

streamlit run streamlit_app.py
Open the provided local URL in your browser to access the app.

File Structure

├── streamlit_app.py  # Main application file
├── best_features_model.pkl  # Pre-trained machine learning model file
User Inputs

The app provides the following input fields in the sidebar:

CIBIL Score (300-900)
Annual Income (INR)
Loan Amount (INR)
Loan Term (months)
Number of Active Loans
Gender
Marital Status
Employment Status
Residence Type
Loan Purpose
Output

Loan Status: Displays whether the loan is Approved or Rejected.
Prediction Probabilities: Shows the probability of approval and rejection.
Downloadable PDF Report:
Prediction results.
Input details provided by the user.
Summary of probabilities.
Deployment

The application is live and can be accessed at: AI Predictive Methods for Credit Underwriting

To deploy the app on Streamlit Cloud:

Push the project to GitHub.
Connect your GitHub repository to Streamlit Cloud.
Ensure requirements.txt is present for dependency installation.
Deploy and access your app via the Streamlit Cloud link.
Troubleshooting

Missing Library Error

If you encounter an error like ModuleNotFoundError: No module named 'fpdf', install it manually:

pip install fpdf
Unicode Character Error (₹ Symbol)

Ensure you have a Unicode-compatible font (e.g., FreeSerif.ttf) in your working directory. Update the PDF font registration in the code if necessary.

License

This project is licensed under the MIT License. See the LICENSE file for details.
