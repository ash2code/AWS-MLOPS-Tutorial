<div align="center">

# AWS MLOps Tutorial

### A 100-day, hands-on journey to building practical and reproducible machine-learning workflows with AWS.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-Learning%20path-232F3E?logo=amazonaws&logoColor=white)
![Journey](https://img.shields.io/badge/100--day-journey-6C63FF)

</div>

---

## About this project

This repository documents a hands-on learning journey through the foundations of MLOps, machine-learning development, and AWS. Each day focuses on a practical topic, with notes and commands captured along the way.

**Current focus:** creating a clean, reproducible local Python development environment.

## Learning roadmap

| Day | Topic | Status |
| ---: | --- | :---: |
| 1 | Python virtual environment for ML | ✅ Complete |
| 2 | JupyterLab server configuration | ⬜ Not started |
| 3 | `uv` lockfile | ⬜ Not started |
| 4 | `.gitignore` and Git artifacts | ⬜ Not started |
| 5 | ML workflow `Makefile` | ⬜ Not started |

> The roadmap will grow as the journey progresses.

## Day 1 — Python virtual environment for ML

### Goal

Create an isolated Python environment so project packages stay separate from system Python and can be recorded for future setup.

### Create and activate the environment

The commands below are for macOS and Linux.

```bash
python3 -m venv ml-env
source ml-env/bin/activate
```

### Verify Python and pip

With the environment active, check that Python and pip point to the virtual environment and inspect the installed packages:

```bash
which python
which pip
pip freeze
```

### Record dependencies

```bash
pip freeze > requirements.txt
```

This records the packages currently installed in the active environment. It can be used as a starting point for recreating the environment.

### Key takeaways

- Virtual environments isolate project dependencies from system Python.
- Activating the environment changes which `python` and `pip` commands are used.
- `pip freeze` lists installed packages, and redirecting its output records them in `requirements.txt`.

### Troubleshooting note

I initially ran `python freeze`, which makes Python look for a script named `freeze`. To list installed packages, use:

```bash
pip freeze
```

**Day 1 status: ✅ Complete**

---

## Follow the journey

As new topics are completed, this README will be updated with progress, hands-on steps, and lessons learned.
