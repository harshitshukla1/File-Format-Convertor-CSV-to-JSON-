# Retail Data File Converter (CSV/Text to JSON)

## Project Description
This project is a modular data processing pipeline built using Python that converts raw CSV/text files into structured JSON format. The input files do not contain column headers, so the project uses a schema definition file to dynamically assign column names.

This project demonstrates a real-world data engineering workflow, including file handling, data transformation, and automation.

---

## Objective
The main objective of this project is to:
- Process raw datasets without column headers
- Apply schema-based column naming
- Convert data into JSON format
- Automate the entire workflow for multiple datasets

---

## Key Features
- Automated file discovery using glob
- Dynamic dataset identification from file paths
- Schema-driven column name extraction
- Data transformation using Pandas
- JSON conversion with proper structure
- Modular and reusable code design

---

## Technologies Used
- Python
- Pandas
- JSON
- Regular Expressions (re)
- OS module
- Glob module
## Project Structure

├── retail_db/ # Raw input data files
│ ├── categories/
│ ├── customers/
│ ├── orders/
│ └── ...
│
├── schemas.json # Schema file with column definitions
├── main.py # Entry point of the project
├── utils.py # Helper functions (modular code)
├── README.md # Project documentation
└── .gitignore # Files/folders to ignore


---

## How It Works
1. Load schema from `schemas.json`
2. Read all input files using glob
3. Extract dataset name from file path
4. Fetch column names based on dataset
5. Load data into Pandas DataFrame
6. Assign column names dynamically
7. Convert DataFrame into JSON format
8. Save output files in structured directories

---

## Example Workflow
- Input: `retail_db/orders/part-orders.txt`
- Schema: defines column names for `orders`
- Output: JSON file with structured records

---

## How to Run the Project
```bash
python modularizecode.ipynb
Use Cases

Data preprocessing pipelines

ETL (Extract, Transform, Load) workflows

Data cleaning and transformation

Preparing datasets for analytics and machine learning

Future Improvements

Add command-line argument support

Implement logging instead of print statements

Add exception handling

Support additional file formats (Excel, Parquet, etc.)

Author

Harshit Shukla

License

This project is open-source and available for learning purposes.

---
