# 🌾 Agri Data Atlas — India District-Level Crop Dashboard

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Folium](https://img.shields.io/badge/Folium-77B829?style=for-the-badge&logo=leaflet&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-1D9E75?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-ICRISAT%20Open%20Data-orange?style=for-the-badge)

<br/>

**An interactive geo-analytics dashboard mapping crop yield, production,
and farming efficiency across 311 districts and 20 states of India —
built on real government data by an Agricultural Engineer turned Data Analyst.**

<br/>

[🗺️ View Live Map](#live-demo) · [📊 Key Findings](#key-findings) · [🚀 How to Run](#how-to-run) · [🔬 Methodology](#methodology)

</div>

---

## 🌟 Why This Project Is Unique

Most data analysts build Netflix recommendations or sales dashboards.

This project is different — it was built by someone who spent 4 years studying Agricultural Engineering and completed internships inside oil refineries, dairy plants, and farm machinery institutes. The domain expertise behind every analysis here is **authentic, not Googled**.

> *"Better agricultural data can feed millions. This project is my attempt to make that data visible."*
> — Tanya Singh Rajput

---

## 📌 Project Overview

The **Agri Data Atlas** is an interactive, map-based analytical dashboard that visualises crop yield, production area, and farming efficiency across Indian districts using 50+ years of government agricultural data from ICRISAT.

The dashboard features:
- 🗺️ **Choropleth map** of India — every district coloured by crop yield
- 📊 **Interactive charts** — state rankings, crop comparisons, trend analysis
- 🔍 **District comparison tool** — compare any two districts head-to-head
- 📈 **Efficiency scatter plot** — identify high-area, low-yield intervention zones

---

## 📋 Project at a Glance

| Detail | Value |
|--------|-------|
| **Data Source** | ICRISAT District Level Database (Official Government Data) |
| **Districts Covered** | 311 districts across 20 Indian states |
| **Time Period** | 1966–2017 (analysis focused on 2013–2017) |
| **Crops Analysed** | 19 crops — Rice, Wheat, Maize, Sugarcane, Cotton, Pulses, Oilseeds and more |
| **Total Records** | 16,146 rows × 80 columns |
| **Tools Used** | Python · Pandas · NumPy · Plotly · Folium · Jupyter |
| **Output Format** | Interactive HTML files — open in any browser |

---

## 🔍 Key Findings

### 1. India's Yield Gap Is Alarming
> The yield difference between India's most and least productive districts spans **multiple times** — districts in Punjab and Haryana produce dramatically more per hectare than rain-dependent districts in Jharkhand and Odisha. This gap reflects decades of unequal infrastructure investment.

### 2. Irrigation Access Defines Productivity
> Districts with canal or groundwater irrigation consistently outperform rain-fed districts. The data confirms that **water access, not soil quality alone**, is the single biggest determinant of yield.

### 3. Rice Dominates Eastern India, Wheat Dominates the North
> State-level crop specialisation is sharp and clear:
| Region | Dominant Crop |
|--------|--------------|
| Punjab, Haryana, UP | Wheat |
| West Bengal, Assam, Odisha | Rice |
| Maharashtra, Gujarat | Cotton |
| UP, Maharashtra | Sugarcane |
| Rajasthan, Gujarat | Pearl Millet |

### 4. High-Area, Low-Yield Districts Are the Priority Zones
> Several districts farm large areas but produce poor yields — these are the highest-priority zones for government intervention, better seed technology, and irrigation investment.

### 5. National Yield Has Improved — But Unevenly
> While the national average yield improved from 2013 to 2017, the improvement is concentrated in already-productive states. Lagging districts are falling further behind, not catching up.

---

## 🛠️ Tools & Technologies

| Tool | Version | Purpose |
|------|---------|---------|
| **Python** | 3.8+ | Core programming language |
| **Pandas** | Latest | Data loading, cleaning, transformation |
| **NumPy** | Latest | Numerical calculations |
| **Plotly Express** | Latest | Interactive bar, line, scatter charts |
| **Plotly Graph Objects** | Latest | Custom subplots for comparison tool |
| **Folium** | Latest | Choropleth map with GeoJSON |
| **Jupyter Notebook** | Latest | Development environment |
| **openpyxl** | Latest | Excel file reading |

---

## 📁 Project Structure

```
## 📁 Project Structure

```text
agri_data_atlas/
│
├── 📂 dashboards/
│   ├── chart_rice_yield_by_state.html
│   ├── chart_scatter_efficiency.html
│   ├── chart_yield_trend.html
│   └── compare_Durg_vs_Ludhiana.html
│
├── 📂 screenshots/
│   ├── Average_rice_yield.png
│   ├── District_efficiency.png
│   ├── agri_data_atlas.png
│   └── district_comparison.png
│
├── 📓 agri_atlas.ipynb
│
└── 📄 README.md
```

---

## 💡 Python & Analytics Concepts Demonstrated

```
✅ Data Loading      → pd.read_csv() with real government open data
✅ Data Cleaning     → Replace -1 sentinel values, str.strip(), str.title()
✅ Wide → Analysis   → Working with wide-format data (19 crops as columns)
✅ GroupBy + Agg     → Multi-metric district and state summaries
✅ Filtering         → Boolean indexing, year range filtering
✅ Geo-Analytics     → Folium choropleth maps with GeoJSON district boundaries
✅ Interactive Maps  → Hover tooltips, clickable popups, layer controls
✅ Plotly Charts     → Bar, line, scatter with dark theme styling
✅ Subplots          → make_subplots() for multi-panel comparison tool
✅ Custom Functions  → compare_districts() — reusable comparison generator
✅ HTML Export       → write_html() — shareable outputs, no Python needed
```

---

## 🚀 How to Run

### Prerequisites
Install Python 3.8 or above from [python.org](https://www.python.org/downloads/).
During installation, tick **"Add Python to PATH"** before clicking Install Now.

### Step 1 — Clone or Download This Repository

**Option A — Download ZIP (easiest for beginners):**
1. Click the green **"Code"** button at the top of this page
2. Click **"Download ZIP"**
3. Extract the ZIP to your Desktop
4. You will see a folder called `agri-data-atlas-india`

**Option B — Clone with Git:**
```bash
git clone https://github.com/TanyaOnTheWeb/agri_data_atlas.git
cd agri_data_atlas
```

---

### Step 2 — Install Required Libraries

Open **Command Prompt** (Windows: press `Win + R` → type `cmd` → Enter).

Navigate to your project folder:
```bash
cd Desktop\agri-data-atlas-india
```

Install all libraries with one command:
```bash
pip install pandas numpy plotly folium openpyxl jupyter notebook
```

Wait for installation to complete (2–5 minutes depending on internet speed).

**Verify installation:**
```bash
pip list
```
You should see pandas, numpy, plotly, folium listed.

---

### Step 3 — Download the Dataset

The ICRISAT dataset is not included in this repository due to file size.
Download it from one of the following sources:

**Primary source:**
1. Go to [ICRISAT Data Portal](http://data.icrisat.org/dld/src/crops.html)
2. Download the District Level Database
3. Save as `ICRISAT_crops.csv` in the project folder

**Alternative (Kaggle):**
1. Go to [Kaggle — India Agriculture](https://www.kaggle.com/datasets/abhinand05/crop-production-in-india)
2. Download the dataset
3. Save as `ICRISAT_crops.csv` in the project folder

**GeoJSON map file** (also required):
1. Download from [India Districts GeoJSON](https://github.com/geohacker/india)
2. Save as `india_district.geojson` in the project folder

---

### Step 4 — Open Jupyter Notebook

In Command Prompt (inside project folder):
```bash
jupyter notebook
```

Browser opens automatically.
Click `agri_atlas.ipynb` to open the notebook.

---

### Step 5 — Run the Notebook

Run each cell from top to bottom by pressing **Shift + Enter**.

The notebook is divided into sections:
```
Cell 1  → Import libraries
Cell 2  → Load dataset
Cell 3  → Clean column names
Cell 4  → Handle missing values (-1 sentinel)
Cell 5  → Build district summary
Cell 6-9  → Analysis (10 business questions)
Cell 10-11 → Build choropleth map
Cell 12-14 → Build Plotly charts
Cell 15 → District comparison tool
Cell 16 → Save all outputs
```

---

### Step 6 — View Outputs

After running all cells, open these files in your browser:

| File | What You See |
|------|-------------|
| `india_crop_map.html` | Interactive map of India — click any district |
| `chart_rice_yield_by_state.html` | State-level rice yield comparison |
| `chart_yield_trend.html` | National yield trend 2013–2017 |
| `chart_scatter_efficiency.html` | District efficiency scatter plot |
| `compare_Durg_vs_Ludhiana.html` | District head-to-head comparison |

**To open:** Find the file in File Explorer → double-click → opens in browser.
No Python or internet connection needed to view the HTML outputs.

---

## 🗺️ Dashboard Preview

> Interactive choropleth map of India — districts coloured by average crop yield.
> Green = high yield | Yellow = medium | Grey = no data available

<img width="1896" height="901" alt="image" src="https://github.com/user-attachments/assets/2d295843-a7c4-458c-9685-cc5169a22c57" />


---

## 📊 Methodology

### Data Source
ICRISAT (International Crops Research Institute for the Semi-Arid Tropics) maintains the most comprehensive district-level agricultural database for India, covering 50+ years of official government crop statistics.

### Data Structure
The dataset is in **wide format** — each crop has its own Area, Production, and Yield columns. This means 19 crops × 3 metrics = 57 crop-specific columns per row, plus identifier columns (District, State, Year).

### Missing Data Handling
ICRISAT uses **-1** as a sentinel value for missing or unreported data (not blank/null). All -1 values were replaced with `NaN` before analysis to prevent them from skewing calculations.

### Analysis Period
While the dataset spans 1966–2017, analysis was focused on **2013–2017** (the most recent 5 years) to reflect current agricultural conditions rather than historical ones.

### District Matching
Of 311 districts in the dataset, **226 matched** the GeoJSON boundary file by name. The remaining 85 districts had minor spelling differences between the two sources. The map displays all 226 matched districts.

---

## 🌱 About the Author

**Tanya Singh Rajput**
Data Analyst at Cognizant | B.Tech Agricultural Engineering, IGAU

I am a data analyst with a background that sits at the exact intersection of agriculture and technology. After completing my engineering degree and 5+ internships across oil refineries, dairy plants, and farm machinery institutes, I transitioned into data analysis — bringing domain expertise that most analysts simply do not have.

This project is my way of contributing to agricultural data visibility in India. Better data leads to better policy, better investment, and better yields.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Tanya%20Singh%20Rajput-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/tanya1511)
[![GitHub](https://img.shields.io/badge/GitHub-TanyaOnTheWeb-181717?style=flat&logo=github&logoColor=white)](https://github.com/TanyaOnTheWeb)

---

## 📜 Data License

ICRISAT District Level Database is published as open data for research and educational purposes.
Source: [http://data.icrisat.org](http://data.icrisat.org)

---

## ⭐ If this project helped you

Give it a star ⭐ — it helps other analysts and agritech enthusiasts find this work.

---

<div align="center">
<i>Built with 🌾 domain expertise and 🐍 Python</i>
</div>
