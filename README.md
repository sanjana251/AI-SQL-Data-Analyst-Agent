**🧠 AI SQL Data Analyst Agent**

An AI-powered data analysis application that allows users to upload CSV datasets and ask questions in natural language. The application converts natural language questions into SQL queries, executes them on a SQLite database, explains the results, and generates interactive visualizations.

## 🚀 Features

* 📂 Upload and analyze CSV datasets
* 🧠 Convert natural language questions into SQL queries using Groq LLM
* 🔎 Display the generated SQL query
* 📊 Execute SQL queries on an SQLite database
* 💡 Provide plain-English explanations of results
* 📈 Automatically generate suitable visualizations
* 🗂️ Display database schema and dataset preview
* 🛠️ Support direct SQL query execution
* 📋 Display dataset statistics such as rows, columns, and file size
* 🎨 Modern and responsive Streamlit interface

## 🛠️ Technologies Used

* **Python**
* **Streamlit** – Web application interface
* **Pandas** – Data processing
* **SQLite** – Database management
* **Groq API** – AI-powered SQL generation
* **Plotly** – Interactive data visualization
* **Matplotlib** – Data visualization
* **JSON** – Structured AI responses

## 🔄 How It Works

```text
CSV Dataset
     ↓
Upload to Streamlit
     ↓
Pandas Data Processing
     ↓
SQLite Database
     ↓
User asks question in Natural Language
     ↓
Groq LLM analyzes schema and question
     ↓
SQL Query Generated
     ↓
SQL Query Executed
     ↓
Result + Explanation
     ↓
Interactive Visualization
```

## 📋 Example

A user can upload a CSV dataset and ask:

```text
What are the top 5 products by total sales?
```

The AI generates an SQL query such as:

```sql
SELECT product, SUM(sales) AS total_sales
FROM data
GROUP BY product
ORDER BY total_sales DESC
LIMIT 5;
```

The query is executed against the SQLite database and the results are displayed along with an appropriate visualization.

## 📁 Project Structure

```text
AI-SQL-Data-Analyst-Agent/
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/AI-SQL-Data-Analyst-Agent.git
```

### 2. Navigate to the project folder

```bash
cd AI-SQL-Data-Analyst-Agent
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

**Windows PowerShell:**

```bash
.\venv\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

## 🔑 API Key Configuration

This project uses the Groq API for AI-powered SQL generation.

For local development, add your API key in `app.py`:

```python
groq_api_key = "YOUR_GROQ_API_KEY"
```

**Important:** Never upload your real API key to GitHub.

For deployment, use Streamlit Secrets instead of hard-coding the API key.

## ▶️ Run the Application

Start the Streamlit application using:

```bash
streamlit run app.py
```

The application will open in your browser at:

```text
http://localhost:8501
```

## 📊 Application Workflow

### 1. Upload Dataset

Upload any suitable CSV dataset through the application.

### 2. Preview Data

The application displays the number of rows, columns, file size, and a preview of the dataset.

### 3. Ask a Question

Enter a question about the uploaded dataset using normal English.

### 4. Generate SQL

The Groq-powered AI analyzes the database schema and generates an appropriate SQLite SQL query.

### 5. View Results

The generated query is executed and the results are displayed in a structured table.

### 6. Visualize Data

The application automatically selects an appropriate visualization such as a bar chart, line chart, pie chart, or scatter plot.

## 🎯 Use Cases

* Business data analysis
* Exploratory data analysis
* CSV-based reporting
* SQL learning and practice
* Quick data exploration
* Natural-language database querying

## 🔮 Future Enhancements

* Support for multiple datasets
* Advanced conversational memory
* More visualization types
* Export reports as PDF
* Support for larger databases
* Cloud database integration
* User authentication
* AI-generated analytical summaries

## 👩‍💻 Author

Sanjana Nadiger

Computer Science Engineering Graduate
Interested in **Data Science, AI/ML, SQL, and Full Stack Development**
