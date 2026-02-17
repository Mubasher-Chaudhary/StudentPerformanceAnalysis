# Student Performance Analysis

## Project Overview
This project analyzes student exam scores to identify top performers, discover trends across demographics, and categorize student performance into result categories (Distinction, Pass, Fail). The analysis uses **Pandas** for data manipulation, **NumPy** for calculations, and **Matplotlib/Seaborn** for visualizations.

---

## Dataset Description
**File:** `Data/StudentsPerformance.csv`

Attributes:
- **Gender:** Student gender (male/female)
- **Parental Level of Education:** Parents’ education background
- **Test Preparation Course:** Completed or None
- **Math Score:** Score (0-100)
- **Reading Score:** Score (0-100)
- **Writing Score:** Score (0-100)

**Key Metrics Created:**
- **Total Score:** Sum of Math, Reading, Writing (0-300)
- **Result:** Categorized as:
  - **Distinction:** Total Score ≥ 270
  - **Pass:** 210–269
  - **Fail:** < 210

---

## Workflow & Steps

1. **Data Import & Exploration**
   - Load CSV dataset using Pandas
   - Display dataset structure and samples

2. **Data Cleaning**
   - Check for missing values
   - Verify data types
   - Remove duplicates

3. **Feature Engineering**
   - Create `Total Score` column
   - Create `Result` column based on score thresholds

4. **Filtering & Selection**
   - Extract top-performing students (Distinction)
   - Filter students by demographics or performance

5. **Grouping & Aggregation**
   - Average scores by gender
   - Count students per result category
   - Analyze effect of test preparation
   - Group performance by parental education

6. **Sorting & Ranking**
   - Sort students by `Total Score` descending
   - Identify top-performing students

7. **Visualization**
   - Bar charts, pie charts, histograms, scatter plots
   - Compare performance across demographics

---

## Key Insights & Findings

### Major Insights

**Parental Education Impact**
- Students with parents holding master's degrees show highest performance
- "Some college" group shows lowest average scores

**Test Preparation Effectiveness**
- Students completing prep courses have higher Distinction rates
- Lower failure rates for course completers

**Gender Performance**
- Female students scored higher on average than male students

**Performance Distribution**
- Score distribution is right-skewed with most near the mean
- High-performing outliers identified

**Result Categories**
- Clear separation of Distinction, Pass, and Fail
- Bachelor’s degree families have the most Distinction/Pass students

---

## Visualizations

### 1️⃣ Result Categories Distribution
![Result Categories Pie Chart](Visuals/result_categories_pie_chart.png)
- Percentage breakdown of Distinction, Pass, and Fail students

### 2️⃣ Total Score Distribution
![Total Score Distribution](Visuals/total_score_distribution.png)
- Histogram with density curve
- Shows score clustering and high-performing outliers

### 3️⃣ Math vs Reading Score Scatter Plot
![Math Reading Scatter Plot](Visuals/math_reading_scatter.png)
- Scatter plot of Math vs Reading scores
- Color-coded by Writing score to show correlation

---

## Libraries Used

| Library | Version | Purpose |
|---------|---------|---------|
| Pandas | ≥1.5.0 | Data cleaning, manipulation |
| NumPy | ≥1.23.0 | Numerical computations |
| Matplotlib | ≥3.7.0 | Static visualizations |
| Seaborn | ≥0.12.0 | Statistical visualizations |
| Jupyter | ≥1.0.0 | Notebook environment |
| IPython | ≥8.0.0 | Interactive Python shell |

---

## How to Run

1. **Install dependencies:**
```bash
pip install -r requirements.txt
