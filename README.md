# language-model-notebooks
Quickstart for interacting with language models and APIs via a notebook-like interface

George Box: "All models are wrong, but some are useful."

## Quickstart

Look at the demo notebook in a colab: 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jaanli/language-model-notebooks/blob/main/notebooks/getting-started.ipynb)

Or in a browser:
[getting-started.ipynb](notebooks/getting-started.ipynb)

## Installing prerequisities

```
python3 -m venv .venv 
source .venv/bin/activate
pip install -r requirements.txt
```

## Running the notebooks

After installing the prerequisites, you can run the notebooks by running the following command:
```
jupyter lab
```

If a browser window doesn't open automatically, you can navigate to `http://localhost:8888/lab` in your browser and follow the instructions there.

## Testing different closed-source language models via a third-party API

You'll need to add a file called `.env` to this repository, with the following content:
```
PROVIDER_API_KEY=your-api-key
```

Replacing `your-api-key` with your actual OpenAI/Anthropic/Microsoft API key.