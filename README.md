# ML_Industrial_HR_Geo_Visualisation

# Industrial Human Resource Analysis with Streamlit
# Project Overview

This repository contains Python code for analyzing a dataset on the industrial classification of the workforce in India. The code leverages Streamlit to create an interactive web-based application, providing a user-friendly interface for data exploration and visualization.

# Structure:

Industrial_Human_Resource.ipynb: This Jupyter Notebook focuses on data preprocessing, feature engineering, exploratory data analysis, and model building.
Industrial_HR_NLP.ipynb: This Jupyter Notebook explores the "NIC Name" column using Natural Language Processing (NLP) techniques.
Industrial_HR_Streamlit_part.ipynb: This Jupyter Notebook contains the Streamlit code that creates the web-based application, integrating visualizations and user interactions.
# Requirements:
The code utilizes several Python libraries, including:

pandas
numpy
matplotlib
seaborn
nltk
sklearn
plotly.express
streamlit
# Instructions:

Clone this repository.
Install the required libraries using pip install <library_name>.
Open the Jupyter notebooks (Industrial_Human_Resource.ipynb, Industrial_HR_NLP.ipynb, and Industrial_HR_Streamlit_part.ipynb) in a Jupyter Notebook environment and run the code cells.
To launch the Streamlit application, navigate to the Industrial_HR_Streamlit_part.ipynb notebook and run the code cell containing the st.run() command. This will open a web browser with the interactive dashboard.
# Output:

The Jupyter notebooks will generate various plots and visualizations related to the data exploration and model performance.
The Streamlit application will provide an interactive interface for exploring the data, visualizing insights, and gaining a deeper understanding of the industrial workforce.
# Additional Notes:

The code is well-commented and includes explanations for each step.
You may need to adjust the file paths and data loading configurations based on your specific environment.
The code assumes that the CSV files are located in the same directory as the Jupyter notebooks.
For more advanced analysis, consider exploring techniques like dimensionality reduction, feature selection, and hyperparameter tuning.
# Key Features of the Streamlit App:

Interactive Data Exploration: Explore data through visualizations like histograms, box plots, scatter plots, and word clouds.
Customizable Filters: Apply filters to drill down into specific data segments.
Natural Language Processing Insights: Visualize the results of NLP analysis, including word clouds and topic modeling.
Model Performance Evaluation: Assess the performance of classification models using metrics like accuracy, precision, recall, and F1-score.
