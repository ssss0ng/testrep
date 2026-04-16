# Data Structures
Project Metadata: Stored in an immutable Tuple (name, version, year started, main language, lead name) to ensure the integrity of official project info.  
Contributors: Managed as a list of dictionaries, where each dictionary tracks a name, role, language, commit count, and country.  
Issues: Tracked in a list of dictionaries including ID, title, type (Bug/Feature), priority, reporter, and status.  

# File Management and Reporting
The system automatically generates a structured directory named after the project to store persistence data:  
-project_report.txt: A comprehensive text report generated using f-strings, including contributor summaries and priority breakdowns.  
-issues.csv: A structured data file containing all tracked issues for external analysis.  
-Error Handling: All file operations are wrapped in try/except blocks to handle IOError or FileNotFoundError.  

# Issue Analysis Logic
Urgent Issues: The system uses list comprehension to instantly filter issues marked as 'Critical' or 'High'.  
Top Reporter: A custom loop identifies the contributor with the highest number of reported issues without relying on built-in functions like max().  
Tech Stack: Sets are utilized to perform union and intersection operations to find commonalities between contributors and project requirements.  
