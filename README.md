# 📊 Analysis of US County Health Index Predictors

This project was completed for the **STAT 4770/7770: An Introduction to Python for Data Science** course at the Wharton School, University of Pennsylvania.

## 📝 Project Overview

This project conducts a comprehensive data analysis to identify the key factors that predict a county's overall health performance in the United States. Using a dataset that combines health, economic, and demographic characteristics, the primary goal is to build an interpretive model that explains the variation in a composite "Health Index" across different counties.

The core of the analysis involves the implementation of a **Regression Tree** model to determine which variables are the most significant predictors. The entire data science workflow is documented, from data cleaning and exploratory analysis to model building and interpretation.

## ❓ Key Questions

The analysis seeks to answer the following central question:
* **Which health behaviors, economic conditions, and demographic factors are the most significant predictors of a county's overall Health Index in the United States?**

## 💾 Dataset

* **Source:** The data is provided by the [County Health Rankings & Roadmaps](https://www.countyhealthrankings.org/) program, a collaboration between the Robert Wood Johnson Foundation and the University of Wisconsin Population Health Institute.
* **Unit of Analysis:** Each row in the dataset represents a single US county.
* **Key Variables:** The dataset includes a wide range of variables, such as Health Outcomes, Health Behaviors (e.g., Obesity, Smoking), Economic Factors (e.g., Income, Unemployment), and Demographics.

## 🛠️ Methodology

The project follows a structured data analysis workflow:
1.  **Data Cleaning & Preprocessing:** Loaded the `Data.csv` file, handled missing values, and prepared the data for analysis.
2.  **Exploratory Data Analysis (EDA):** Generated numerical and graphical summaries to understand the distribution of the target variable (Health Index) and its relationship with key predictors.
3.  **Model Building:** Constructed a `DecisionTreeRegressor` model using Scikit-learn to predict the Health Index based on the other variables.
4.  **Model Interpretation:** Visualized and interpreted the resulting regression tree to identify the most influential factors and decision rules.

## 💡 Key Findings

The final regression tree model and subsequent analysis revealed several key insights:

* **Median Household Income is the strongest predictor** of health outcomes. 💰
* **Smoking rates have a significant negative effect** on health. 🚬
* **Unemployment correlates negatively with health**, but its impact is less pronounced than that of income and smoking. 📉
* **Adult Obesity's impact on health was not significant** in the final regression model, possibly due to interactions with other variables.
* Potential **multicollinearity** in the model suggests that some predictors (like income and education) are interdependent. 🔗
* **Geographic disparities in health are evident**, as seen in the state-by-state Health Index scores. 🗺️
* The model effectively captures a substantial portion of the Health Index's variance. ✅

## 📜 Conclusions

Based on the findings, we can draw the following conclusions:

* **Economic status is crucial for health**, with income being a primary driver.
* Public health efforts should **prioritize smoking cessation** programs.
* Addressing **unemployment** may lead to secondary improvements in community health.
* Further research is needed to clarify the complex role of obesity in population health models.
* Significant **regional health disparities** exist across the United States and warrant targeted policy interventions.

## 💻 Technologies Used

* **Language:** Python
* **Libraries:**
    * Pandas (Data Manipulation)
    * NumPy (Numerical Operations)
    * Scikit-learn (Machine Learning - Regression Tree)
    * Matplotlib & Seaborn (Data Visualization)
* **Environment:** Jupyter Notebook

## 📁 File Structure

* `Final Project Code.ipynb`: The main Jupyter Notebook containing all Python code for the analysis.
* `Data.csv`: The raw dataset used for this project.
* `Index.html`: An HTML export of the final presentation slides.
* `Introduction.pdf`: The original project guidelines and description.
* `README.md`: This summary file.

## 🚀 How to Run This Project

To replicate this analysis, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    cd YOUR_REPOSITORY_NAME
    ```

2.  **Install the required libraries.** It is recommended to create a virtual environment first.
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn jupyter
    ```

3.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

4.  Open the `Final Project Code.ipynb` file and run the cells sequentially.
