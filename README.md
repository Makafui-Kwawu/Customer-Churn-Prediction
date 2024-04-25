# 💼 Customer Churn Classification Prediction Project


![Churn photo](https://github.com/Makafui-Kwawu/Customer-Churn-Prediction/assets/160020850/7b7d264b-3365-4f01-a5f6-fe60ab7db44a)

In the dynamic and ever-evolving landscape of the telecommunications industry, customer churn has become a critical challenge for service providers. The ability to predict and understand customer churn can significantly impact business success, customer retention strategies and increase customer service satisfaction.

## Project Overview

This project follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework to explore and analyze customer churn within the Vodafone network service. The aim is to leverage data-driven insights to identify key factors influencing churn, build predictive models, and develop actionable recommendations that can help Vodafone proactively retain valuable customers and enhance their overall service offerings.

## 📑 Table of Contents

- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Data Dictionary](#data-dictionary)
- [Project Highlights](#project-highlights)
- [Summary](#summary)
- [Hypothesis Investigated](#hypothesis-investigated)
  - [Results](#results)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Evaluation (Confusion Matrix)](#model-evaluation-confusion-matrix)
- [Classification Metrics Score](#classification-metrics-score)
- [Recommendations](#recommendations)
- [Getting Started](#getting-started)
- [License](#license)
- [Author](#author)

## Project Structure📂

- `code/`: Contains the dataset used for analysis and the Jupyter notebook detailing the data exploration, preprocessing, and model building steps.
- `article/`: Holds project-related article.
- `customer churn analysis.pbix`: The file for the deployed Power BI dashboard.
- `LICENSE`: Project license.
- `README.md`: Project overview, links, highlights, and information.

## Data Dictionary

| Feature          | Description                                                                                                      |
| ---------------- | ---------------------------------------------------------------------------------------------------------------- |
| Gender           | Whether the customer is a male or a female                                                                       |
| SeniorCitizen    | Whether a customer is a senior citizen or not                                                                    |
| Partner          | Whether the customer has a partner or not (Yes, No)                                                              |
| Dependents       | Whether the customer has dependents or not (Yes, No)                                                             |
| Tenure           | Number of months the customer has stayed with the company                                                        |
| Phone Service    | Whether the customer has a phone service or not (Yes, No)                                                        |
| MultipleLines    | Whether the customer has multiple lines or not                                                                   |
| InternetService  | Customer's internet service provider (DSL, Fiber Optic, No)                                                      |
| OnlineSecurity   | Whether the customer has online security or not (Yes, No, No Internet)                                           |
| OnlineBackup     | Whether the customer has online backup or not (Yes, No, No Internet)                                             |
| DeviceProtection | Whether the customer has device protection or not (Yes, No, No internet service)                                 |
| TechSupport      | Whether the customer has tech support or not (Yes, No, No internet)                                              |
| StreamingTV      | Whether the customer has streaming TV or not (Yes, No, No internet service)                                      |
| StreamingMovies  | Whether the customer has streaming movies or not (Yes, No, No Internet service)                                  |
| Contract         | The contract term of the customer (Month-to-Month, One year, Two year)                                           |
| PaperlessBilling | Whether the customer has paperless billing or not (Yes, No)                                                      |
| Payment Method   | The customer's payment method (Electronic check, mailed check, Bank transfer(automatic), Credit card(automatic)) |
| MonthlyCharges   | The amount charged to the customer monthly                                                                       |
| TotalCharges     | The total amount charged to the customer                                                                         |
| Churn            | Whether the customer churned or not (Yes or No)                                                                  |

# Project Highlights🚀

- Utilized the CRISP-DM framework to thoroughly analyze customer churn in the Vodafone network service.
- Conducted exploratory data analysis to uncover insights and patterns within the dataset.
- Built predictive models using machine learning algorithms like Random Forest Classifier.
- Implemented hyperparameter tuning to optimize model performance.
- Developed a Power BI dashboard for interactive visualization of key findings.
- Published an insightful article detailing the project and its results.

## Summary

| Code | Name                                     |                                             Published Article                                              |                                                                                                                                                    Deployed Dashboard |
| ---- | ---------------------------------------- | :--------------------------------------------------------------------------------------------------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| LP 2 | Customer Churn Classification Prediction | [Read Article](https://medium.com/@sm.kwawu/telco-customer-churn-prediction-a-machine-learning-approach-1d67728b27f9) | [View Dashboard](https://app.powerbi.com/groups/me/reports/edd94735-4684-4700-ad91-f80aa3479239/ReportSection?experience=power-bi) |

## Hypothesis Investigated

**Null Hypothesis (H0)** :The monthly subscription cost (MonthlyCharges) has no significant effect on customer churn (Churn) from the Vodafone network service.

**Alternate Hypothesis (H1)** : The monthly subscription cost (MonthlyCharges) has a significant effect on customer churn (Churn) from the Vodafone network service.

### Results

| Test Conducted               | T-Statistic        | P-Value                |
| ---------------------------- | ------------------ | ---------------------- |
| Mann-Whitney U statistic     | 3100791.0          | 1.2019873209608733e-42 |

The statistical analysis yielded a calculated statistic of `3100791.0`, accompanied by a remarkably low p-value of approximately `1.20e-47`. With this statistical outcome, we confidently reject the null hypothesis and conclude that Monthly Charges exert a substantial influence on customer churn. The p-value indicates that the observed relationship between Monthly Charges and churn is highly unlikely to occur by chance, reinforcing the robustness of our findings.

## Exploratory Data Analysis (EDA)📊

A snapshot of the conducted exploratory data analysis, aimed at addressing pivotal business inquiries during the analysis process.


  |  ![C1](https://github.com/Makafui-Kwawu/Customer-Churn-Prediction/assets/160020850/80d6efad-e393-4086-af30-6fc45a8d7123)  |![C2](https://github.com/Makafui-Kwawu/Customer-Churn-Prediction/assets/160020850/dda8cdae-d896-402e-8bb4-8afefa8421ac)
                                                                                                                                          
                                           
![C3](https://github.com/Makafui-Kwawu/Customer-Churn-Prediction/assets/160020850/5dfd4c2b-3da0-49dc-a590-71b48f7fc322)  ![C4](https://github.com/Makafui-Kwawu/Customer-Churn-Prediction/assets/160020850/30be7148-b6f5-45ac-87e5-3cf169046173)



## Model Evaluation (Confusion Matrix)📉

| Before Hyperparameter Tunning                                                                                                                            | After Hyperparameter Tunning                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![CM1](https://github.com/Makafui-Kwawu/Customer-Churn-Prediction/assets/160020850/19f1bb0f-b0b3-4055-9f0f-e1e664a249e6)
                                                                                                                      |![CM2](https://github.com/Makafui-Kwawu/Customer-Churn-Prediction/assets/160020850/e455ac5e-8f2b-4e9f-84cf-7ca2ac9cfa98)



## Recommendations

1. **Tailor Pricing Strategies:** The analysis reveals that higher monthly charges are associated with an increased likelihood of customer churn. To enhance customer retention, Vodafone can explore competitive pricing strategies that balance revenue generation with customer satisfaction, ensuring that the cost aligns with the value perceived by customers.

2. **Enhance Early Customer Experience:** Early months of customer tenure exhibit a higher churn rate, suggesting that customer experience in the initial stages is vital. Focusing on improving onboarding processes, service quality, and addressing customer concerns during this crucial period can enhance customer satisfaction and loyalty.

3. **Promote Long-Term Contracts:** The analysis indicates that customers with month-to-month contracts have a significantly higher churn rate compared to those with one-year or two-year contracts. Encouraging customers to opt for longer-term contracts through incentives and benefits can potentially reduce churn rates and foster customer commitment.

4. **Leverage Additional Services:** The presence of Online Security and Online Backup services has shown to impact churn rates. Strategically promoting and enhancing these services can play a role in reducing churn rates by providing value-added features that address customer needs and concerns.

5. **Monitor and Adjust Fiber Optic Offering:** Given the higher monthly charges and elevated churn rate among Fiber Optic customers, closely monitor customer satisfaction and service quality for this group. Continuously fine-tune offerings and support to ensure that the premium cost of Fiber Optic service aligns with customer expectations.

6. **Personalized Customer Engagement:** Utilize customer insights from the churn analysis to develop personalized engagement strategies. Tailored communication, offers, and targeted marketing campaigns based on customer tenure, contract type, and service preferences can enhance customer loyalty and mitigate churn.

## Getting Started🏁

1. Clone this repository: `[git clone https://github.com/Makafui-Kwawu/Customer-Churn-Prediction.git]'
2. Navigate to the project directory: `LP2-Customer-Churn-Machine-Learning-Prediction`
3. Explore the Jupyter notebooks for detailed steps and code execution.
4. Check out the Power BI dashboard for interactive visualizations.
5. Read the published article for a comprehensive understanding of the project.

## License📜

This project is licensed under the [MIT License](LICENSE).

## Author✍️

Success Makafui Kwawu

Connect with me on LinkedIn: [LinkedIn Profile](https://linkedin.com/in/smkwawu/)

---

Feel free to star ⭐ this repository if you find it helpful!
