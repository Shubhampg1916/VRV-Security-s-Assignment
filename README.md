# VRV-Security-s-Assignment
Log Analysis Script
**This Python script processes a log file (sample.log), analyzes it for:**
      IP Request Counts: Tracks how many requests each IP address made.
      Most Accessed Endpoint: Identifies the most frequently accessed resource (e.g., /login, /home).
      Suspicious Activity: Detects IPs with too many failed login attempts.
The results are displayed in the terminal and saved into a CSV file (log_analysis_results.csv).
# Features
IP Request Count: Counts requests made by each IP address.
Most Accessed Endpoint: Finds the most visited endpoint in the log.
Suspicious Activity: Flags IPs with failed login attempts exceeding a set threshold.
# How to Use
1. Prepare the Files
    Place a sample.log file in the project directory (contains server logs).
    (Optional) Create a config.json file to customize settings:
    json
    Copy code
    {
        "FAILED_LOGIN_THRESHOLD": 5,
        "LOG_FILE": "sample.log",
        "OUTPUT_CSV": "log_analysis_results.csv"
    }
2. Default Configurations
    If config.json is missing, the script uses these default settings:
3. Running the Script
  Run the script in your terminal:
  python script.py
# Results
The script outputs:
**In the Terminal:**
  Request counts per IP address.
  The most frequently accessed endpoint.
  IPs with suspicious failed login activity.
**In a CSV File:** Results are saved to log_analysis_results.csv, including:

Requests per IP: IP addresses and their request counts.
Most Accessed Endpoint: The endpoint and how many times it was accessed.
Suspicious Activity: IPs with failed login attempts exceeding the threshold.
