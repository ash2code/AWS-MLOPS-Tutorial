# AWS MLOps Tutorial

A hands-on, 100-day journey through the tools and practices used to build reproducible machine-learning workflows on AWS.

> **Current focus:** setting up the local development foundation before moving on to AWS and MLOps workflows.

## Progress

| Day | Topic | Status |
| ---: | --- | --- |
| 1 | Python virtual environment for ML | ✅ Completed |
| 2 | JupyterLab server configuration | ⬜ Not started |
| 3 | `uv` lockfile | ⬜ Not started |
| 4 | `.gitignore` and Git artifacts | ⬜ Not started |
| 5 | ML workflow `Makefile` | ⬜ Not started |

## Day 1 — Python Virtual Environment for ML

### Objective

Create an isolated Python environment for the project so its packages are separate from system Python and can be recorded for reproducibility.

### Set up the environment

Create a virtual environment:

```bash
python3 -m venv ml-env
```

Activate it on macOS or Linux:

```bash
source ml-env/bin/activate
```

Confirm that Python and pip resolve to the environment, then inspect installed packages:

```bash
which python
which pip
pip freeze
```

Save the installed dependencies to `requirements.txt`:

```bash
pip freeze > requirements.txt
```

### What I learned

- Why Python virtual environments are useful for ML projects.
- How system Python differs from the Python inside an activated environment.
- How activation changes the `python` and `pip` paths.
- How `pip` installs packages and `pip freeze` lists installed dependencies.
- How `requirements.txt` helps record dependencies for reproducibility.

### Issue encountered

I initially ran `python freeze`. Python interpreted `freeze` as a script name. The correct command is:

```bash
pip freeze
```

### Status

✅ **Completed**

---

*This README will be updated as the 100-day journey progresses.*
