# Contributor Management and Issue Tracking System
This Python-based application serves as a command-line tool for managing open-source project data, including contributor details and issue tracking. The system is designed to run as a single, continuous program where data from early stages flows into subsequent analysis and reporting phases.

# Environment
Python 3.x
OS: Windows / macOS / Linux
IDE: Jupyter Notebook, VS Code, or Google Colab
Libraries: Standard Python libraries (os, file I/O)

# Core Features
1. Project Initialization: Stores official project metadata (name, version, lead) in immutable structures.
2. Contributor Management: Registers contributors with details such as roles, languages, and commit counts using dictionaries.
3. Issue Tracking: Collects and categorizes project issues by priority (Critical, High, Medium, Low) and status.
4. Data Analysis:  
-Calculates "Open" issue counts without built-in counting methods.  
-Identifies the top reporter through custom logic.  
-Maps tech stacks and reporter sets using set operations (union, intersection, difference).  
5. File Reporting: Generates a structured project folder containing a full text report and a CSV summary of all tracked issues.

