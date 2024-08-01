# Data Analysis Expert

Data Analysis Expert is a Streamlit-based web application designed to provide data analysis insights using advanced AI models. The app integrates with Azure OpenAI and utilizes LangChain for natural language processing and data analysis, generating comprehensive reports based on user queries.

## Table of Contents
1. [Codebase](#codebase)
2. [Dependencies](#dependencies)
3. [Environment Configurations](#environment-configurations)
4. [Input Data](#input-data)
5. [Expected Output](#expected-output)
6. [Installation and Execution Instructions](#installation-and-execution-instructions)
7. [Additional Documentation](#additional-documentation)

## Codebase

### File Structure
- `streamlit_app.py`: Main Streamlit application file that handles the UI and integrates with backend services for data analysis.
- `utils.py`: Utility functions for generating KPIs, executing SQL queries, and formatting output data.

## Dependencies

The project requires several Python packages, which are listed in the `requirements.txt` file:

- `langchain`
- `langchain-core`
- `langchain-community`
- `pandas`
- `streamlit`
- `openai`
- `tabulate`
- `openpyxl`

These packages can be installed using pip:

```sh
pip install -r requirements.txt
```

## Environment Configurations
To run the application, you'll need to set up environment variables and configuration files. Key configurations include:

- Azure OpenAI API Credentials: Store in st.secrets or .env for secure access.
- Database URI: The URI for the SQLite database (e.g., sqlite:///sales_dataset.db).

## Secrets or .env file sample
```sh
openai_api_key: "<your_openai_api_key>"
azure_endpoint: "<your_azure_endpoint>"
deployment_name: "<your_deployment_name>"
model_name: "<your_model_name>"
```

## Input Data

The application expects the following inputs from the user:

1. **User Question**: A detailed question or problem statement related to data analysis.
2. **Domain Selection**: The domain or category of data the user is interested in analyzing.

## Example Input
```markdown
**User Question:** 
How can we optimize sales performance in the retail sector using historical sales data?
```

## Expected Output
```
**SQL Query:**
SELECT * FROM sales WHERE ...

**Data Analysis Report:**
- KPI 1: ...
- KPI 2: ...
...

**Output Data:**
| Column 1 | Column 2 | ... |
|----------|----------|-----|
| Data 1   | Data 2   | ... |
...

```
