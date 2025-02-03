# Chat Assistant with FastAPI and SQLite

This is a simple chat assistant built with FastAPI and SQLite. The assistant responds to natural language queries related to employee and department information.

## Features
- Query the employees in a specific department.
- Get the manager of a department.
- Find employees hired after a specific date.
- Calculate total salary expense of a department.

## How it Works
1. The assistant receives a query through a GET request at `/query`.
2. The query is processed using basic natural language processing (NLP) to extract relevant information.
3. The corresponding SQL query is executed on the SQLite database, and the response is returned to the user.

## Steps to Run Locally

1. Clone the repository:
    ```bash
    git clone https://github.com/Om1405/https://github.com/Om1405/Projects/tree/main/ChatBot.git
    cd your-repository-name
    ```

2. Create a virtual environment and activate it:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the FastAPI server:
    ```bash
    uvicorn main:app --reload
    ```

5. Visit the API documentation at `http://127.0.0.1:8000/docs`.

## Known Limitations
- The current version of the assistant only supports basic queries.
- It only handles a limited set of departments and employees.
- The database file is currently static, and changes to it are not reflected in real-time.

## Suggestions for Improvement
- Add support for more departments and employees.
- Implement more advanced NLP for better query understanding.
- Enable the assistant to update or modify the database.

## Deployment Link
https://sql-chatbot-3yk4.onrender.com

## Ask Query Using 
https://sql-chatbot-3yk4.onrender.com/query?q=Your Query
