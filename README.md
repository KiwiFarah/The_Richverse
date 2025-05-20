# The Richverse – Portfolio Analytics Dashboard

> **Personal Developer Fork by Farah Warnakulasuriya**  
> A polished and professionally engineered version of the Richverse app originally built during CITS5505 at UWA.  
> This version showcases my end-to-end skills in backend engineering, frontend design, testing, and secure application architecture.

---

## 🚀 Overview

**The Richverse** is a full-stack investment portfolio dashboard built using **Flask**, **Chart.js**, and **SQLAlchemy**. It empowers users to create, analyze, and benchmark financial portfolios using real-world historical market data. 

This version reflects significant contributions and refactoring by me to ensure robustness, extensibility, and industry-grade software practices.

---

## 🔧 Technologies Used

| Layer       | Tools & Libraries                            |
|-------------|----------------------------------------------|
| Backend     | Python, Flask, SQLAlchemy, WTForms           |
| Frontend    | HTML, CSS, JavaScript, Chart.js              |
| Database    | SQLite (Production + In-memory for Testing)  |
| Testing     | unittest, Selenium, Headless ChromeDriver    |
| Data APIs   | Yahoo Finance via `yfinance`                 |

---

## Key Engineering Highlights

- **Refactored Secure Login System**: Enhanced WTForms validation and password handling for security and clarity.
- **Modularized Chart Rendering**: Created reusable Chart.js components including heatmaps, donut allocations, and cumulative returns.
- **Test Automation**: Developed a comprehensive suite of unit tests and Selenium tests that simulate real browser interaction.
- **CLI Developer Tools**: Added commands to automate environment setup, data seeding, and price refresh logic.
- **Clean Architecture**: Reorganized routes, models, and frontend logic for maximum clarity, maintainability, and separation of concerns.

---

## How to Run

### 1. Clone this repository
```bash
git clone https://github.com/KiwiFarah/CITS5505_Richverse_Fork.git
cd CITS5505_Richverse_Fork
```

### 2. Set up your environment
```bash
python -m venv venv
source venv/bin/activate  # Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Run database migrations
```bash
flask db upgrade
```

### 4. Launch the app
```bash
python run.py
```
Visit `http://localhost:5000`

---

## Testing

### Unit Tests
```bash
python tests/run_unit_tests.py
```

### Selenium UI Tests (Live Server)
```bash
python -m unittest discover -s tests/seleniumTests -p "*.py"
```

All tests run using in-memory SQLite with seeded test users and headless Chrome.

---

## References & Inspiration

- Charting: [Chart.js](https://www.chartjs.org/docs/latest/)
- Backend: [Flask](https://flask.palletsprojects.com/), [SQLAlchemy](https://www.sqlalchemy.org/)
- Market Data: [yfinance](https://pypi.org/project/yfinance/)
- Testing: [Selenium](https://www.selenium.dev/documentation/)
- Portfolio Theory: Bodie et al., Sharpe Ratio (CAPM), Morningstar, Portfolio Visualizer

---

## Author

**Farah Warnakulasuriya**  
MSc Computer Science @ University of Western Australia  
[GitHub – KiwiFarah](https://github.com/KiwiFarah)

---

> This fork demonstrates my ability to take an academic group project and elevate it into a professional-grade portfolio platform with full test coverage and clear architecture.