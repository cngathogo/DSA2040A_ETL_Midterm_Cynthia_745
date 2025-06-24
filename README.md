# ETL Lab – Midterm Project

## 🎯 Project Overview
This ETL (Extract, Transform, Load) lab takes raw CSV datasets (`raw_data.csv` and `incremental_data.csv`), applies data cleaning, enrichment, structural and categorization transformations, then loads the processed results into a structured format for further analysis.

---

## 🛠️ ETL Phases

### 1. **Extract**
- Load raw CSV files into Pandas DataFrames.
- Preview using `.head()` and `.info()`.
- Store raw copies (for audit) in `data/`.

### 2. **Transform**
- Remove duplicate rows.
- Handle missing values (e.g., filling or dropping).
- Convert date strings into `datetime`.
- Enrich with `total_price = quantity * unit_price`.
- Outcome saved to `transformed/transformed_full.csv` and `transformed/transformed_incremental.csv`.

### 3. **Load**
- Load transformed data into either:
  - A SQLite database (`loaded/transformed_data.db`)
- Preview results via `SELECT` or `df.head()` to ensure integrity.

---

## 🧰 Tools Used
- **Python 3.12.4**  
- **Pandas** – data manipulation  
- **SQLite (`sqlite3`)** – database loading  

---

## 🚀 How to Run the Project

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your-username/ETL_Midterm_Cynthia_745.git
   cd ETL_Midterm_Cynthia_745
