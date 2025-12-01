# Industrial Human Resource Geo-Visualization

This project analyzes and visualizes the industrial classification of the workforce in India. It includes data exploration, NLP analysis, and a Streamlit dashboard.

## Project Structure

- `notebooks/`: Contains Jupyter Notebooks for data exploration, NLP, and the original Streamlit code.
  - `part_1_Industrial_Human_Resource.ipynb`: Data exploration and cleaning.
  - `part_2_Industrial_HR_NLP.ipynb`: NLP analysis.
  - `part_3_Industrial_HR_Streamlit_part.ipynb`: Original Streamlit notebook.
- `src/`: Contains the source code for the Streamlit application.
  - `app.py`: The main Streamlit application script.
- `data/`: Directory for dataset files (CSVs). **Please place your CSV files here.**
- `requirements.txt`: List of Python dependencies.

## Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd ML_Industrial_HR_Geo_Visualisation
    ```

2.  **Install dependencies:**
    It is recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```

3.  **Data Setup:**
    Ensure your CSV data files (e.g., `HR_1.csv`, etc.) are placed in the `data/` directory. The application reads from this folder.

## Running the Application

To run the Streamlit dashboard:

```bash
streamlit run src/app.py
```

## Features

- **Home:** Overview of the project and dataset.
- **Overview:** Data statistics, clustering analysis, and visualizations.
- **Explore:** Interactive exploration of workforce data, including maps and charts.
