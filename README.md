# AGC Climate

## Setup

Retrieve an API token for Azavea from https://app.climate.azavea.com/accounts/api/ and place it in a `.env` with the following syntax

```bash
CLIMATE_API_TOKEN={YOUR_API_TOKEN_HERE}
```

Install dependencies

```bash
pip install requirements.txt
```

If you do not have an environment that runs Jupyter Notebooks natively such as VSCode, you can start the jupyter server with

```bash
jupyter notebook .
```

Run all the cells in `climate.ipynb`
