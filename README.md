
# 📊 SDG 3.1 Maternal Health Prediction using IBM AutoAI

## 📌 Project Overview

This project focuses on **tracking maternal health progress toward Sustainable Development Goal (SDG) 3.1**, which aims to reduce the **global Maternal Mortality Ratio (MMR) to less than 70 per 100,000 live births by 2030**.

We use the **AI Kosh dataset (National Indicator Framework v3.1, 2021)** from [data.gov.in](https://www.data.gov.in/resource/sustainable-development-goals-national-indicator-framework-version-31-2021), along with **IBM Watsonx.ai AutoAI** on **IBM Cloud Lite**, to build and deploy machine learning models for predicting MMR and analyzing its key drivers.

---

## 🎯 Problem Statement

Despite global efforts, maternal health outcomes vary significantly across regions, income groups, and healthcare systems. Monitoring and predicting MMR is crucial for effective policymaking.
Key influencing indicators include:

* Antenatal care coverage (ANC visits)
* Skilled birth attendance (%)
* Adolescent birth rate
* Current health expenditure (% of GDP)

---

## ✅ Proposed Solution

* **Data Collection:** AI Kosh NIF dataset (2021) — MMR & related health indicators.
* **Data Preprocessing:** Cleaning, handling missing values, ensuring numeric DataValue.
* **Modeling:** IBM Watsonx.ai AutoAI automatically built multiple regression pipelines.
* **Deployment:** Best pipeline (Decision Tree Regressor) deployed as an **online REST API**.
* **Prediction:** Returns real-time MMR predictions from given input values.
 
---

## 🛠️ System Development Approach

* **Platform:** IBM Cloud Lite (Watsonx.ai Studio, AutoAI, Data Refinery, Deployment Spaces)
* **Language/Tools:** Python (for preprocessing & EDA), IBM AutoAI (for modeling)
* **Dataset:** AI Kosh – National Indicator Framework v3.1 (2021), data.gov.in

---

## 🤖 Algorithm & Deployment

* **Algorithm Selection:** AutoAI tested multiple models → best performer: **Decision Tree Regressor** (RMSE ≈ 73.8).
* **Input Features:** Skilled Birth Attendance, ANC Coverage, Adolescent Birth Rate, Health Expenditure, Year, Region.
* **Target Variable:** Maternal Mortality Ratio (per 100,000 live births).
* **Deployment:** Model deployed as **Online REST API** → accepts JSON/CSV inputs and returns predictions.

---

## 📈 Results

* **Best Model:** Decision Tree Regressor (RMSE \~73.8)
* **Sample Prediction:** Input (India, 2015–16, Indicator: MMR) → Output ≈ **138.54** per 100,000 live births
* **Screenshots included:**

  * AutoAI Leaderboard
  * Deployment Test Results (JSON prediction output)

---

## 📝 Conclusion

* A working ML pipeline was successfully built and deployed on IBM Cloud Lite.
* AutoAI enabled automated data preprocessing, feature engineering, and model optimization.
* Deployment provides **real-time predictions** for MMR, useful for **policy simulations and forecasting**.

---

## 🔮 Future Scope

* Expand dataset with WHO/UN maternal health indicators (global coverage).
* Implement **time-series forecasting** up to 2030.
* Create **what-if analysis dashboards** to test effects of increasing ANC or Skilled Birth Attendance.
* Extend framework to other SDG health indicators (child mortality, healthcare access).

---

## 📚 References

* WHO – [SDG 3.1: Maternal Mortality](https://www.who.int/data/gho/data/themes/topics/topic-details/GHO/sdgtarget3-1-reduce-maternal-mortality)
* UN Sustainable Development Goals – [Goal 3: Good Health and Well-being](https://sdgs.un.org/goals/goal3)
* MoSPI (India) – [National Indicator Framework v3.1 (2021)](https://www.data.gov.in/resource/sustainable-development-goals-national-indicator-framework-version-31-2021)
* IBM Cloud Docs – [Watsonx.ai AutoAI & Deployment](https://www.ibm.com/docs/en/watsonx/saas?topic=cloud-watsonxai-studio-plans)

---
## 📝 Jupyter Notebook

For exploratory data analysis (EDA) and preprocessing, we used a Jupyter Notebook before uploading data into AutoAI.


📓 **Jupyter Notebook**
👉 Open Notebook 

[SDG31_MaternalHealth_Model.pdf](https://github.com/user-attachments/files/21955911/SDG31_MaternalHealth_Model.pdf)

---

##  Acknowledgments

This project was developed as part of the **Capstone Project** under Problem Statement 3: *Tracking Maternal Health Progress Toward SDG 3.1*.

Special thanks to:

* **AI Kosh (MoSPI – National Indicator Framework v3.1, 2021)** for providing the dataset.
* **IBM Cloud Lite / Watsonx.ai AutoAI** for enabling automated machine learning, model deployment, and experimentation.
* Edunet Foundation


---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 👨‍💻 Developed by

**Soumen Bhunia**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/soumen-bhunia/)

---
