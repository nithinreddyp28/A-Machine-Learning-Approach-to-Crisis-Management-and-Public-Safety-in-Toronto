# A Machine Learning Approach to Crisis Management and Public Safety in Toronto

## 🚀 Project Overview

This project aims to **improve crisis management** in Toronto by analyzing **crisis events** and leveraging **machine learning models** to predict patterns and apprehensions. By analyzing factors such as **event types**, **time of day**, and **neighborhoods**, we can provide actionable insights to enhance **public safety** and **crisis response strategies**.

Key findings include identifying **high-risk neighborhoods**, **peak crisis times**, and improving prediction accuracy for **apprehensions** using machine learning techniques like **Logistic Regression**, **Random Forest**, **Gradient Boosting**, and **K-Means Clustering**.

## 🔍 Key Findings

1. **Crisis Event Distribution by Time of Day**:  
   - Suicide-related events peak during early morning (12 AM, 1 AM, 5 AM) and late afternoon (3 PM, 4 PM).
   - Overdose events are most frequent around **4 AM**.
   
2. **High-Risk Neighborhoods**:  
   - High-risk neighborhoods for crisis events: **Moss Park**, **Downtown Yonge East**, **Kensington-Chinatown**.
   - Low-risk areas include: **Princess Resothorn**, **NSA**, **Bayview Woods**.
   
3. **Predictive Modeling Insights**:
   - **Logistic Regression** and **Random Forest** models achieved strong predictive accuracy (up to 85.47%).
   - High recall for **apprehensions** ensures timely intervention.

## 📊 Purpose & Approach

The objective is to predict **crisis events** and **apprehensions** based on various features and patterns. The approach involves:

- **Data Preprocessing**: Encoding features, handling imbalances (SMOTE), and transforming cyclical data (time-related features).
- **Modeling**: Utilizing **Random Forest Classifier**, **Gradient Boosting Classifier**, and **K-Means Clustering** to predict and classify crisis events.
  
Key techniques include:
- **Binary Encoding**: Converting the "Apprehension Made" column to a binary format.
- **Cyclical Feature Encoding**: Using sine and cosine transformations for **hour of the day** to model periodic patterns effectively.

## 🧠 Analysis & Insights

### 1. **Crisis Event Type Distribution by Time of Day**  
   We explored how different crisis event types occur throughout the day and found that **suicide-related events** occur during specific hours while **overdose events** have a clear peak in the early morning.

   ![Crisis Events by Time](https://github.com/user-attachments/assets/159a7587-8402-422f-bc84-1b14c5bfccd5)

### 2. **High-Risk Neighborhoods for Crisis Events**
   We identified **high-risk neighborhoods** for crisis events to enable targeted interventions. Areas like **Moss Park** and **Kensington-Chinatown** had high event frequencies, indicating the need for increased crisis management resources.

   ![High-Risk Neighborhoods](https://github.com/user-attachments/assets/82d55e82-6cdb-4fc5-9abe-2b3598c14702)

## 🔧 Modeling Approach

### **Logistic Regression**
   - **Accuracy**: 85.28%
   - **Precision**: 0.64 (Apprehension Class)
   - **Recall**: 0.94 (Apprehension Class)
   - **Impact**: High recall for apprehensions ensures most events are flagged for intervention.

### **Random Forest Classifier**
   - **Accuracy**: 84.5%
   - **Precision**: 0.64 (Apprehension Class)
   - **Recall**: 0.83 (Apprehension Class)
   - **Impact**: More apprehensions identified but with lower precision than logistic regression, yielding more false positives.

### **Gradient Boosting Classifier**
   - **Accuracy**: 85.47%
   - **ROC AUC**: 0.92 (indicating strong performance)
   - **Impact**: The Gradient Boosting model also showed high recall for apprehensions, critical for public safety.

   ![Feature Importance](https://github.com/user-attachments/assets/e22fb984-6c85-40e8-93b7-b24463a9a2fa)

### **K-Means Clustering**
   - **Purpose**: Group crisis events by type and occurrence.
   - **Impact**: Clusters help prioritize response efforts based on event types like **overdose** and **person in crisis**.

   ![K-Means Clustering](https://github.com/user-attachments/assets/65bed612-117a-4636-bf4d-38b637d05a74)

## 🔮 Key Insights for Crisis Management

- **Time of Day (EVENT_HOUR)**: Critical for modeling crisis events, as specific hours see more frequent types of crises.
- **Event Type**: **Suicide-related** and **Person in Crisis** events are most likely to lead to apprehensions.
- **High-Risk Neighborhoods**: Areas like **Moss Park** and **Kensington-Chinatown** require increased crisis response strategies.
- **Occurrence Status**: The likelihood of apprehension increases significantly when an official **OCCURRENCE_CREATED** status is recorded.

## 🌍 Impact on Public Safety

### Benefits:
1. **Targeted Resource Allocation**: Increased focus on high-risk neighborhoods and peak crisis times.
2. **Enhanced Crisis Management**: Models provide insights into when and where to prioritize intervention.
3. **Preventive Measures**: Early predictions help prevent potential harm by anticipating crisis events before they escalate.

### Dataset
https://open.toronto.ca/dataset/persons-in-crisis-calls-for-service-attended/
