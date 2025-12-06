
````markdown
# 🏡 Pandas CSV Reader & Basic Analysis — Airbnb Dataset

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)

## 🔍 Project Overview

This project demonstrates a complete **Pandas-based exploratory analysis workflow** using the Airbnb Listings dataset. It showcases common operations used in real-world data analytics workflows, processing a large dataset of approximately **279,000 rows**.

The project is designed in a clean, organized, and industry-standard format suitable for academic, internship, or professional submissions.

### **Key Objectives**
* **Data Loading:** Efficient and memory-safe reading of large CSVs.
* **Exploration:** Inspecting structure, types, and null values.
* **Statistics:** Computing mean, median, min, max, and counts.
* **Manipulation:** Filtering rows, selecting columns, and slicing subsets.
* **Export:** Saving processed insights to new CSV/Excel files.

---

## 📁 Repository Structure

```text
airbnb-eda-project/
│
├── data/
│   └── airbnb_listings.csv       # (Not included - See Setup below)
│
├── outputs/
│   ├── high_rated.csv            # Filtered: Ratings >= 4.8
│   ├── budget_private_rooms.csv  # Filtered: Private rooms <= $80
│   ├── family_homes.csv          # Filtered: Houses with 2+ bedrooms
│   └── ... 
│
├── src/
│   └── airbnb_eda_notebook.ipynb # Main Analysis Pipeline
│
├── requirements.txt              # Project dependencies
└── README.md                     # Project Documentation
````

-----

## 🚀 Features Implemented

This project fulfills the following specific data analysis tasks:

### ✅ 1. Read CSV into DataFrame

  * Used `pd.read_csv()` with `low_memory=False` for efficiency.
  * Implemented robust file path management using `pathlib`.
  * Includes validation to check if the file exists before loading.

### ✅ 2. Inspect Dataset Structure

  * **Head/Tail:** Inspection of first and last rows.
  * **Dtypes:** Verification of column data types.
  * **Null Check:** Summary of missing values across the dataset.

### ✅ 3. Compute Summary Statistics

Calculated key metrics for numeric columns (Price, Review Scores, etc.):

  * Mean, Median, Minimum, Maximum, Count.
  * Utilized `df.describe()` and individual aggregation functions.

### ✅ 4. Filter, Select, and Slice

Complex queries applied to extraction insights:

  * **High-Rated:** `review_scores_rating >= 4.8`
  * **Budget Options:** `room_type == "Private room"` AND `price <= 80`
  * **Family Homes:** `property_type == "House"` AND `bedrooms >= 2`
  * **Slicing:** `df.iloc[:20]` and specific column subsets like `['price', 'bedrooms']`.

### ✅ 5. Save Results

  * Processed subsets are exported to the `outputs/` directory using `df.to_csv()` and `df.to_excel()`.

-----

## 🧪 How to Run the Project

### 1\. Clone the Repository

```bash
git clone [https://github.com/Aftab0023/Pandas-CSV-Reader---Basic-Analysis.git](https://github.com/Aftab0023/Pandas-CSV-Reader---Basic-Analysis.git)
cd Pandas-CSV-Reader---Basic-Analysis
```

### 2\. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3\. Download the Dataset

⚠️ **Note:** The dataset is not included in this repo due to Kaggle licensing.

1.  Download the **Airbnb Listings Dataset** from [Kaggle](https://www.kaggle.com/datasets/ulrikthygepedersen/airbnb-listings).
2.  Rename the file to `airbnb_listings.csv`.
3.  Place it inside the `data/` folder.

### 4\. Run the Analysis

You can run the analysis via Jupyter Notebook or Python script:

**Option A: Jupyter Notebook (Recommended)**

```bash
jupyter notebook src/airbnb_eda_notebook.ipynb
```

**Option B: Python Script**

```bash
python src/airbnb_eda.py
```

-----

## 📊 Outputs Generated

After running the script, the following files are generated in the `outputs/` folder:

| File Name | Description |
| :--- | :--- |
| `high_rated.csv` | Listings with review scores of 4.8 or higher. |
| `budget_private_rooms.csv` | Private rooms priced at $80 or less. |
| `family_homes.csv` | Houses suitable for families (2+ bedrooms). |

-----

## 📝 Technologies Used

  * **Python 3.x**
  * **Pandas** (Data Manipulation)
  * **NumPy** (Numerical Operations)
  * **Matplotlib** (Optional Visualizations)
  * **Jupyter Notebook** (Interactive Environment)

-----

## 📬 Contact

For questions, feedback, or collaboration opportunities:

**Aftab Tamboli** 📧 [aftabtamboli3234@gmail.com](mailto:aftabtamboli3234@gmail.com)  
GitHub: [@Aftab0023](https://www.google.com/search?q=https://github.com/Aftab0023)

```
```
