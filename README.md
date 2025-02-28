# Stock insights application

This is a repository for the Stock Prices Insights project. In this project, we are:

1. Loading the data from pickle files(constituent_stock_prices.pkl, constituent_stock_fundamentals.pkl).
2. Storing the data in a SQLite database (Tables: stock_prices, income_statement, balancesheet_statement, cashflow_statement).
3. Using LLMs to create chains for querying insights from this database.

## Steps to Follow

1. Add your OpenAI key to your repository Secrets. 
   
   Go to Settings -> Secrets and Variables -> Codespaces -> New repository secret -> Give Name(eg. OPENAI_KEY) and paste Secret Value

2. Start a Codespace by going to `Code` dropdown > Select `Codespaces` tab > Click on `Create codespace on main`

3. Create and Activate a virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate
   ```

4. Install requirement:
   ```
   pip install -r requirements/requirements.txt
   ```

5. Read data from pickle files and create a database:
   ```
   python main.py
   ```

6. Start application:
   ```
   chainlit run app.py
   ```

7. Once the application is running, access it in browser

8. Stop the application by pressing `Ctrl + C`

9. Delete the Codespace by going to `Code` dropdown > Select `Codespaces` tab > Click on 3 dots (...) showing against your codespace and select `Delete`
