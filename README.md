# Contributor Management and Issue Tracking System
This Python-based application serves as a command-line tool for managing open-source project data, including contributor details and issue tracking. The system is designed to run as a single, continuous program where data from early stages flows into subsequent analysis and reporting phases.

# Core Features
Project Initialization: Stores official project metadata (name, version, lead) in immutable structures.
Contributor Management: Registers contributors with details such as roles, languages, and commit counts using dictionaries.
Issue Tracking: Collects and categorizes project issues by priority (Critical, High, Medium, Low) and status.
Data Analysis:
-Calculates "Open" issue counts without built-in counting methods.
-Identifies the top reporter through custom logic.
-Maps tech stacks and reporter sets using set operations (union, intersection, difference).
File Reporting: Generates a structured project folder containing a full text report and a CSV summary of all tracked issues.

#Setup and Usage
1. Environment: Run the script in Google Colab (recommended) or any local Python environment like VS Code or PyCharm.
2. Execution: Run the oss_task5.ipynb or .py file from top to bottom.
3. Input: The program will prompt for exactly 4 contributors and 5 issues via the console.
4. Output:A welcome banner and data summary will print to the console.A local folder (e.g., open_track/) will be created containing project_report.txt and issues.csv.
