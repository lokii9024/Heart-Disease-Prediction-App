# Heart Disease Prediction with SVM

A machine learning web application that predicts the risk of heart disease using Support Vector Machine (SVM) algorithm. Built with Streamlit for an interactive user experience.

## 🚀 Features

- **Interactive Web Interface**: User-friendly Streamlit application for easy input of patient data
- **SVM Model**: Trained Support Vector Machine classifier for accurate predictions
- **Real-time Predictions**: Instant risk assessment with probability scores
- **Comprehensive Input**: 13 health parameters including age, blood pressure, cholesterol, etc.
- **Visual Feedback**: Clear risk indicators with color-coded results

## 📊 Dataset

This model is trained on the Cleveland Heart Disease dataset, which contains 303 patient records with 13 clinical features:

- Age
- Sex
- Chest pain type (4 values)
- Resting blood pressure
- Serum cholesterol
- Fasting blood sugar > 120 mg/dl
- Resting electrocardiographic results (3 values)
- Maximum heart rate achieved
- Exercise induced angina
- ST depression induced by exercise
- Slope of the peak exercise ST segment
- Number of major vessels colored by fluoroscopy
- Thalassemia (3 values)

## 🛠️ Installation

1. **Clone the repository** (if applicable) or ensure you have the project files

2. **Create a virtual environment** (recommended):
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**:
   - Windows:
     ```bash
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## 🎯 Usage

1. **Run the Streamlit application**:
   ```bash
   streamlit run app.py
   ```

2. **Access the web interface**:
   - Open your browser and go to `http://localhost:8501`

3. **Enter patient information**:
   - Fill in all the required health parameters
   - Click the "Predict" button

4. **View results**:
   - The app will display the risk level (High/Low)
   - Probability score is provided for confidence assessment

## 🤖 Model Details

- **Algorithm**: Support Vector Machine (SVM)
- **Kernel**: RBF (Radial Basis Function)
- **Features**: 13 clinical parameters
- **Target**: Binary classification (0 = No disease, 1 = Disease present)
- **Performance**: Trained for optimal accuracy on heart disease prediction

## 📋 Requirements

- Python 3.7+
- Streamlit
- Scikit-learn
- Pandas
- NumPy
- Joblib

## 📁 Project Structure

```
heart-disease-prediction/
│
├── app.py                 # Main Streamlit application
├── svm_model.pkl         # Trained SVM model
├── scaler.pkl            # Feature scaler
├── requirements.txt      # Python dependencies
└── README.md            # Project documentation
```

## 🔬 Input Parameters

| Parameter | Description | Range/Type |
|-----------|-------------|------------|
| Age | Patient age in years | 20-100 |
| Sex | Gender (0=Female, 1=Male) | 0 or 1 |
| Chest Pain Type | Type of chest pain | 0-3 |
| Resting BP | Resting blood pressure | Numeric |
| Cholesterol | Serum cholesterol | Numeric |
| Fasting BS | Fasting blood sugar >120 | 0 or 1 |
| Rest ECG | Resting ECG results | 0-2 |
| Max HR | Maximum heart rate | Numeric |
| Exercise Angina | Exercise induced angina | 0 or 1 |
| Oldpeak | ST depression | Numeric |
| Slope | Peak exercise ST slope | 0-2 |
| CA | Major vessels count | 0-3 |
| Thal | Thalassemia | 0-3 |

## ⚠️ Disclaimer

This application is for educational and demonstration purposes only. It should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult with qualified healthcare professionals for medical decisions.

## 🤝 Contributing

Feel free to submit issues, feature requests, or pull requests to improve this project.

## 📄 License

This project is open source and available under the MIT License.