# Industrial Human Resource Geo-Visualization Dashboard

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Framework-Streamlit-red?logo=streamlit)
![NLP](https://img.shields.io/badge/AI-NLP%20%26%20Clustering-yellow?logo=scikit-learn)
![Plotly](https://img.shields.io/badge/Visualization-Plotly-green?logo=plotly)
![Status](https://img.shields.io/badge/Status-Research%20Prototype-success)

---

## 📊 Business Use Case

Understanding the distribution of India's workforce across diverse industries is critical for **economic planning and policy formulation**. This dashboard addresses the challenge of analyzing complex, unstructured industrial data by combining **Geo-Spatial Visualization** with **Natural Language Processing (NLP)**. It enables policymakers and researchers to:

- **Map Workforce Distribution**: Visualize the density of Main vs. Marginal workers across rural and urban landscapes.
- **Categorize Industries**: Automatically cluster thousands of unorganized industry descriptions (NIC codes) into meaningful sectors using AI.
- **Identify Regional Specializations**: Pinpoint which states dominate specific industrial sectors.
- **Drive Employment Strategy**: Make data-driven decisions to boost employment in under-represented regions or sectors.

---

## 🏗️ Architecture

The system leverages a hybrid **Data Analytics & ML Pipeline** to transform raw census data into actionable insights:

```
┌─────────────────────────────────────────────────────────────┐
│                    RAW CENSUS DATA                           │
│             (State-wise Industrial CSV Files)               │
└──────────────────────┬──────────────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  🧹 DATA PREPROCESSING ENGINE                               │
│  • Merging: Automated aggregation of multi-state CSVs       │
│  • Cleaning: State/District name normalization              │
│  • Filtering: Separation of Main vs. Marginal workers       │
└──────────────────────┬──────────────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  🧠 AI & NLP CORE                                           │
│  • Text Vectorization: TF-IDF on Industry Names (NIC)       │
│  • Clustering: K-Means to group similar industries          │
│  • Keyword Extraction: NLTK-based tokenization              │
└──────────────────────┬──────────────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  📈 INTERACTIVE DASHBOARD (Streamlit)                       │
│  • Geo-Maps: Plotly Choropleth for state-wise density       │
│  • Cluster Analysis: Word Clouds & Treemaps                 │
│  • Comparative Plots: Urban vs. Rural scatter plots         │
└─────────────────────────────────────────────────────────────┘
```

---

## ✨ Features

### 🗺️ **Geo-Spatial Intelligence**
- **Interactive India Map**: Choropleth maps visualizing worker population density across all states and union territories.
- **Demographic Filters**: Drill down by Worker Type (Main/Marginal), Gender (Male/Female), and Area (Rural/Urban).

### 🧠 **NLP-Powered Industry Analysis**
- **Automated Clustering**: Uses K-Means to group thousands of diverse industry descriptions into 5 distinct clusters for easier analysis.
- **Word Clouds**: Visualizes the most dominant terms within each industry cluster (e.g., "Manufacturing", "Retail", "Construction").
- **Treemaps**: Hierarchical view of the top 10 industries contributing to the workforce.

### 📊 **Advanced Data Visualization**
- **Urban vs. Rural Correlation**: Scatter plots to analyze the relationship between urbanization and workforce participation.
- **State-wise Distribution**: Dynamic bar charts showing the ranking of states based on employment figures.
- **Cluster Distribution**: Pie charts showing the proportion of industries falling into each AI-generated category.

---

## 💻 Tech Stack

| Category | Technologies |
|----------|-------------|
| **Language** | Python 3.8+ |
| **Web Framework** | Streamlit, Streamlit Option Menu |
| **Machine Learning** | scikit-learn (KMeans, TF-IDF) |
| **NLP** | NLTK (Tokenization, Stopwords) |
| **Visualization** | Plotly Express, Matplotlib, Seaborn, WordCloud |
| **Data Processing** | Pandas, NumPy |

---

## 📦 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup Steps

1. **Clone the repository**:
   ```bash
   git clone git@github.com:rajaganaa/Industrial-HR-Geo-Dashboard.git
   cd Industrial-HR-Geo-Dashboard
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
   *Note: Installs streamlit, pandas, scikit-learn, nltk, plotly, and other visualization libraries.*

3. **Data Setup**:
   - Ensure your CSV data files (containing columns like `India/States`, `NIC Name`, `Main Workers`, etc.) are placed in the `data/` directory.
   - The app automatically merges all CSVs found in this folder.

4. **NLTK Setup**:
   - The app will automatically download necessary NLTK data (`stopwords`, `punkt`) on the first run.

---

## 🚀 Usage

1. **Launch the Dashboard**:
   ```bash
   streamlit run src/app.py
   ```

2. **Navigate Modules**:
   - **Home**: Project overview and objectives.
   - **Overview**: High-level statistics, AI clustering analysis, and Word Clouds.
   - **Explore**: Deep dive with Geo-Maps, Scatter plots, and State-wise comparisons.

3. **Interact**:
   - Use the sidebar to switch between views.
   - Use dropdowns to filter by Worker Type, Sex, and Area to update visualizations in real-time.

---

## 📝 License

This project is open-source and available for educational and portfolio purposes.

---

## 👤 Author

**Rajaganapathy M**  
GitHub: [@rajaganaa](https://github.com/rajaganaa)  
Email: rajaganaa@gmail.com

---

**Built with ❤️ for Economic Research and Data Science**
