# Scraping Data from a Real Website + Pandas 🔍
[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)

This repository contains a Jupyter Notebook that scrapes the Wikipedia page "List of largest companies in the United States by revenue" and converts the extracted table into a Pandas DataFrame.

Files
- [data scrapping from a sample website..ipynb](data scrapping from a sample website..ipynb) — main notebook.
- [requirements.txt](requirements.txt) — Python dependencies.

Key symbols in the notebook
- [`soup`](data scrapping from a sample website..ipynb) — BeautifulSoup object created from the fetched page.
- [`table`](data scrapping from a sample website..ipynb) — selected HTML table element.
- [`df`](data scrapping from a sample website..ipynb) — resulting Pandas DataFrame created from the table.
- [`df.to_csv`](data scrapping from a sample website..ipynb) — cell that writes the DataFrame to CSV (update the output path before running).

Requirements
- Python 3.9 (notebook metadata indicates Python 3.9.13)
- See [requirements.txt](requirements.txt) for the exact packages.

Quick start
1. Create and activate a virtual environment (recommended):
   - python -m venv .venv
   - Windows: .venv\Scripts\activate
   - macOS/Linux: source .venv/bin/activate
2. Install dependencies:
   - pip install -r requirements.txt
3. Open the notebook:
   - In VS Code: open [data scrapping from a sample website..ipynb](data scrapping from a sample website..ipynb)
   - Or start Jupyter: jupyter notebook
4. Run cells top-to-bottom. Before exporting, update the CSV output path in the cell that calls [`df.to_csv`](data scrapping from a sample website..ipynb).

Notes
- The notebook currently fetches data from: https://en.wikipedia.org/wiki/List_of_largest_companies_in_the_United_States_by_revenue
- If the page structure changes, update the table selection logic in the notebook.
