# Contributing to the Project
This guide outlines the technical standards and coding requirements for developers looking to modify or extend the Contributor Management and Issue Tracking System.

# Technical Requirements
Environment: Development must be conducted in Google Colab or a standard Python 3.12.12 environment.
Input Handling: All data for projects, contributors, and issues must be gathered using the input() function to ensure dynamic data collection.
Program Flow: The script must be written as a single, continuous program where data from early sections is passed to later ones.

# Project Architecture & Core Logic
To contribute effectively, please understand the following implementation details:

# Code Standards & Constraints
1. Data Integrity & Immutability
Official Info: The project variable must be a Tuple to store name, version, and lead information.
2. Collection Management
Dictionaries: Every contributor and issue record must be stored as a dictionary.
Set Operations: Developers must use Set methods (add, union, intersection, difference, discard) to analyze unique technology stacks and reporter data.
3. File System & Reporting
Error Handling: File operations must be wrapped in try/except blocks, specifically catching IOError for writing and FileNotFoundError for reading.
Formatting: All final summary outputs and file writes must utilize f-strings; string concatenation using the + operator is prohibited in these sections.

# Contribution Policy
Individual Effort: This project follows a strict individual code policy.
Originality: While conceptual discussions are allowed, all logic and code implementation must be your own.
