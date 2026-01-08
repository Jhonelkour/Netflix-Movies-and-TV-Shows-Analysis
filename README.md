# 🎬 Netflix Movies and TV Shows Analysis

A comprehensive data analysis project exploring Netflix's content strategy, production trends, and audience targeting using Python data science tools.

## 📊 Project Overview

This project analyzes Netflix's catalog of movies and TV shows to uncover strategic insights about content distribution, production trends, and audience preferences. Using exploratory data analysis (EDA) and statistical techniques, we examine over 8,000 titles available on Netflix as of mid-2021.

## 🎯 Objectives

The analysis addresses four key questions:

1. **Content Distribution**: Understanding what content is available across different countries
2. **Content Similarity**: Identifying similar content by matching text-based features
3. **Network Analysis**: Examining relationships between actors and directors to find collaboration patterns
4. **Strategic Shift**: Analyzing whether Netflix has shifted focus from movies to TV shows in recent years

## 📁 Project Structure

```
Netflix Movies and TV Shows/
│
├── data/
│   └── netflix_titles.csv          # Raw dataset (8,000+ titles)
│
├── notebooks/
│   └── Netflix.ipynb                # Main analysis notebook
│
├── requirements.txt                 # Python dependencies
└── README.md                       # Project documentation
```

## 📦 Dataset

**Source**: Netflix catalog data (as of mid-2021)

**Features**:

- `show_id`: Unique identifier
- `type`: Movie or TV Show
- `title`: Name of the content
- `director`: Director(s)
- `cast`: Main cast members
- `country`: Production country/countries
- `date_added`: Date added to Netflix
- `release_year`: Original release year
- `rating`: Content rating (TV-MA, PG-13, etc.)
- `duration`: Length (minutes for movies, seasons for TV shows)
- `listed_in`: Genre categories
- `description`: Brief synopsis

**Size**: 8,807 rows × 12 columns

## 🛠️ Technologies Used

- **Python 3.9+**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **matplotlib** - Data visualization
- **seaborn** - Statistical visualizations
- **Jupyter Notebook** - Interactive development environment

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.9 or higher installed on your system.

### Installation

1. **Clone or download this repository**
2. **Navigate to the project directory**:

   ```bash
   cd "Netflix Movies and TV Shows"
   ```
3. **Install required packages**:

   ```bash
   pip install -r requirements.txt
   ```
4. **Launch Jupyter Notebook**:

   ```bash
   jupyter notebook
   ```
5. **Open** `notebooks/Netflix.ipynb` and run the cells sequentially

## 📈 Analysis Workflow

### 1. Data Quality Assessment

- ✅ No duplicate records found
- 🔧 Handled missing values (director: 2,634, cast: 825, country: 831)
- 🔧 Fixed data misalignment in 3 records
- 🔧 Inferred missing countries using genre keywords

### 2. Feature Engineering

Created derived features for deeper analysis:

- `num_country`: Number of production countries per title
- `num_cast`: Number of cast members
- `rating_category`: Grouped ratings into Kids/Teens/Adults
- `duration_value`: Numeric duration
- `duration_type`: Unit (minutes/seasons)

### 3. Exploratory Data Analysis

Comprehensive visualizations and statistical analysis covering:

- Content type distribution
- Geographic content production
- Temporal trends (2010-2021)
- Genre analysis
- Rating category distribution
- Cast and production scale
- Duration patterns

### 4. Advanced Analysis

- **Trend Analysis**: Movie vs TV Show ratio over time
- **Network Analysis**: Director-actor collaboration patterns
- **Correlation Analysis**: Feature relationships
- **Gap Analysis**: Underserved audience segments

## 🔍 Key Findings

### Content Distribution

- **70% Movies** vs **30% TV Shows** in the catalog
- **United States leads** with 2,809 titles (37% of content)
- India and South Korea show strong presence as emerging markets

### Strategic Shift ⭐

- **Answer**: YES, Netflix has significantly increased TV show focus
- TV shows grew from **19% (2010)** to **44% (2020)**
- Clear strategic pivot toward serialized content

### Audience Targeting

- **69% Adult content** (TV-MA, R ratings)
- Kids content: only **8%** of catalog
- Teens content: **23%** of catalog
- **Gap Identified**: Family-friendly content is underserved

### Production Trends

- **42% of content** released from 2018 onwards
- Focus on **modern content** over archival material
- **Single-country productions** dominate (90%)
- Most movies: **90-120 minutes** duration
- Most TV shows: **1-2 seasons** (mini-series format)

### Network Insights

- Top directors have **3-5+ collaborations** with specific actors
- Strong **regional partnership networks** exist
- Small group of **prolific creators** dominate the catalog

### Genre Patterns

- **Top genres**: Drama, Documentary, International Movies
- Most titles span **2-3 genre categories**
- Genre preferences vary significantly by country

## 📊 Visualizations Included

The notebook contains 15+ professional visualizations:

- Count plots for content distribution
- Pie charts for geographic analysis
- Line plots for temporal trends
- Stacked area charts for strategy shifts
- Bar charts for genre analysis
- Histograms for duration patterns
- Heatmaps for correlation analysis
- Horizontal bar charts for network analysis

## 🎓 Skills Demonstrated

- Data cleaning and preprocessing
- Missing value imputation strategies
- Feature engineering
- Exploratory data analysis (EDA)
- Statistical analysis
- Data visualization
- Trend analysis
- Network analysis
- Strategic business insights
- Python programming
- Pandas data manipulation
- Matplotlib/Seaborn visualization

## 📄 License

This project is open source and available for educational purposes.

🙏 Acknowledgments

- Netflix for providing the inspiration
- Data science community for best practices and methodologies
- Kaggle for hosting similar datasets

---

**Note**: This analysis is based on mid-2021 data and represents a snapshot of Netflix's strategy at that time. Current Netflix catalog may differ significantly.

For questions or suggestions, please open an issue or contribute to the project!
