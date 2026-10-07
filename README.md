# Cleaning Financial Data with PySpark

This project is focused entirely on the most critical step of any data workflow: cleaning up messy, real-world data so it is actually reliable enough to use. 

I built this specifically as a hands-on practice project to build my familiarity with **PySpark**, a framework designed to process massive datasets that are simply too large for standard tools like Excel or Pandas to handle. By using a heavy financial dataset from LendingClub (containing over 2.2 million records), I wanted to tackle the practical challenges that must be solved before any dashboards or reports can be built.

## What This Project Does

Raw data is rarely perfect. This notebook walks through the step-by-step process of organizing and rescuing the data. Key steps include:

* **Handling Missing Information:** Deciding what to do when data is blank. Instead of just blindly deleting every row with a missing value, I looked at the context to figure out if a blank space was a harmless error or a critically broken record that needed to be dropped.
* **Fixing Dates:** Converting messy, text-based dates (like "Jan-2015") into a standardized calendar format that systems can properly understand, sort, and analyze.
* **General Housekeeping:** Filtering out bad rows, removing duplicates, and ensuring the remaining information makes logical sense.

## Why PySpark?

I chose PySpark because it is the industry standard for big data engineering. While I could have used simpler tools for a smaller file, my goal was to learn how to write code that scales. The logic built in this project is designed so that it could easily handle 20 million or 200 million rows without crashing the system.

## Tools Used

* **Python & PySpark:** The core programming language and data engine used to process the files.
* **Jupyter Notebook:** To write, test, and document the code step-by-step.
* **Git & GitHub:** To track changes and ensure massive data files are safely excluded from the online repository using `.gitignore`.
