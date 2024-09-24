# T-504-ITML-Project-1


# Diabetes Prediction Project

This project is focused on predicting diabetes using machine learning models.
Follow the instructions below to get started.

## Getting Started

### Prerequisites
- Python 3.8, 3.9, 3.10, or 3.11 (at this time PyCaret is **not** fully yet supported on Python 3.12)
- Virtual environment setup tools (`venv` or `virtualenv`)
- Homebrew (for macOS users)

### Setup Instructions

1. **Create a Virtual Environment:**
    #### Create a virtual environment in the project directory:
    ```bash
    python -m venv .venv
    ```

2. **Activate the Virtual Environment:**
    
    On macOS/Linux:
    ```bash
    source .venv/bin/activate
    ```
    
    On Windows:
    ```bash
    .venv\Scripts\activate
    ```

3. **Install Required Dependencies:**

    Install all the necessary packages from requirements.txt:
    ```bash
    pip install -r requirements.txt
    ```
4. **Run the Project:**

    Once the environment is set up, run your code:
    ```bash
    python predict_diabetes.ipynb
    ```

## Known Issues
While trying to run this project we stumbled on an issue with libomp (https://openmp.llvm.org) on macos. The error surficed while trying to run the machine learning models in PyCaret (e.g., issues related to OpenMP). The issue was solved by installing libomp via homebrew:

```bash
brew install libomp
````

Hopefully this helps if you encounter the same issue.
