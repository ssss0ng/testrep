# Technical Documentation: Functionality and Logic
This document explains the functional logic and built-in Python methods implemented to handle data processing and file management.  

# Contributor and Issue Management
list.append(): Adds newly created dictionaries (contributors/issues) into their respective master lists.  
list.sort(): Orders the names list alphabetically to ensure a professional and organized display in the final report.  
Dictionary Methods:  
  get(): Safely retrieves values from contributor records.  
  update(): Used to modify or add new keys (like status: 'Active') to the contributor dictionaries.  
  keys(), values(), items(): Essential for iterating through issue data to extract priorities and reporters.  

# File I/O and System Operations
os.makedirs() & os.path.join(): Manages directory creation and handles file paths safely across different operating systems.  
open() with Modes:  
  'w' (Write): Creates and overwrites the initial project_report.txt and issues.csv.  
  'a' (Append): Adds the "Urgent Issues" section to the end of the report without deleting existing content.  
File Reading:  
read() / readline(): Used for basic file verification.  
readlines(): Specifically used with negative slicing ([-6:]) to read and display the last 6 lines of the report.  

# contributors
The central collection for all registered members of the project.  
Structure: A list of dictionary objects, where each dictionary represents a contributor with keys for name, role, language, commits, and country.  
Role: It acts as the master database for technical staff. It is populated dynamically via input() and serves as the source for generating tech stack summaries and name lists.  
Constraint: The status for all entries in this list is managed as 'Active' by default to simplify tracking.

# names
A secondary list derived from the primary repository to facilitate organized reporting.  
Structure: A flat list of strings containing only the names of the contributors.  
Role:  
  Created by extracting values from the contributors list.  
  Uses the .sort() method to arrange participants alphabetically for the final report.  
  Enables the use of negative indexing and slicing to display specific segments of the team (e.g., the last registered member).  

# issues
A comprehensive list used to monitor the health and progress of the software project.  
Structure: A list of dictionaries, each containing details such as ID, title, type, priority, reporter, and status.  
Role:  
  Functions as the primary target for data analysis loops.  
  Used to calculate the number of 'Open' issues manually without relying on built-in search methods.  
  Provides the raw data for calculating the "Top Reporter" through frequency mapping.  

# urgent
A specialized list designed for immediate management action, created through advanced filtering logic.  
Structure: A list of strings containing only the titles of high-priority problems.  
Role: It isolates high-risk items from the general issues list, allowing them to be appended to the final section of the project_report.txt file for maximum visibility.  

# reporters
A collection focused on identifying the individuals contributing to the issue tracking process.  
Structure: A list of names extracted from the reporter field of each issue.  
Role:  
  Used in conjunction with Sets to determine the total number of unique individuals who have filed reports.  
  Serves as the basis for set operations (union/intersection) to compare project members against active reporters.  
