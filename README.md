## 💡 Project Readme: Development Environment & Version Control

This repository is dedicated to establishing the core infrastructure for a data analysis project, focusing on **Git, GitHub, and foundational environment setup**. The goal is to build a robust, reproducible, and well-versioned codebase ready for advanced tasks.

-----

### 🎯 Task 1 Objectives

| Area | Description | Deliverables |
| :--- | :--- | :--- |
| **Setup** | Set up a functional and reproducible Python development environment. | `requirements.txt`, documented setup process. |
| **Version Control** | Implement proper Git practices, including branching and descriptive commits. | `task-1` branch, regular commits ($\ge 3$/day). |
| **Automation** | Configure a basic Continuous Integration (CI) pipeline using GitHub Actions. | `.github/workflows/unittests.yml`. |
| **Analysis** | Perform comprehensive Exploratory Data Analysis (EDA) on the provided dataset. | Analysis presented in the `notebooks/` directory. |

-----

### 📁 Repository Structure

The project adheres to a standard, modular structure to separate configuration, source code, and analysis notebooks.

```
.
├── .github/                   # CI/CD Workflow configuration
├── .vscode/                   # Editor-specific settings
├── .gitignore                 # Files to ignore
├── requirements.txt           # Python dependency list
├── README.md                  # This file
├── src/                       # Core Python source code (e.g., reusable functions)
├── notebooks/                 # Exploratory Data Analysis (EDA) and prototyping
├── tests/                     # Unit tests for the src/ directory
└── scripts/                   # Utility scripts (e.g., data downloading, setup)
```

-----

### 🧪 Required Exploratory Data Analysis (EDA)

The following areas must be explored and documented within the `notebooks/` directory:

#### 1\. Descriptive Statistics

  * Calculate basic metrics for **textual lengths** (e.g., headline length distribution).
  * **Publisher Activity:** Count articles per publisher to identify major contributors.
  * **Date Trends:** Analyze publication dates to identify high-frequency periods.

#### 2\. Text Analysis (Topic Modeling)

  * Use NLP techniques to extract **common keywords, phrases, or topics** (e.g., "FDA approval," "price target") that characterize the news articles.

#### 3\. Time Series Analysis

  * Investigate the **publication frequency over time** to spot spikes correlating with market events.
  * Analyze the **time of day** when news is released, crucial for trading systems.

#### 4\. Publisher Analysis

  * Identify the **top contributing publishers**.
  * Examine the **difference in the type of news** reported by various publishers.
  * For email-based publisher names, identify **unique organizational domains**.

-----

### 🛠️ Development & Version Control Guidelines

  * **Branching:** All development work must be conducted on the **`task-1`** branch.
  * **Commits:** Commit frequently (at least **three times a day**) with clear and descriptive commit messages explaining *what* was done and *why*.
  * **CI/CD:** The `.github/workflows/unittests.yml` file is set up to automatically run tests and checks upon push, ensuring code quality is maintained.
