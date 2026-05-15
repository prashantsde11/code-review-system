# Code Review System

A rule-based static code analysis system for detecting bugs, vulnerabilities, code smells, security hotspots, and dead code using AST parsing and pattern-based analysis.

---

# Features

* Static code analysis
* Rule-based issue detection
* Repository scanning
* File-wise issue reporting
* Severity classification
* SonarQube-style dashboard
* Code snippet viewer
* Multi-language project support
* Security issue detection
* Dead code detection
* Code smell detection

---

# Supported Issue Types

## 1. Bug

Runtime or logic-related issues.

Examples:

* Wrong conditions
* Unsafe access
* Possible runtime failures

---

## 2. Vulnerability

Security-related risks.

Examples:

* Hardcoded passwords
* SQL injection patterns
* Exposed secrets
* Unsafe API usage

---

## 3. Code Smell

Maintainability and design issues.

Examples:

* Long functions
* Debug print statements
* Poor naming
* Duplicate logic

---

## 4. Security Hotspot

Sensitive code requiring manual review.

Examples:

* Authentication logic
* Token handling
* Encryption usage
* Access control logic

---

## 5. Dead Code

Unused or unreachable code.

Examples:

* Unused functions
* Unused variables
* Unreachable blocks

---

# Tech Stack

## Frontend

* React
* Vite
* Axios

## Backend

* FastAPI
* Python AST
* Rule-based analysis engine

---

# Project Structure

```text
code-review-system/
│
├── backend/
│   ├── app/
│   ├── engines/
│   ├── routes/
│   └── main.py
│
├── dashboard/
│   ├── src/
│   └── pages/
│
└── README.md
```

---

# Installation

## Backend

```bash
cd backend

python -m venv venv

venv\Scripts\activate

pip install -r requirements.txt

uvicorn app.main:app --reload
```

---

## Frontend

```bash
cd dashboard

npm install

npm run dev
```

---

# Usage

1. Start backend server
2. Start frontend dashboard
3. Enter repository path
4. Click Analyze
5. Review detected issues

Example repository path:

```text
D:\projects\sample-project
```

---

# Dashboard Metrics

The dashboard provides:

* Total files scanned
* Total issues
* Severity distribution
* Issue type distribution
* File-wise analysis
* Code snippet viewer

---

# Example Output

```text
Files: 43
Total Issues: 304

High: 11
Medium: 189
Low: 104

Bug: 0
Vulnerability: 11
Code Smell: 104
Dead Code: 189
```

---

# Future Improvements

* CI/CD integration
* GitHub webhook support
* Pull request analysis
* Duplicate code detection
* Complexity analysis
* Report export (PDF/HTML)
* Custom rule engine
* Multi-language parsers

---

# License

MIT License

---

# Author

Prashant Mishra
