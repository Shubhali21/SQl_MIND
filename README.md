# SQLMind

**SQLMind** is an AI-powered agent system that lets users query the **Chicago Crime Dataset** using natural language. It uses the **Gemini API** to convert natural language queries into SQL and fetches results  from a **DuckDB** database.

---

## 📦 Features

- Converts natural language to SQL using Gemini API
- Retrieves real-time data from the Chicago Crime Dataset (2023–May 2025)
- Validates data using `pointblank`
- Executes queries using DuckDB
- Returns query results as clean, readable **tables**

---

## 🔗 Data Source

- **Chicago Data Portal**  
  Dataset: [Chicago Crime](https://data.cityofchicago.org/)  
  Filter: From **January 2023 to May 2025**

---

## 🏗️ System Architecture

![System Architecture](architecture%201.png)

### Components

- **Create Prompt**: Transforms natural language questions into SQL prompts
- **API Handler**: Communicates with the Gemini API to generate SQL queries
- **DB Handler**: Takes the query and returns a dataframe 
- **Data Validator**: Uses `pointblank` for schema and data validation
- **Output**: Displays final result as an **table**

---

## ⚙️ TechStack

| Technology         | Purpose                                           |
|--------------------|---------------------------------------------------|
| **Python**         | Core development language                         |
| **Gemini API**     | Converts user input into SQL                      |
| **DuckDB**         | Embedded SQL query engine                         |
| **pandas**         | Data manipulation and tabular formatting          |
| **pointblank**     | Data validation and schema checks                 |
| **Chicago Data API** | Source for live crime data from city portal     |


---


---



