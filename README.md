Server Metrics SQL Parser & Analyzer
This project provides a Google Colab script to parse server performance metrics from SQL INSERT statements, analyze them, and visualize trends.
Features
SQL Parsing: Extracts data from INSERT INTO server_metrics statements.
Data Cleaning: Converts timestamps and numerical values into a structured Pandas DataFrame.
Statistical Summary: Generates descriptive statistics for CPU, memory, disk I/O, and network usage.
Visualization: Plots CPU usage per host using Matplotlib.
Anomaly Detection: Identifies entries where CPU usage exceeds 90%.
Requirements
Python 3
Pandas
Matplotlib
Google Colab (or Jupyter Notebook)
Usage
Upload your SQL file in Colab.
The script will:
Parse the file.
Create a DataFrame.
Display summaries and plots.
Print CPU usage anomalies.
View and analyze the output directly in the notebook.
Example
Example SQL line processed:
sql
Copy
Edit
INSERT INTO server_metrics (timestamp, host, cpu_usage, mem_usage, disk_io, net_in, net_out) 
VALUES ('2025-06-01 00:00:00', 'host01', 73.82, 3841.09, 391.34, 45.15, 7.69);
