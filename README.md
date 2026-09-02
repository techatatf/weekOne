# Week 1 — LLM Foundations

Hands-on notebooks covering probability and neural networks through to
working with live LLM APIs. Every notebook runs in Google Colab in the
browser — no local setup, no installs.

## Notebooks

| # | Notebook | Topics | |
|---|----------|--------|---|
| 01 | [Probability & Neural Networks](01_probability_neural_networks.ipynb) | Probability foundations, network basics | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/samegavi/weekOne/blob/main/01_probability_neural_networks.ipynb) |
| 02 | [LLM Architecture Anatomy](02_llm_architecture_anatomy.ipynb) | Tokenization, embeddings, model internals | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/samegavi/weekOne/blob/main/02_llm_architecture_anatomy.ipynb) |
| 03 | [Transformer Attention](03_transformer_attention.ipynb) | Self-attention, attention maps | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/samegavi/weekOne/blob/main/03_transformer_attention.ipynb) |
| 04 | [Prompting Techniques](04_prompting_techniques.ipynb) | Prompt patterns and evaluation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/samegavi/weekOne/blob/main/04_prompting_techniques.ipynb) |
| 05 | [Free APIs & Integration](05_api_integration.ipynb) | Groq/Gemini APIs, digital twin build | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/samegavi/weekOne/blob/main/05_api_integration.ipynb) |

Facilitators: see `Week 1 Curriculum & Facilitator Guide.docx`.

## How to work on your own version

Click any **Open in Colab** badge above, then **File → Save a copy in
Drive**. That copy is yours — edit and run it freely; nothing you do
affects this repo.

Prefer to keep your work in Git? Fork this repo first, then swap
`samegavi` for your username in the Colab URL. Colab can commit straight
back to your fork via **File → Save a copy in GitHub**.

## Requirements

Notebooks 01–04 need nothing beyond what Colab preinstalls (numpy,
pandas, matplotlib, seaborn, scikit-learn).

Notebook 05 calls a live LLM API and needs a free
[Groq API key](https://console.groq.com). Don't paste the key into a
cell — anything you type into a notebook can end up shared. Use Colab's
Secrets panel instead (🔑 in the left sidebar): add a secret named
`GROQ_API_KEY`, enable notebook access, then read it with

```python
from google.colab import userdata
api_key = userdata.get('GROQ_API_KEY')
```

Running locally instead? Set it as an environment variable and the
notebook's `os.getenv('GROQ_API_KEY')` will pick it up.
