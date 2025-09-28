#  Startups Profit Prediction App

An **interactive Machine Learning application** that predicts the profits of startups based on their expenditures in R&D, Administration, Marketing, and State location. Built with **Python, Scikit-learn, Streamlit, and Joblib**, this project demonstrates the full cycle of a predictive modeling pipeline — from data preprocessing to deployment.

---

## 🔍 Project Overview

Startups often struggle to forecast profitability accurately due to numerous interdependent factors. This project leverages **Multiple Linear Regression** to model the relationship between financial inputs and expected profits. The model is trained on the **50_Startups dataset**, which contains historical data of 50 different startups in various states.

Key insights:

- **R&D Spend** has the most significant impact on profitability.
- **Administration and Marketing Spend** contribute moderately.
- **State location** affects profitability, captured via one-hot encoding.

---

## ⚙️ How It Works

1. **Data Preprocessing**
   - Categorical variable `State` is converted into numeric using **one-hot encoding**.
   - Missing values are checked to ensure data integrity.

2. **Model Training**
   - Dataset is split into **training (80%)** and **testing (20%)** subsets.
   - **Linear Regression** is applied to learn relationships between features (`R&D Spend`, `Administration`, `Marketing`, `State`) and target (`Profit`).
   - Trained model is saved using **Joblib** for future predictions.

3. **Streamlit App**
   - Users enter values for R&D, Administration, Marketing, and select a State.
   - Categorical input (`State`) is manually converted to one-hot encoded features.
   - Model predicts **expected profit** instantly.
   - Interactive visual feedback includes **success messages and celebratory balloons**.

---

## 💡 Features

- **Interactive prediction** using a user-friendly web interface.
- **Model persistence** with Joblib ensures no need to retrain for each session.
- **Realistic simulation** of startup financial decision-making.
- **Extensible design**: easily add more features or datasets to improve predictions.

---

## 📈 How to Run

1. Clone the repository:  
   ```bash
   git clone https://github.com/YusraIsar/Machine-Learning-Projects.git
   ```
2. Navigate to project folder:  
   ```bash
   cd Machine-Learning-Projects/50_Startups
   ```
3. Install dependencies:  
   ```bash
   pip install pandas scikit-learn streamlit joblib numpy
   ```
4. Run the Streamlit app:  
   ```bash
   python -m streamlit run "startup_pred.py"
   ```

---

## 🚀 Potential Applications

- **Startup Planning:** Estimate profits before making investment decisions.  
- **Financial Advisory:** Evaluate impact of budget allocation across departments.  
- **Educational Tool:** Demonstrates full ML workflow: preprocessing → training → deployment.  
- **Scalable Framework:** Can be adapted for larger datasets or other industries.

---

## 🧠 Competitive Advantages

- **End-to-End Pipeline:** Full ML workflow implemented from scratch, suitable for portfolio or resumes.  
- **Interactive Web App:** Makes the project more engaging than just a script.  
- **Insightful Analysis:** Highlights which factors most influence startup profits.  
- **Reproducible and Extensible:** Easy for others to run, modify, or scale with new datasets.

---

## 👩‍💻 Author
Yusra Isar– Machine Learning Enthusiast | Python Developer | Data-Driven Decision Making Advocate

---

## 📄 License

This project is licensed under the **MIT License**. Feel free to use, modify, and share for personal or educational purposes.

---

## ⚡ Fun Tip

💡 Want to experiment? Try increasing R&D spend in the app — you'll see profits soar! This demonstrates how data-driven insights can guide real-world business decisi
ons.
