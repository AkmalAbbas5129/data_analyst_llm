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

- Azure OpenAI API Credentials: Store in st.secrets for secure access.
- Database URI: The URI for the SQLite database (e.g., sqlite:///sales_dataset.db).

