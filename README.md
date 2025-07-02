# Student Score Predictor

## 📌 Overview:
This project is an AI-powered tool that predicts a student’s average exam score and assigns an appropriate letter grade (A–F) using non-academic features like gender, demographic group, parental education level, lunch type, and test preparation status.

## 🎯 What Does This Project Do?
- Trains a machine learning regression model to estimate a student’s average score (0–100)
- Converts that score into a final letter grade (A, B, C, D, or F)
- Builds an interactive web application using Gradio, where users input student characteristics and receive:
- A predicted average score
- A predicted final grade

## 🧩 Problem It Solves:
In real-life education systems:
- Teachers, schools, and policy makers often need to identify students at risk of underperforming
- But they may not always have access to actual exam results until it’s too late
  
This project helps solve that by:
- Predicting performance before tests are taken
- Using non-academic indicators to anticipate outcomes
- Helping schools target resources or offer support to students who may be at risk

## 💡 Why Is It Helpful?
- Early Intervention: Helps identify students who may need academic support before scores come in
- Data-Driven Insights: Shows which features (like test prep or lunch access) most impact performance
- Educational Equity: Could highlight social or demographic factors that correlate with academic challenges
- Simplicity & Accessibility: The model uses simple, easy-to-gather inputs—no exams or complex history required

## 📊 Features Used in Prediction:
- ✅ Gender (male, female)
- ✅ Demographic Group (anonymized groups A–E)
- ✅ Parental Level of Education
- ✅ Lunch Type (standard, free/reduced)
- ✅ Test Preparation Course (completed, none)

These are all non-invasive inputs that schools often already collect.

## ⚙️ How It Works (Under the Hood):
- Uses Random Forest Regressor to train on a real-world student dataset
- Transforms categorical fields into numerical values for ML use
- Outputs an estimated average score and maps it to
  - A: 90–100
  - B: 80–89
  - C: 70–79
  - D: 60–69
  - F: below 60

## 📈 Visualizations Included:
- Distribution of average scores (Histogram)
- Score spread by gender (Box Plot)
- Score spread by lunch type (Violin Plot)
- Feature importance chart (Bar Graph showing which inputs influence predictions the most)

## 🌐 Interactive Gradio App:
- Inputs: Dropdowns for gender, demographic group, etc.
- Outputs: Predicted score and grade

Fully functional inside Google Colab for easy testing and sharing

## 📊 Evaluation Metrics:
- R² Score: Measures how well the model explains score variance
- RMSE: Shows how far off predictions are, on average

These metrics confirm that the model performs far better than guessing and captures real patterns

## 🧠 Conclusion:
This project is a simple yet powerful example of how AI can support education. It doesn’t replace exams, but it helps anticipate outcomes, offer support early, and make schools more data-driven.

It’s also a great entry-level AI project that includes:
- Data processing
- Model training
- Evaluation
- Visualization
