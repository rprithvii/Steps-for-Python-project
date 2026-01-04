# Steps-for-Python-project


**Step1:**
```
conda create --prefix ./.venv python=3.11
```
**Step2:**
```
conda activate ./.venv
```
**Folder structure**
CinemaSeatBooking/
│
├── venv/                   # Virtual environment
├── main.py                 # Main entry point
├── requirements.txt
│
├── notebooks/              # <--- New Sandbox Folder
│   ├── 01_test_logic.ipynb # Experimenting with Seat assignments
│   └── 02_prototyping.ipynb# Testing UI/Flow
│
├── src/                    # Official Project Logic
│   ├── __init__.py
│   ├── cinema.py
│   └── seat.py
│
└── data/                   
    └── layout.json

**Step3:**
```
conda install jupyter
```

**Step4:**
```
conda install ipykernel
```

**Step5:**
```
python -m ipykernel install --user --name=cinema_env --display-name "Python (Cinema Project)"
