# Web Automation Framework with Playwright and Pytest.


Basic Playwright and Pytest testing framework. Framework displays how to test different UI elements and scenarios, utilising  [https://demoqa.com](https://demoqa.com) as a testing sandbox.

## Reports
Framework utilises functionality of the Allure reporter. Reports are stored and displayed via GitHub Pages. There is also an integrated Slack notification, when GitHub Actions run.
HTML Reporting system is hosted at [GitHub Pages](https://shiro-san-ua.github.io/playwright_pytest_demo/).

## Install environment


```
python -m pip install --upgrade pip
pip install pipenv
pipenv install --system
playwright install chromium
```


## Run Playwright tests

Run all set of tests:
``` 
pytest
```
Run one particular test:
```
pytest -k <name of the test>
```
Run tests, marked with a specific mark:
```
pytest -m <name of a Pytest mark>
```


## Generate Allure report

Test report is generated automatically after each test-run, overriding the previous report. Use this command to see the report:
```
allure serve reports
```