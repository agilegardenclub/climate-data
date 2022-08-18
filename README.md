# AGC Climate

## Setup

Retrieve an API token for Azavea from https://app.climate.azavea.com/accounts/api/ and place it in a file named `.env` in the root level of the repository (where this README is contained) with the following syntax

```bash
CLIMATE_API_TOKEN={YOUR_API_TOKEN_HERE}
```

Install dependencies

```bash
pip install -r requirements.txt
```

If you do not have an environment that runs Jupyter Notebooks natively such as VSCode, you can start the jupyter server with

```bash
jupyter notebook .
```

Open the notebook named `climate.ipynb`. Proceed to run all the cells in the notebook by pressing the "Run All" button. If you are using the notebook server started from the command above, it will be located under "Cell" then "Run All".

The notebook will generate an individual JSON file for each of the climate indicators (except ones labeled "threshold") with the monthly historical data over the last 10 years starting from the current month. There will also be a JSON file named `climate_data.json` that will contain all the indicators separated as individual top-level keys within the JSON file. The data is otherwise identical between the individual JSON files and the mergred `climate_data.json` file.
