Pandas CSV Reader & Basic Analysis — Airbnb Dataset

This project demonstrates a complete Pandas-based exploratory analysis workflow using the Airbnb Listings dataset downloaded from Kaggle.
It follows the exact tasks assigned:

✔ Read CSV/Excel into a DataFrame
✔ Inspect dataset (head, tail, types)
✔ Compute summary statistics (mean, median, min, max, count)
✔ Filter rows, select columns, slice subsets
✔ Save filtered results into CSV/Excel

🔍 Project Overview

This project uses Pandas to perform structured data analysis on a large Airbnb listings dataset (~279,000 rows).
It showcases common operations used in real data-analytics workflows, including:

Data loading and memory-safe reading

Basic dataset exploration

Numeric summary statistics

Filtering by conditions

Selecting and slicing subsets

Exporting processed data

(Optional) simple visualizations to support insights

The project is designed in a clean, organized, and industry-standard format that is suitable for academic, internship, or professional submissions.

📁 Repository Structure
airbnb-eda-project/
│
├── data/
│   └── airbnb_listings.csv       
│
├── outputs/
│   ├── high_rated.csv
│   ├── budget_private_rooms.csv
│   ├── family_homes.csv
│   └── ... (additional filtered results)
│
├── src/
│   └── airbnb_eda_notebook.ipynb  # Main Jupyter Notebook (analysis pipeline)


⚠️ Dataset is not included due to Kaggle licensing.
Download it manually and place in: data/airbnb_listings.csv.

🚀 Features Implemented (Task Requirements)
✅ 1. Read CSV into DataFrame

Used pd.read_csv() with low_memory=False

Handled file path management using pathlib.Path

Verified file existence before loading

✅ 2. Inspect Basic Dataset Structure

head() and tail() for first/last rows

dtypes to inspect column types

Null value summary

✅ 3. Compute Summary Statistics

Statistics computed for key numeric columns:

Mean

Median

Minimum

Maximum

Count

Using:

df.describe()
df[col].mean(), df[col].median(), df[col].min(), df[col].max(), df[col].count()

✅ 4. Filter, Select, and Slice Subsets

Examples implemented:

High-rated listings (review_scores_rating >= 4.8)

Budget private rooms (room_type == "Private room" and price <= 80)

Family homes (property_type == "House" and bedrooms >= 2)

Column selection:

df[['price', 'bedrooms', 'room_type']]


Row slicing:

df.iloc[:20]
df[df['price'] < 100]

✅ 5. Save Results to CSV/Excel

Filtered outputs saved using:

df.to_csv("outputs/high_rated.csv", index=False)
df.to_excel("outputs/budget_rooms.xlsx", index=False)

🧪 How to Run the Project
▶️ 1. Install Dependencies
pip install -r requirements.txt

▶️ 2. Place Dataset
data/airbnb_listings.csv

▶️ 3. Run the Jupyter Notebook
jupyter notebook notebooks/airbnb_eda_notebook.ipynb

▶️ 4. Or Run the Python Script
python src/airbnb_eda.py

📊 Outputs Generated

The project produces filtered datasets inside outputs/, including:

high_rated.csv

budget_private_rooms.csv

family_homes.csv

Each file contains only the cleaned, filtered subset based on analysis criteria.

📝 Technologies Used

Python

Pandas

NumPy

Matplotlib (optional plots)

Jupyter Notebook

📌 About the Dataset

The dataset includes detailed Airbnb listing information such as:

Host details

Property type & room type

Bedrooms & accommodates

Latitude/Longitude

Review scores

Pricing

Amenities

This provides a rich foundation for practicing real-world data analysis.

📬 Contact

For questions or improvements:

Aftab Tamboli
📧 aftabtamboli3234@gmail.com
