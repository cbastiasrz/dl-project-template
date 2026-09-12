# Boiler template for deep learning related projects.

The folder structure is the following:

ml-churn/
├── pyproject.toml        # the wish
├── uv.lock               # the answer
├── Makefile              # the verbs
├── Dockerfile
├── .pre-commit-config.yaml
├── conf/
│   ├── base.yaml         # all parameters and paths
│   └── ci.yaml           # small overrides for CI
├── src/churn/
│   ├── config.py         # load YAML into a typed object
│   ├── data.py           # ingest and split
│   ├── features.py       # transforms
│   ├── train.py          # main(cfg) -> model, metrics
│   └── evaluate.py
├── tests/
├── notebooks/            # imports from src, defines nothing
├── data/                 # git-ignored; DVC manages it in phase 2
└── README.md