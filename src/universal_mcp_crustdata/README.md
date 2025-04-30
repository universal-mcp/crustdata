# Universal Mcp Crustdata MCP Server

An MCP Server for the Universal Mcp Crustdata API.

## 📋 Prerequisites

Before you begin, ensure you have met the following requirements:
* Python 3.11+ (Recommended)
* [uv](https://github.com/astral-sh/uv) installed globally (`pip install uv`)

## 🛠️ Setup Instructions

Follow these steps to get the development environment up and running:

### 1. Sync Project Dependencies
Navigate to the project root directory (where `pyproject.toml` is located).
```bash
uv sync
```
This command uses `uv` to install all dependencies listed in `pyproject.toml` into a virtual environment (`.venv`) located in the project root.

### 2. Activate the Virtual Environment
Activating the virtual environment ensures that you are using the project's specific dependencies and Python interpreter.
- On **Linux/macOS**:
```bash
source .venv/bin/activate
```
- On **Windows**:
```bash
.venv\\Scripts\\activate
```

### 3. Start the MCP Inspector
Use the MCP CLI to start the application in development mode.
```bash
mcp dev src/universal_mcp_crustdata/mcp.py
```
The MCP inspector should now be running. Check the console output for the exact address and port.

## 🔌 Supported Integrations

- AgentR
- API Key (Coming Soon)
- OAuth (Coming Soon)

## 🛠️ Tool List

This is automatically generated from OpenAPI schema for the Universal Mcp Crustdata API.

| Tool | Description |
|------|-------------|
| `screen_companies` | Screens companies based on specified metrics, filters, sorting, and pagination parameters, and returns the result as a JSON-compatible dictionary. |
| `get_headcount_timeseries` | Retrieve headcount timeseries data from the data lab endpoint using the provided filters, pagination, and sorting options. |
| `get_headcount_by_facet_timeseries` | Retrieves headcount timeseries data aggregated by specified facets using provided filters and sorting options. |
| `get_funding_milestone_timeseries` | Retrieves a time series of funding milestone data based on specified filters, pagination, and sorting options. |
| `get_decision_makers` | Retrieves decision makers based on specified filters and parameters. |
| `get_web_traffic` | Retrieves web traffic data based on provided filters, pagination, and sorting criteria. |
| `get_investor_portfolio` | Retrieves the investment portfolio information for a specified investor. |
| `get_job_listings` | Retrieves job listings data based on specified parameters. |
| `search_persons` | Submits a search request for persons associated with a given asynchronous job and returns the search results as a dictionary. |
| `search_companies` | Searches for companies using specified filters and pagination parameters. |
| `enrich_person` | Retrieves enriched person data from LinkedIn profile using the provided profile URL, enrichment mode, and requested fields. |
| `enrich_company` | Retrieves enriched company data using the provided company domain and enrichment mode. |
| `get_linked_in_posts` | Fetches LinkedIn posts for a specified company using its LinkedIn URL. |
| `search_linked_in_posts` | Searches LinkedIn posts using the provided keyword and filters, returning the search results as a dictionary. |

## 📁 Project Structure

The generated project has a standard layout:
```
.
├── src/                  # Source code directory
│   └── universal_mcp_crustdata/
│       ├── __init__.py
│       └── mcp.py        # Server is launched here
│       └── app.py        # Application tools are defined here
├── tests/                # Directory for project tests
├── .env                  # Environment variables (for local development)
├── pyproject.toml        # Project dependencies managed by uv
├── README.md             # This file
```

## 📝 License

This project is licensed under the MIT License.

---

_This project was generated using **MCP CLI** — Happy coding! 🚀_
