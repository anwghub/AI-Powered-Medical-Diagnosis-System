# Implementation-of-AI-Powered-Medical-Diagnosis-System-P2
### Project Title
AI-Powered Disease Prediction Tool
---

### Overview of the AI-Powered Medical Diagnosis System
Project Overview
This system leverages AI to help doctors diagnose diseases faster and more accurately using machine learning models like Logistic Regression and Support Vector Machines (SVM). It analyzes various medical data such as symptoms, test results, and medical images. The system is integrated into an easy-to-use Streamlit web app for real-time diagnostics.

Disease Prediction Models
Diabetes: Predicts diabetes risk based on medical features using Logistic Regression and SVM.
Heart Disease: Predicts the likelihood of heart disease based on medical and lifestyle data.
Thyroid Disease: Uses preprocessed data for predicting hypo- and hyperthyroidism.
Parkinson's Disease: Predicts Parkinson's risk from voice measurements.
Lung Cancer: Predicts lung cancer risk based on medical data.
---

### Why It's Important

- **Improved Accuracy**: Reduces human error and identifies patterns that are difficult for doctors to spot.
- **Faster Decision-Making**: Quick predictions help doctors make informed decisions, crucial in critical situations.
- **Accessibility**: Makes diagnostic tools available in underserved areas with limited medical resources.
- **Personalized Treatment**: Tailors treatment plans based on patient data.
- **Cost-Effective**: Minimizes unnecessary tests and streamlines the diagnostic process, reducing costs.
---

### Installation
Follow these steps to run the project locally:

1. **Clone the Repository**:
   ```bash
   [git clone https://github.com/yourusername/ai-medical-diagnosis.git](https://github.com/anwghub/AI-Powered-Medical-Diagnosis-System)
   cd AI-Powered-Medical-Diagnosis-System

2. **Set Up Virtual Environment:**
   ```bash
   python -m venv env
   source env/bin/activate  # On macOS/Linux
   .\env\Scripts\activate  # On Windows

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt

4. **Run:**
    ```bash
   streamlit run app.py
---

### Technologies Used

- **Python**: The main programming language used to develop the application and machine learning models.
- **Streamlit**: A powerful Python library for creating interactive web applications. It is used to deploy and visualize the machine learning models as a user-friendly web app.
- **Scikit-learn**: A machine learning library in Python that provides implementations of models like **Logistic Regression** and **Support Vector Machine (SVM)**.
- **Pandas**: Used for data manipulation, cleaning, and preprocessing.
- **NumPy**: Used for numerical computations and handling arrays.
- **Matplotlib** and **Seaborn**: For visualizing data, model performance, and results.
- **GitHub**: For version control, collaboration, and hosting the project code.
- **Streamlit Cloud** : The platform where the app is deployed, making it accessible for users worldwide.

These technologies were chosen for their flexibility, simplicity, and their ability to integrate well into an efficient workflow for deploying machine learning models as web applications.
---

### Dataset

This project uses 5 different datasets, each corresponding to a specific disease. The datasets have been preprocessed to handle missing values, normalize the data, and ensure consistency for model training and prediction. The datasets are as follows:

1. **Diabetes Data**:
   - **Description**: Contains medical data for predicting whether a person is likely to have diabetes or not.
   - **Features**: Age, BMI, blood pressure, insulin levels, and other medical factors.
   - **Preprocessing**: The dataset has been cleaned by handling missing values and normalizing numerical features for accurate model predictions.

2. **Heart Disease Data**:
   - **Description**: This dataset is used to predict the likelihood of a person having heart disease based on features like age, cholesterol levels, and exercise habits.
   - **Features**: Age, cholesterol, resting blood pressure, ECG results, maximum heart rate, etc.
   - **Preprocessing**: Missing values were imputed, and categorical variables were encoded.

3. **Hypothyroid Data** (Preprocessed):
   - **Description**: This dataset helps in diagnosing hypothyroidism (underactive thyroid) and hyperthyroidism (overactive thyroid).
   - **Features**: TSH, T3, T4, FTI, and other blood test results.
   - **Preprocessing**: The dataset has been preprocessed by handling missing values and normalizing numerical features.

4. **Parkinson's Disease Data**:
   - **Description**: This dataset is used to predict the presence of Parkinson's disease based on voice measurements.
   - **Features**: Fundamental frequency, jitter, shimmer, and other voice-related features.
   - **Preprocessing**: The dataset is already well-cleaned and does not require much preprocessing. Feature scaling was applied to certain features.

5. **Lung Cancer Data**:
   - **Description**: The dataset is used to predict the likelihood of lung cancer based on medical imaging and other factors.
   - **Features**: Age, smoking history, radiological findings, and other medical factors.
   - **Preprocessing**: Data was cleaned by handling missing values and categorical encoding applied where needed.

#### Preprocessed Hypo and Hyperthyroid Data

- **Hypothyroid and Hyperthyroid Data**: These two datasets were merged and preprocessed to create one unified dataset that predicts both conditions.
  - **Preprocessing Steps**:
    - Handling missing values using mean or mode imputation.
    - Feature scaling to bring all features to the same scale.
    - Encoding categorical variables into numerical form.
    - Removal of duplicate and irrelevant records to ensure clean data for training the models.
---

### **Project Structure**
📂 AI-POWERED-MEDICAL-DETECTION  
├── 📂 dataset/  
│   ├── 📄 diabetes_data.csv  
│   ├── 📄 heart_disease_data.csv  
│   ├── 📄 hypothyroid.csv  
│   ├── 📄 parkinson_data.csv  
│   ├── 📄 preprocessed_hypothyroid.csv  
│   ├── 📄 preprocessed_hyperthyroid.csv  
│   ├── 📄 preprocessed_lungs_data.csv  
│   ├── 📄 survey_lung_cancer.csv  
│  
├── 📂 Models/  
│   ├── 📄 diabetes_model.sav  
│   ├── 📄 heart_disease_model.sav  
│   ├── 📄 lungs_disease_model.sav  
│   ├── 📄 parkinsons_model.sav  
│   ├── 📄 Thyroid_model.sav  
│  
├── 📂 notebooks/  
│   ├── 📄 diabetes_detection.ipynb  
│   ├── 📄 heart_disease_detection.ipynb  
│   ├── 📄 lung_cancer.ipynb  
│   ├── 📄 parkinson_disease.ipynb  
│   ├── 📄 thyroid_detection.ipynb  
│  
├── 📂 venv/  
├── 📄 .gitignore  
├── 📄 app.py  
├── 📄 README.md  
├── 📄 requirements.txt  
---

### **Usage**

1. **Enter Input Values**: If you don’t have a dataset, you can manually input data such as:
   - **Symptoms**: Enter the value symptoms you're experiencing.
   - **Test Results**: Input medical test results (e.g., blood pressure, glucose levels).
   
2. **Click Predict**: After entering the values, click on the **Test Results** button to get real-time diagnostic insights.

3. **View Results**: The system will provide a prediction, telling you whether you are at risk of a particular disease based on the input data.
---

