# PySpark Practice & Interview Prep 🚀

This repository contains my **PySpark practice notebook** where I explored fundamental Spark concepts, practical coding, and interview-style Q&A. It demonstrates how to use PySpark for real-world data handling and analysis while also preparing for data engineering and analyst interviews.

---

## 📂 Notebook Overview

- **Dealing with Corrupted Records**
  - Detecting and handling malformed data in CSV/JSON
  - Read modes: `PERMISSIVE`, `FAILFAST`, `DROPMALFORMED`
  - Printing and storing bad records using `.option("badRecordsPath", ...)`

- **Transformations & Actions**
  - Lazy evaluation and DAG execution
  - Narrow vs. wide transformations
  - Common actions: `show`, `collect`, `count`

- **Hands-On PySpark**
  - Building a local Spark session
  - Reading CSV with schema inference
  - Performing `groupBy`, `joins`, and aggregations

---

## ⚙️ Tech Stack

- Python 3.x  
- Apache Spark (PySpark)  
- Jupyter Notebook  

---

## 🚀 How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/<your-username>/PySpark-Practice.git
   cd PySpark-Practice
Install dependencies (if not already installed):

bash
Copy code
pip install pyspark jupyter
Launch Jupyter Notebook:

bash
Copy code
jupyter notebook
Open PySpark.ipynb and run cells.

📌 Use Cases
This project demonstrates how to:

Clean and process large datasets in PySpark

Handle corrupted records gracefully without breaking jobs

Apply transformations and actions effectively to optimize performance

Explain Spark internals (lazy evaluation, DAG execution) during interviews

Strengthen hands-on familiarity with PySpark for real-world data pipelines

❓ Sample Interview Q&A from Notebook
Q: What happens in PERMISSIVE mode when reading corrupted records?
A: Bad records are replaced with null values.

Q: What is the difference between a transformation and an action in Spark?
A: Transformations are lazy and build the DAG, while actions trigger execution and return results.

Q: How do you store corrupted records for debugging?
A: Use .option("badRecordsPath", "path/to/store") when reading the data.

Q: What is the role of groupBy and join in transformations?
A: They create wide transformations, which shuffle data across partitions, impacting performance.
