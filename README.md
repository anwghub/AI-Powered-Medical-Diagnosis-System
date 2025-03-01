# Implementation-of-AI-Powered-Medical-Diagnosis-System-P2
### Project Title
AI-Powered Disease Prediction Tool

---

### Overview of the AI-Powered Medical Diagnosis System
This system uses AI to help doctors diagnose diseases faster and more accurately. By applying machine learning techniques like Logistic Regression and Support Vector Machines (SVM), it can analyze a wide variety of medical data—everything from symptoms and test results to medical images. The best part? It’s all wrapped up in an easy-to-use Streamlit web app, making it super simple for users to input data and get real-time diagnostic insights.

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

### **Project Structure**

---

### **Usage**

1. **Enter Input Values**: If you don’t have a dataset, you can manually input data such as:
   - **Symptoms**: Enter the value symptoms you're experiencing.
   - **Test Results**: Input medical test results (e.g., blood pressure, glucose levels).
   
2. **Click Predict**: After entering the values, click on the **Test Results** button to get real-time diagnostic insights.

3. **View Results**: The system will provide a prediction, telling you whether you are at risk of a particular disease based on the input data.

---

