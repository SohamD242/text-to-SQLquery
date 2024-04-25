
# AtliQ Fashion Studios: Natural Language to SQL Database Interface
## End-to-End LLM project for a Retail domain

Welcome to AtliQ Fashion Studios, an end-to-end project that leverages Google PaLM and LangChain to create an intelligent system that converts natural language questions into SQL queries, executes them on a MySQL database, and returns the results. This project is ideal for store managers and analysts who need quick answers to questions about inventory, sales, and discounts.

![AtliQ Fashion Studios](atliq_tshirts.png)

## Key Features

- **Database-Backed Information Retrieval**: Users can ask questions in natural language, and the system will generate accurate SQL queries to fetch the relevant information from a MySQL database.
- **T-Shirt Store Context**: AtliQ Fashion Studios is a fictional store that sells various brands like Adidas, Van Heusen, Nike, and Levi's. The database includes information on inventory, sales, and discounts.
- **Tech Stack**: The project uses cutting-edge technology, including:
  - Google PaLM LLM for language processing
  - Hugging Face embeddings
  - Streamlit for the user interface
  - LangChain framework for question-to-query conversion
  - ChromaDB as a vector store
  - Few-shot learning for enhanced query accuracy

## Installation

To set up the project on your local machine, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/SohamD242/text-to-SQLquery.git

```
2. Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
4.Acquire an api key through makersuite.google.com and put it in .env file

```bash
  GOOGLE_API_KEY="your_api_key_here"
```
5. For database setup, run database/db_creation_atliq_t_shirts.sql in your MySQL workbench

## Usage

1. Run the Streamlit app by executing:
```bash
streamlit run main.py

```

2.The web app will open in your browser where you can ask questions

## Sample Questions
  - How many total t shirts are left in total in stock?
  - How much sales amount will be generated if we sell all small size adidas shirts today after discounts?
  - How many t-shirts do we have left for Nike in XS size and white color?
  - How much is the total price of the inventory for all S-size t-shirts?
  
## Project Structure

- main.py: The main Streamlit application script.
- langchain.py: This has all the langchain code
- requirements.txt: A list of required Python packages for the project.
- few_shots.py: Contains few shot prompts
- .env: Configuration file for storing your Google API key.
