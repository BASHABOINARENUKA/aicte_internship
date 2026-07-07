# Intelligent Classification of Rural Infrastructure Projects Under PMGSY Using Machine Learning on IBM Cloud

## Project Overview

The **Pradhan Mantri Gram Sadak Yojana (PMGSY)** is a Government of India rural development initiative focused on improving road and bridge connectivity in rural areas.

PMGSY includes multiple schemes, such as:

* PMGSY-I
* PMGSY-II
* RCPLWEA
* Other related rural infrastructure schemes

Manually classifying thousands of infrastructure projects into the correct scheme is time-consuming, error-prone, and difficult to scale.

This project uses **Machine Learning** and **IBM Cloud services** to automatically classify rural infrastructure projects into the appropriate PMGSY scheme based on project characteristics.

---

## Problem Statement

The PMGSY program contains a large number of rural road and bridge infrastructure projects across different states and districts in India.

Each project must be classified under the correct PMGSY scheme. Manual classification can lead to:

* Increased processing time
* Human errors
* Difficulty in handling large datasets
* Inefficient project monitoring
* Challenges in budget allocation and policy planning

The objective of this project is to build an intelligent machine learning system that automatically predicts the appropriate PMGSY scheme for a rural infrastructure project.

---

## Proposed Solution

The proposed system uses historical PMGSY project data to train a multi-class classification model.

The complete workflow consists of:

1. Data collection
2. Data preprocessing
3. Feature selection
4. Machine learning model training
5. Model evaluation
6. Best model selection
7. Model deployment on IBM Cloud
8. Prediction of PMGSY schemes for new project data

---

## Dataset

The project uses structured rural infrastructure project data obtained through the **AI-KOSH platform**.

The dataset contains project-related information such as:

* State
* District
* Project type
* Road or bridge information
* Total project cost
* Project length
* Number of bridges
* Number of road segments
* PMGSY scheme

The PMGSY scheme is used as the target variable for the machine learning classification task.

---

## System Architecture

```text
PMGSY Dataset
      |
      v
Data Upload to IBM Cloud
      |
      v
Data Preprocessing
      |
      v
Feature Selection and Transformation
      |
      v
AutoAI Model Training
      |
      v
Multiple Pipeline Evaluation
      |
      v
Best Model Selection
      |
      v
IBM Watson Machine Learning Deployment
      |
      v
Prediction of PMGSY Scheme
```

---

## System Development Approach

The project was developed using IBM Cloud services and standard machine learning tools.

### IBM Cloud Services

* IBM Cloud Lite Account
* IBM watsonx.ai Studio
* IBM Cloud Object Storage
* IBM Watson Machine Learning
* IBM AutoAI
* IBM Deployment Space

### Python Libraries

* pandas
* NumPy
* scikit-learn
* matplotlib
* seaborn
* joblib

---

## Data Preprocessing

Before training the machine learning model, the dataset is processed to improve data quality and model performance.

The preprocessing steps include:

* Handling missing values
* Removing inconsistent data
* Encoding categorical variables
* Selecting relevant input features
* Transforming the target variable
* Normalizing numerical features where required

Categorical features such as state, district, and project type can be converted into numerical representations using encoding techniques.

---

## Machine Learning Approach

This project is a **multi-class classification problem**.

The model learns patterns from historical PMGSY infrastructure project data and predicts the correct scheme for new projects.

The machine learning workflow includes:

* Training multiple classification algorithms
* Comparing model performance
* Hyperparameter optimization
* Selecting the best-performing pipeline
* Deploying the selected model

The project uses **IBM AutoAI** to automate major parts of the machine learning lifecycle.

AutoAI performs:

* Data preprocessing
* Feature engineering
* Algorithm selection
* Hyperparameter optimization
* Pipeline generation
* Model comparison

A classification algorithm such as **Random Forest Classifier** can be used because it performs well on structured data and can capture complex relationships between project features.

---

## Model Training

The historical PMGSY dataset is divided into training and testing data.

The model learns the relationship between project characteristics and their corresponding PMGSY schemes.

Example input features include:

```text
State
District
Project Type
Total Cost
Project Length
Number of Bridges
Road Information
```

Target variable:

```text
PMGSY Scheme
```

The model learns from labelled historical data and predicts the scheme for new or unlabelled infrastructure projects.

---

## Model Evaluation

The trained classification pipelines are evaluated using standard machine learning metrics.

The main evaluation metrics include:

* Accuracy
* Precision
* Recall
* F1-Score

The best-performing pipeline is selected based on its evaluation results.

---

## Deployment

After selecting the best-performing machine learning pipeline, the model is deployed using **IBM Watson Machine Learning**.

Deployment steps:

1. Create an IBM Cloud project.
2. Upload the PMGSY dataset.
3. Associate IBM Cloud Object Storage.
4. Create an AutoAI experiment.
5. Select the prediction target.
6. Train multiple machine learning pipelines.
7. Compare pipeline performance.
8. Select the best-performing model.
9. Save the model.
10. Create a deployment space.
11. Deploy the model as an online service.
12. Test the deployed model using new project data.

The deployed model can provide real-time predictions for new rural infrastructure projects.

---

## Prediction Workflow

```text
New Infrastructure Project Data
              |
              v
      Deployed ML Model
              |
              v
     Feature Processing
              |
              v
     Scheme Classification
              |
              v
Predicted PMGSY Scheme
```

---

## Results

The machine learning model was trained to classify rural infrastructure projects into the appropriate PMGSY schemes.

The prediction is based on project characteristics such as:

* Project cost
* Project length
* Number of bridges
* State information
* District information
* Project type

The trained model successfully demonstrates how machine learning can automate PMGSY scheme classification and reduce manual effort.

---

## Key Benefits

* Automates infrastructure project classification
* Reduces manual effort
* Minimizes human errors
* Improves scalability
* Supports faster project monitoring
* Helps with budget allocation
* Supports government planning and decision-making
* Enables real-time prediction through cloud deployment

---

## Future Scope

The current system can be improved by including additional project information.

Future enhancements include:

### Additional Features

The model can use:

* Project start date
* Project completion date
* Weather conditions
* Terrain type
* Forest or hill region information
* Project delays
* Contractor performance
* Construction quality information

### Model Improvements

Future versions can include:

* Advanced ensemble models
* Explainable AI techniques
* Automated model retraining
* Continuous performance monitoring
* Real-time data integration

### Application Development

A web application can be developed where users can:

1. Enter project details.
2. Submit the project information.
3. Send the data to the deployed model.
4. Receive the predicted PMGSY scheme.

### Government Dashboard Integration

The deployed model can be integrated with government monitoring dashboards to classify new infrastructure projects automatically.

---

## Conclusion

This project demonstrates the application of machine learning for automatically classifying rural infrastructure projects under the appropriate PMGSY schemes.

By using structured project data and machine learning classification techniques, the system reduces manual effort and improves the efficiency of scheme identification.

The use of IBM Cloud, AutoAI, and Watson Machine Learning enables the complete machine learning lifecycle, from data preparation and model training to evaluation and cloud deployment.

This project demonstrates how artificial intelligence and cloud technologies can support rural development planning, infrastructure monitoring, and data-driven governance.

---

## References

1. AI-KOSH Dataset – PMGSY Project Data
2. Government of India National AI Portal
3. Scikit-learn Machine Learning Documentation
4. IBM watsonx.ai Studio Documentation
5. IBM Cloud Documentation
6. Breiman, L. (2001). Random Forests. Machine Learning, 45(1), 5–32.
7. Kotsiantis, S. (2007). A Survey on Classification Techniques in Data Mining.

---

