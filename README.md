# USA Accidents Analysis

A comprehensive exploratory data analysis (EDA) project analyzing traffic accidents data across the United States. This project investigates patterns, trends, and factors contributing to road accidents using a dataset containing over 7.7 million accident records.

## 📊 Dataset

**Source:** Kaggle  
**File:** `US_Accidents_March23.csv`  
**Records:** 7,728,394 accident entries  
**Columns:** 46 features including location, time, weather conditions, and road infrastructure data

### Dataset Features

The dataset includes information about:
- **Location Data:** City, State, County, Zipcode, Latitude/Longitude coordinates
- **Temporal Data:** Start time, End time, Timezone, Sunrise/Sunset times
- **Weather Conditions:** Temperature, Humidity, Pressure, Visibility, Wind conditions, Precipitation
- **Road Infrastructure:** Traffic signals, junctions, crossings, roundabouts, and other road features
- **Accident Severity:** Severity ratings for each incident
- **Note:** The dataset does not contain data for New York state

### Why This Dataset is Useful

- **Accident Prevention:** Identify high-risk areas and times to implement preventive measures
- **Traffic Management:** Understand patterns to optimize traffic flow and safety protocols
- **Weather Impact Analysis:** Correlate weather conditions with accident frequency
- **Infrastructure Planning:** Identify locations that may need safety improvements
- **Public Awareness:** Generate insights to raise awareness about accident-prone times and locations

## 🔍 Analysis Overview

This project performs comprehensive analysis across multiple dimensions:

### 1. Data Cleaning & Preparation
- Examined data structure and data types
- Identified and handled missing values
- Dropped columns with excessive missing data (End_Lat, End_Lng, Temperature, Wind_Chill, Precipitation, Wind_Speed)

### 2. City-Level Analysis
- Distribution of accidents across cities
- Identification of cities with highest and lowest accident counts
- Statistical analysis of accident frequency patterns

### 3. Temporal Analysis
- Day of week patterns
- Hourly distribution (with special focus on weekends)
- Monthly trends and seasonal variations
- Year-over-year trends

### 4. Geographic Analysis
- State-level accident distribution
- Geographic heatmaps using latitude/longitude coordinates
- Identification of high-risk regions

### 5. Weather & Environmental Factors
- Weather condition analysis
- Correlation between weather and accident frequency

## 📈 Key Insights

1. **Missing Data:** New York state data is absent from the dataset

2. **City Distribution:**
   - Less than 9% of cities have 2000+ yearly accidents
   - Over 1000 cities reported only one accident
   - Accident frequency decreases exponentially across cities

3. **Time Patterns:**
   - **Peak Hours:** Highest accident rates occur during:
     - Morning rush hour (6 AM - 9 AM)
     - Evening rush hour (3 PM - 6 PM)
   - **Weekends:** More accidents between 10 AM - 2 PM

4. **Seasonal Trends:**
   - Highest accident rates in:
     - January
     - November
     - December
   - Contributing factors include:
     - Weather conditions (snow, ice)
     - Holiday seasons (Christmas, Thanksgiving)
     - Increased alcohol consumption during celebrations

## 🛠️ Technologies Used

- **Python 3**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Folium** - Interactive map visualizations
- **Jupyter Notebook** - Interactive development environment

## 📋 Questions Explored

1. Are there more accidents in warmer or cooler areas?
2. Which state has the highest number of accidents (per capita)?
3. In which weather conditions do more accidents occur?
4. How many accidents occur in each city?
5. Why is New York not present in the data, and if present, why does it have fewer accidents despite being a populous city?
6. In the top 100 cities by accident count, which states do they most frequently belong to?
7. At which times do more accidents occur?
8. Which month has the most accidents?
9. What is the trend of accidents year by year (increasing/decreasing)?

## 📁 Project Structure

```
us accidents/
│
├── app.ipynb                    # Main Jupyter notebook with analysis
├── US_Accidents_March23.csv     # Dataset file
└── README.md                    # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.x installed along with the following packages:

```bash
pip install pandas numpy matplotlib seaborn folium jupyter
```

### Running the Analysis

1. Clone or download this repository
2. Ensure the dataset file `US_Accidents_March23.csv` is in the project directory
3. Open `app.ipynb` in Jupyter Notebook:
   ```bash
   jupyter notebook app.ipynb
   ```
4. Run the cells sequentially to execute the analysis

### Note on Dataset

The dataset file (`US_Accidents_March23.csv`) is large (~2GB+) and needs to be downloaded separately from Kaggle. Due to its size, it is not included in this repository.

## 📝 Dataset Details

- **Total Columns:** 46 (after cleaning: 40)
- **Numerical Columns:** 7
- **Categorical Columns:** Multiple (City, State, Weather_Condition, etc.)
- **Memory Usage:** ~2.0+ GB

## 🔬 Analysis Methods

- **Descriptive Statistics:** Summary statistics and distributions
- **Data Visualization:** Histograms, bar charts, heatmaps, and geographic visualizations
- **Temporal Analysis:** Time series analysis of accident patterns
- **Geographic Analysis:** Spatial distribution using coordinates
- **Missing Data Analysis:** Percentage and impact assessment of missing values

## 📊 Visualizations

The notebook includes various visualizations:
- Missing values percentage bar chart
- City accident distribution histograms
- Day of week and hourly distributions
- Geographic heatmaps showing accident hotspots
- Seasonal and monthly trend analyses

## 🤝 Contributing

This is an exploratory analysis project. Suggestions and improvements are welcome!

## 📄 License

This project uses publicly available data from Kaggle. Please refer to the original dataset's license for usage terms.

## 🙏 Acknowledgments

- Kaggle for providing the dataset
- Contributors to the open-source data science libraries used in this project

---

**Note:** This analysis is for educational and exploratory purposes. The insights should not be considered as official statistics without further validation and verification.

