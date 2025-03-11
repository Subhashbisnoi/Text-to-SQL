# Text-to-SQL Streamlit App

This project is a **Streamlit-based web application** that converts natural language queries into **SQL commands** and retrieves results from an SQLite database.

## 🚀 Features
- Converts English questions to SQL queries using **LangChain & Groq LLM**.
- Supports querying an SQLite database (`students.db`).
- Displays the results of the executed SQL queries.
- Example SQL queries:
  - *"How many entries of records are present?"* → `SELECT COUNT(*) FROM STUDENT;`
  - *"Tell me all the students studying in Data Science COURSE?"* → `SELECT * FROM STUDENT WHERE COURSE="Data Science";`

## 📂 Project Structure
```
📁 text-to-sql
│── main.py              # Streamlit application for user interaction
│── database.py          # Creates SQLite database & inserts sample records
│── requirements.txt     # Lists required Python libraries
│── README.md            # Documentation
```

## 📥 Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/text-to-sql.git
   cd text-to-sql
   ```

2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

3. Set up the **Groq API key** (required for LLM-based SQL conversion):
   ```sh
   export GROQ_API_KEY="your_api_key_here"
   ```

4. Run the database script to create `students.db`:
   ```sh
   python database.py
   ```

5. Start the Streamlit app:
   ```sh
   streamlit run main.py
   ```

## 🛠 Technologies Used
- **Streamlit** - Interactive web interface
- **LangChain** - Query conversion using LLM
- **Groq LLM** - Converts natural language to SQL
- **SQLite** - Database for storing student data
- **Python** - Core programming language

## 🖥️ Usage
1. Enter a natural language question in the **input box**.
2. Click **"Enter"** to generate & execute the SQL query.
3. The retrieved results will be displayed on the screen.

🔗 **Live Demo**: [Text-to-SQL Web App](https://text-to-sql-data.streamlit.app/)

## 📜 License
This project is open-source and available under the **MIT License**.

---
💡 **Feel free to contribute and enhance this project!**
