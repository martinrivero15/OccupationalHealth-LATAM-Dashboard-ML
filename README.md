# OccupationalHealth-LATAM-Dashboard-ML
This project simulates a realistic occupational health data analysis environment for a multinational company operating across Latin America. The goal is to build interactive dashboards, predictive models, and integrated machine learning services.
# 🏥 LATAM Occupational Health Analytics

This project simulates a realistic occupational health data analysis environment for a multinational company operating across Latin America. The goal is to build interactive dashboards, predictive models, and integrated machine learning services.

---

## 📌 Project Objectives

1. **Synthetic Data Generation**  
   We use Python to create a synthetic dataset representing 1,000 employees working in 20 different LATAM cities.  
   Key simulated variables include age, gender, location, absenteeism, workplace accidents, medical indicators (BMI, cholesterol, smoking status), and monthly KPIs by department.

2. **Data Visualization with Power BI**  
   Based on the generated tables, we designed interactive dashboards in Power BI to explore:
   - Geographic distribution of employees
   - Health indicators by location
   - Departmental/sector comparisons
   - Monthly KPI trends (absenteeism, accidents, active employees)
📽️ **Dashboard Walkthrough Video**  
Watch a short demo of the Power BI dashboard in action:  
👉 [YouTube Video – Power BI Dashboard Overview](https://www.youtube.com/watch?v=O7O_9dIz7y4)

<p align="center">
  <a href="https://www.youtube.com/watch?v=O7O_9dIz7y4" target="_blank">
    <img src="https://img.youtube.com/vi/O7O_9dIz7y4/0.jpg" alt="Dashboard Video" width="600"/>
  </a>
</p>

3. **Machine Learning Models in Python**  
   Using libraries such as `numpy`, `pandas`, `matplotlib`, `seaborn`, and `scikit-learn`, we developed models to:
   - Predict long-term absenteeism risk
   - Identify employees unfit for work
   - Classify employees into health risk profiles

4. **Model Deployment with FastAPI**  
   The final ML model is deployed as a REST microservice using `FastAPI`, enabling integration with external systems.

5. **Power BI Integration with FastAPI**  
   Power BI connects to the API endpoint to dynamically consume model predictions and enrich dashboards with real-time insights.

---

## 🛠️ Technologies Used

- **Python**: `pandas`, `numpy`, `faker`, `scikit-learn`, `matplotlib`, `seaborn`, `FastAPI`
- **Power BI**: Interactive dashboards connected to CSV/API
- **DAX**: Dynamic measures within Power BI
- **Git/GitHub**: Version control and documentation
- **JSON / CSV**: Formats for data exchange and API communication
---
## 📂 Project Structure

```plaintext
01_data/
├── employees.csv
├── health_events.csv
├── medical_evaluations.csv
└── monthly_kpis.csv

02_powerbi/
└── dashboard.pbix

03_notebooks/
├── 01_generate_synthetic_data.ipynb
├── 02_eda_visualization.ipynb
└── 03_ml_models.ipynb

04_api/
├── app.py        # FastAPI server
└── model.pkl     # Trained ML model
