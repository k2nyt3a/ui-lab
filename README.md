# ui-lab
# Automated UI Testing Lab

**Course:** ITCS386 Software Verification and Validation

This repository contains automated UI tests using two testing tools: Robot Framework (Part 3) and Cypress (Part 4).

## Part 3: Robot Framework

The `robot/` folder contains automated tests for Selenium Web Form and QuickPizza. The `resources/` folder stores reusable keywords, while `results/` contains test reports from two successful runs.

**Run the tests:**

```powershell
cd robot
.\.venv\Scripts\Activate.ps1
robot --outputdir results pizza_scenario.robot
```

## Part 4: Cypress

The `cypress/` folder contains Cypress tests for Selenium Web Form and QuickPizza. It also includes a custom admin login command, screenshots, and videos from the test runs.

**Run the tests:**

```powershell
cd cypress
npm install
npx cypress run --browser chrome
```

## Test Results

Both Robot Framework and Cypress successfully completed QP-01, which checks the pizza restrictions, login requirement, and admin list.

See `RESULTS.md` for detailed test results and reflection answers.