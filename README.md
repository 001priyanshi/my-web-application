# Simple Python CI/CD Application

## Project Overview
This project demonstrates a basic CI/CD pipeline using GitHub Actions for a Python application. The pipeline automates building, testing, and deployment.

---

## Application Configuration

- Language: Python 3.10  
- Testing Framework: pytest  
- CI/CD Tool: GitHub Actions  

---

## CI/CD Pipeline Configuration

The pipeline is defined in:
.github/workflows/ci-cd.yml

### Trigger
- Runs automatically on every push to the `main` branch.

### Stages

1. **Build Stage**
   - Installs dependencies using:
     ```
     pip install -r requirements.txt
     ```

2. **Test Stage**
   - Runs automated tests using:
     ```
     python -m pytest
     ```

3. **Deployment Stage**
   - Simulates deployment by copying files into a `deploy/` folder.

---

## Project Structure
  - Simple-Web-Application/
│
├── app.py
├── test_app.py
├── requirements.txt
└── .github/
└── workflows/
└── ci-cd.yml


---

## How to Run Locally

1. Install dependencies:
   - pip install -r requirements.txt
2. Run the application:
   - python app.py
3. Run tests:
   - python -m pytest

---

## Expected Output

- Application Output: `5`
- Test Result: `1 passed`
- CI/CD Pipeline: Successful execution in GitHub Actions

---

## CI/CD Workflow Explanation:

- The workflow is triggered automatically on every push to the main branch.
- The repository code is checked out and a Python environment is set up.
- Required dependencies are installed using the requirements file.
- Automated tests are executed using pytest to verify the application.
- If tests pass, the application is deployed through a simulated deployment process.

---
