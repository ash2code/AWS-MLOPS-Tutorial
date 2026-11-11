#AWS-MLOPS-Tutorial

MLOps 100-Day Hands-On Journey
Progress
Day	Topic	Status
1	Python Virtual Environment for ML	🔨 In Progress
2	JupyterLab Server Configuration	⬜ Not Started
3	uv Lockfile	⬜ Not Started
4	.gitignore and Git Artifacts	⬜ Not Started
5	ML Workflow Makefile	⬜ Not Started


Day 1 - Python Virtual Environment for ML
Objective
Create an isolated Python environment for the ML project.

Hands-On
Create environment
python3 -m venv ml-env

Activate environment
source ml-env/bin/activate

Verify Python
which python

Verify pip
which pip

Check dependencies
pip freeze

Save dependencies
pip freeze > requirements.txt

What I Learned
Why Python virtual environments are required
System Python vs virtual-environment Python
How environment activation changes the Python/pip paths
How pip manages packages
How pip freeze captures installed dependencies
Why requirements.txt helps reproducibility
Issues Encountered
I initially used:

python freeze

Python treated freeze as a Python file.

The correct command is:

pip freeze

Status
✅ Completed
