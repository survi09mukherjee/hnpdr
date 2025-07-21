# 🧬 HNPDR – Healthcare Needs Prediction and Disease Risk Estimator

![Tech](https://img.shields.io/badge/Tech-Python%20%7C%20Machine%20Learning%20%7C%20Streamlit%20%7C%20MySQL-informational)

> HNPDR is a smart health analytics system designed to predict medical needs and assess potential disease risks using machine learning and patient data.

---

## 🩺 Key Features

- 🔍 **Healthcare Needs Prediction**:  
  Suggests future healthcare services based on patient demographics, medical history, and behavior patterns.

- ⚠️ **Disease Risk Detection**:  
  Estimates risk level for chronic and lifestyle diseases (e.g., diabetes, heart disease).

- 📈 **ML-Powered Predictions**:  
  Supports multiple models including Logistic Regression, Decision Trees, Random Forest, and Neural Networks.

- 🧠 **Explainability with SHAP**:  
  Visualizes the impact of each input feature on the prediction.

- 🧾 **Secure Data Logging**:  
  Saves predictions and inputs to a MySQL database for further analysis.

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit  
- **Backend**: Python  
- **ML Libraries**: Scikit-learn, SHAP, Pandas, NumPy  
- **Database**: MySQL  
- **Optional**: Flask API wrapper for remote access

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/survi09mukherjee/hnpdr.git
cd hnpdr
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:
```bash
pip install streamlit scikit-learn pandas numpy shap mysql-connector-python
```

### 3. Launch the App

```bash
streamlit run app.py
```

---

## 🗃️ Database Configuration (MySQL)

1. Create a MySQL database named `hnpdr_db`:
   ```sql
   CREATE DATABASE hnpdr_db;
   ```

2. Update DB credentials in `db_utils.py`:
   ```python
   connection = mysql.connector.connect(
       host="localhost",
       user="root",
       password="yourpassword",
       database="hnpdr_db"
   )
   ```

3. Run the app and test the prediction logging.

---

## 📸 Screenshots

> _(Add images inside an `assets/` folder and update paths accordingly)_

| Prediction Form | Risk Visualization | SHAP Explainability |
|------------------|--------------------|----------------------|

<img width="712" height="519" alt="og helmet" src="https://github.com/user-attachments/assets/84838bcd-2f0e-46ae-85a0-33fe04e4554f" />
<img width="560" height="432" alt="og non helmet" src="https://github.com/user-attachments/assets/387569c6-332e-4583-a767-a233bc337967" />
<img width="1000" height="600" alt="accuracy_over_images (1)" src="https://github.com/user-attachments/assets/1d9a3470-f4ae-4891-a4e1-1a04c23e6242" />
<img width="1000" height="500" alt="Training_and_Validation_Loss" src="https://github.com/user-attachments/assets/45e5ee97-d80b-4c6d-9bbf-a965f1c22c3b" />
<img width="1000" height="500" alt="Model_Accuracy" src="https://github.com/user-attachments/assets/b022f6b5-f3de-4d85-88b7-4ecbacb437e5" />
<img width="1901" height="880" alt="2" src="https://github.com/user-attachments/assets/e9319d67-6415-4706-87a7-728f52fe41c7" />
<img width="1901" height="880" alt="2" src="https://github.com/user-attachments/assets/bdde99de-7c5e-47a9-9dd7-f617d36b4ef7" />
<img width="1901" height="880" alt="2" src="https://github.com/user-attachments/assets/48283361-46b2-42a7-a609-dda1128fd9d4" />
<img width="1898" height="883" alt="1" src="https://github.com/user-attachments/assets/c403bf8a-d910-4547-86bd-1f47ff5725d0" />
<img width="1901" height="880" alt="2" src="https://github.com/user-attachments/assets/238dbc3c-a62b-46aa-b518-19ea4d0eb1d2" />
<img width="1901" height="880" alt="2" src="https://github.com/user-attachments/assets/73b28b1e-041e-4121-954a-81dc796f7fbd" />
<img width="1901" height="880" alt="2" src="https://github.com/user-attachments/assets/572a5574-2123-4977-8771-660568def3ac" />
<img width="1901" height="880" alt="2" src="https://github.com/user-attachments/assets/8500ef45-8b50-4f18-b2a7-965ac07f274e" />
<img width="1919" height="881" alt="5" src="https://github.com/user-attachments/assets/f1dffeb4-755d-4af1-88c4-ce1ce2af374c" />

---

## 📂 Folder Structure

```
hnpdr/
├── app.py                  # Streamlit app
├── db_utils.py             # MySQL database connector
├── models/                 # Saved ML models
├── logs/                   # Prediction logs
├── utils/                  # SHAP and helper functions
├── requirements.txt
└── README.md
```

---

## 🔮 Future Improvements

- Integrate real-time wearable device data  
- Build patient dashboards with charts  
- Enable live doctor recommendations using NLP  
- Add multi-disease ensemble models  
- Deploy as a cloud-based health intelligence API

---



## 👩‍💻 Author

**Survi Mukherjee**  
🔗 [GitHub](https://github.com/survi09mukherjee)  
🌐 [Portfolio](https://survimukherjeeportfolio.framer.website/)

---

## 🌟 Support

If you found this helpful, please ⭐ star the repo and share it with others!
