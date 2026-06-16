<!-- ===================== HERO ===================== -->
<div align="center">

<img src="assets/banner.svg" alt="LangChain Notes" width="100%" />

<br/>

<!-- Badges -->
<a href="#"><img alt="Python" src="https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white"></a>
<a href="#"><img alt="LangChain" src="https://img.shields.io/badge/LangChain-ecosystem-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"></a>
<a href="#"><img alt="uv" src="https://img.shields.io/badge/managed%20with-uv-DE5FE9?style=for-the-badge&logo=astral&logoColor=white"></a>
<a href="#"><img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white"></a>
<br/>
<img alt="Status" src="https://img.shields.io/badge/status-actively%20growing-5FD6BE?style=flat-square">
<img alt="Type" src="https://img.shields.io/badge/type-learning%20journal-F4A259?style=flat-square">

</div>

<br/>

> A living notebook where I keep the **notes and code** from studying the LangChain library — one topic at a time. Not a course, not a tutorial repo, just my own working understanding written down as I go. New modules get added as I learn them.

<br/>

## 📓 What's inside

Each module is a self-contained Jupyter notebook focused on one corner of the framework. Status reflects where my notes currently stand.

| # | Module | Focus | Status |
|:--:|:--|:--|:--:|
| 01 | [`langchain_intro`](updatedlangchain/langchain_intro.ipynb) | Core concepts, first chains, the mental model | 🟡 In progress |
| 02 | [`messages`](updatedlangchain/messages.ipynb) | System / human / AI messages & prompt structure | 🟡 In progress |
| 03 | [`modelintegration`](updatedlangchain/modelintegration.ipynb) | Wiring up OpenAI, Groq & Google models | 🟡 In progress |
| 04 | [`tools`](updatedlangchain/tools.ipynb) | Tool calling and giving models hands | 🟡 In progress |

<sub>🟢 solid · 🟡 in progress · ⚪ planned — update these as the notes mature.</sub>

<br/>

## 🧰 Stack

The notebooks are model-agnostic on purpose — the same patterns are tried across a few providers.

| Layer | What I'm using |
|:--|:--|
| **Framework** | `langchain` · `langchain-community` |
| **Model providers** | `langchain-openai` · `langchain-groq` · `langchain-google-genai` |
| **Config / secrets** | `python-dotenv` |
| **Environment** | `uv` · `ipykernel` · Python 3.11+ |

<br/>

## 🗂️ Repo structure

```text
LangChain-Notes/
├── updatedlangchain/          # the notebooks — one topic each
│   ├── langchain_intro.ipynb
│   ├── messages.ipynb
│   ├── modelintegration.ipynb
│   └── tools.ipynb
├── assets/
│   └── banner.svg             # header art
├── main.py                    # scratch entry point
├── pyproject.toml             # project + dependencies
├── requirement.txt            # plain-pip dependency list
└── uv.lock                    # pinned, reproducible versions
```

<br/>

## 🚀 Getting started

**1. Clone**

```bash
git clone https://github.com/<your-username>/LangChain-Notes.git
cd LangChain-Notes
```

**2. Install dependencies**

<details open>
<summary><b>With <code>uv</code> (recommended)</b></summary>

```bash
uv sync          # installs from uv.lock into a fresh .venv
```
</details>

<details>
<summary><b>With plain <code>pip</code></b></summary>

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirement.txt
```
</details>

**3. Add your API keys**

Create a `.env` file in the project root with whichever providers you want to run:

```env
OPENAI_API_KEY=sk-...
GROQ_API_KEY=gsk_...
GOOGLE_API_KEY=...
```

**4. Open the notebooks**

```bash
jupyter lab        # or open the folder in VS Code / Cursor
```

Then start with `updatedlangchain/langchain_intro.ipynb` and work down the list.

<br/>

## 🛣️ Roadmap

Topics I want to fold into the notebook next:

- [ ] **LCEL** — chaining with the pipe (`|`) syntax
- [ ] **Prompt templates** — reusable, parameterized prompts
- [ ] **Output parsers** — structured & typed outputs
- [ ] **Memory** — keeping context across turns
- [ ] **RAG** — embeddings, vector stores & retrieval
- [ ] **Agents** — reasoning loops over tools
- [ ] **LangGraph** — stateful, multi-step graphs

<br/>

## 🎯 Why this repo exists

This is a **personal study log**, kept public in case the notes help someone walking the same path. Explanations are in my own words, code is meant to be run and broken, and everything is a work in progress by design. Spotted something off or have a better way? Issues and suggestions are welcome.

<br/>

<div align="center">
<sub>Built while learning · maintained out of curiosity 🦜🔗</sub>
</div>
