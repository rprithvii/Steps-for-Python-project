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
```
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
```
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
```

**Step6: Contents of requirements.txt file**
```
# --- Core Application ---
# No external libraries needed for basic OOP, but these are helpful as you grow:
pandas==2.1.0        # Great for managing seat layouts as dataframes
tabulate==0.9.0      # Beautifully formats your seat maps in the console

# --- Testing & Prototyping ---
ipykernel            # Allows your Jupyter Notebooks to use this environment
notebook             # The Jupyter Notebook interface
pytest==7.4.0        # The standard tool for testing your OOP classes

# --- Utilities ---
python-dotenv        # Helps manage environment variables (like file paths)
```
**Step7: Install packages from requirements.txt file**
```
conda install -r requirements.txt
```

**Step8: Save environment set up to .yml file**
```
conda env export > environment.yml
```

**Step9: For a new project, create environment based on the .yml file**
```
conda env create --prefix ./venv --file environment.yml
```
