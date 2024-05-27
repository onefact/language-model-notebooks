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

Then after activating (`source .venv/bin/activate`) run jupyter lab `jupyter lab`. You will need to make sure to activate the virtual environment every time you restart your computer or shell session.

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

## Applications that are helpful for working with large language models

On a Mac, you can install the following applications to make working with large language models easier:

- Maccy: clipboard manager (https://maccy.app/): `brew install maccy`
- Rectangle: window manager (https://rectangleapp.com/): `brew install rectangle`
- Amethyst: tiling window manager (https://ianyh.com/amethyst/): `brew install amethyst`

There are equivalents on Windows, that can be installed with chocolatey.org, such as copyq: `choco install copyq`.

## Enabling word wrapping in Jupyter Lab

Inside a virtual environment, run the following command:
```
which jupyter-lab
```

This will give you a path:

```
/Users/me/projects/language-model-notebooks/.venv/bin/jupyter-lab
```

Alternatively:
```
jupyter --path
```

You can then edit the settings file:

```
code ~/.jupyter/lab/user-settings/@jupyterlab/notebook-extension/tracker.jupyterlab-settings
```

And add the following to make sure line wrapping and code cell wrapping is on:

```
{
  "MarkdownCell": {
    "cm_config": {
      "lineWrapping": true
    }
  },
  "CodeCell": {
    "cm_config": {
      "lineWrapping": true
    }
  }
}
```

## Enabling GitHub Copilot support in Jupyter Lab

- [ ] TODO
