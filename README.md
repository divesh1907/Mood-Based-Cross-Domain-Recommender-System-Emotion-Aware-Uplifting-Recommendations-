# Recommender System Project

This repository contains a cross-domain uplift recommender system implemented in Python.

## Contents
- `notebook.ipynb` — original development notebook.
- `module.py` — extracted Python module.
- `requirements.txt` — dependencies.
- `.gitignore` — standard ignores.

## Usage
```
pip install -r requirements.txt
python module.py
```

## Overview
This project implements a **cross-domain content-based recommender system** capable of suggesting **songs, movies, and books** based on a user's **emotional state, mood, or textual query**. Unlike traditional recommenders that operate on a single domain, this system unifies multiple content domains into a **single semantic search space**, allowing a user to receive recommendations across media types using the same query.

## Key Features
- Cross-domain recommendation across songs, movies, and books.
- Natural-language querying using TF-IDF and cosine similarity.
- Evaluation metrics including Precision@K, nDCG@K, Coverage, and Popularity Bias.
- Optional Streamlit app for interactive use.

## Architecture & Methodology
1. Data loading of three domain datasets.
2. TF-IDF vectorization of corpus.
3. Query vectorization and cosine similarity search.
4. Ranking, scoring, and metric computation.
5. Optional Streamlit UI.

## Project Structure
```
recsys-project/
├─ src/recsys/
│  ├─ core.py
│  └─ __init__.py
├─ app.py
├─ notebooks/
│  └─ Recommender System Project final.ipynb
├─ scripts/
│  └─ run_demo.py
├─ tests/
│  └─ test_import.py
├─ data/
│  └─ .gitkeep
├─ requirements.txt
├─ dev-requirements.txt
├─ pyproject.toml
├─ README.md
├─ LICENSE
└─ .gitignore
```

## Usage
```
pip install -r requirements.txt
python scripts/run_demo.py
```

## Streamlit
```
streamlit run app.py
```

## Future Enhancements
- Upgrade to Sentence Transformers.
- Add collaborative filtering.
- Add multi-stage re-ranking.
