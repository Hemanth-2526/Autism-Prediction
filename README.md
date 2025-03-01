# **Autism Prediction Using Machine Learning**  

## **Project Overview**  
This project aims to predict Autism Spectrum Disorder (ASD) using machine learning techniques. Early detection is crucial for timely intervention, and this model utilizes behavioral assessment data to classify individuals as either at risk or not at risk of ASD.  

## **Dataset Description**  
The dataset contains information on individuals, including their responses to the Autism Spectrum Quotient (AQ-10) screening tool and other relevant features.  
To download dataset:
>>kaggle competitions download -c autismdiagnosis
### **Key Features**  
- **A1_Score - A10_Score**: Scores from the AQ-10 screening test  
- **Age**: Age of the patient  
- **Gender**: Male/Female  
- **Ethnicity**: Ethnic background of the patient  
- **Jaundice**: History of jaundice at birth (Yes/No)  
- **Autism**: Family history of autism (Yes/No)  
- **Country_of_residence**: Patient’s country of residence  
- **Used_app_before**: Previous screening test history (Yes/No)  
- **Result**: Total score from the AQ-10 test  
- **Relation**: Relation of the person who completed the test  
- **Class/ASD**: Target variable (0 - No Autism, 1 - Autism)  

## **Project Workflow**  
1. **Data Preprocessing**  
   - Handling missing values  
   - Feature selection and engineering  
   - One-hot encoding for categorical variables  

2. **Exploratory Data Analysis (EDA)**  
   - Data visualization using **seaborn** and **matplotlib**  
   - Correlation heatmaps and distribution plots  

3. **Model Training**  
   - **Logistic Regression**  
   - **Support Vector Machine (SVM)**  
   - **Random Forest Classifier**  

4. **Model Evaluation**  
   - Accuracy, F1-score, and confusion matrix analysis  
   - Comparing multiple models to determine the best performer  

## **Results & Performance**  
| Model | Accuracy |  
|--------|---------|  
| Logistic Regression | 84% |  
| SVM (Polynomial) | 85.5% |  
| SVM (RBF) | 85% |  
| SVM (Sigmoid) | 54.5% |  
| **Random Forest Classifier** | **88%** |  

Random Forest achieved the highest accuracy, making it the best model for ASD prediction in this project.  

## **Conclusion**  
The project demonstrates that machine learning can be effectively used to predict ASD with high accuracy. The **Random Forest Classifier** performed best, achieving an accuracy of **88%**.  

## **Future Directions**  
- **Ensemble Learning**: Combine multiple models to enhance prediction robustness.  
- **Feature Engineering**: Explore domain-specific features and external datasets (e.g., genetic or neuroimaging data).  
- **Hyperparameter Tuning**: Optimize the Random Forest model using Grid Search or Bayesian Optimization.  

## **How to Run the Code**  
1. Clone this repository  
   ```
   git clone <repository-link>
   cd autism-prediction
   ```
2. Install dependencies  
   ```
   pip install pandas numpy seaborn matplotlib scikit-learn imbalanced-learn
   ```
3. Run the Jupyter Notebook or Python script  
   ```
   python autism_prediction.py
   ```

---

Let me know if you need any modifications! 🚀
