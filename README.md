# AWS MLOps Tutorial

This repository is my learning log for a 100-day MLOps journey.

## Progress

| Day | Topic | Status |
| ---: | --- | --- |
| 1 | Python virtual environment for ML | ✅ Completed |
| 2 | JupyterLab server configuration | ⬜ Not started |
| 3 | `uv` lockfile | ⬜ Not started |
| 4 | `.gitignore` and Git artifacts | ⬜ Not started |
| 5 | ML workflow `Makefile` | ⬜ Not started |

## Day 1 - Python Virtual Environment for ML

### Objective

Create an isolated Python environment for the project so dependencies do not mix with the system Python.

### Create environment

```bash
python3 -m venv ml-env
```

### Activate environment

```bash
source ml-env/bin/activate
```

### Check Python and pip

```bash
which python
which pip
pip freeze
```

### Save dependencies

```bash
pip freeze > requirements.txt
```

### What I learned

- Why Python virtual environments are needed
- How system Python is different from environment Python
- How activation changes the `python` and `pip` paths
- How `pip` installs packages
- How `pip freeze` helps save dependencies
- Why `requirements.txt` helps reproducibility

### Issue I faced

I first tried:

```bash
python freeze
```

That did not work because Python treated `freeze` like a file name.

The correct command is:

```bash
pip freeze
```

### Status

✅ Completed

This README will be updated as I continue the MLOps journey.
