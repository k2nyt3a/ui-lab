## Part 0: Getting Ready

### Step 0.1: Chrome Version
- Browser: Google Chrome
- Version: 157.0.8103.51
- OS: Windows 11 (64-bit)

### Step 0.3: ChromeDriver Setup
- ChromeDriver version: 157.0.8103.51
- ChromeDriver path: C:\drivers\chromedriver-win64\chromedriver.exe
- Environment variable: CHROMEDRIVER
- Result: Successfully configured and verified

### Step 0.4: Stable Locators

| Element | Locator | Matches |
|---------|---------|---------|
| Pizza, Please! button | button[name='pizza-please'] | 1 |
| Excluded tools | select | 1 |
| Must be vegetarian | #default-checkbox | 1 |
| Custom Pizza Name | input#pizza-name | 1 |

### Step 0.5: Manual Test Case QP-01

**Test Case ID:** QP-01
**Title:** A custom pizza reaches the admin list

| Step | Expected Result | Actual Result | Status |
|------|-----------------|---------------|--------|
| 1 | Correct homepage heading | Looking to break out of your pizza routine? | PASS |
| 2 | Four Advanced fields appear | All four fields displayed | PASS |
| 3 | Restrictions and pizza name entered correctly | Max calories: 600; Excluded tool: Knife; Vegetarian: checked; Name: Lab Pizza 20261115-022900 | PASS |
| 4 | Correct pizza name, tool other than Knife, calories ≤ 600 | Name: Lab Pizza 20261115-022900; Tool: Pizza cutter; Calories: 500 | PASS |
| 5 | Rating without login requires login | Please log in first. | PASS |
| 6 | Admin login succeeds | Latest pizza recommendations displayed | PASS |
| 7 | Admin list contains the same pizza name and tool | Lab Pizza 20261115-022900 (tool=Pizza cutter, ingredients_number=6) | PASS |

### Step 3.2: First Robot Framework Test

- Initial run: PASS (1 passed, 0 failed)
- Intentional failure: Changed `Web form` to `Web Form`
- Failure reason: Page title did not match the expected title
- Final run: PASS (1 passed, 0 failed)

### Step 3.8: Robot Framework Full Runs

| Run | Result | Tests Passed | Elapsed Time | Pizza Name |
|-----|--------|--------------|--------------|------------|
| Run 1 | PASS | 1/1 | 10.680 s | Lab Pizza 20261115-031114 |
| Run 2 | PASS | 1/1 | 11.133 s | Lab Pizza 20261115-031330 |

Both runs passed using headless Chrome. Each run generated a unique pizza name and completed all seven steps of QP-01.