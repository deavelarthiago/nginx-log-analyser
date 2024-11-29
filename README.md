##################################################################################################

Nginx Log Analyser

##################################################################################################

Purpose: This is a simple and efficient shell script designed to analyze Nginx access log files and extract useful insights from them. The script was created as a project for `Roadmaps.sh`.
(https://roadmap.sh/projects/nginx-log-analyser)

The script uses standard Unix tools like `awk`, `sort`, and `uniq` to process the log file and display the following information:

1. Top 5 IP addresses with the most requests;
2. Top 5 most requested paths;
3. Top 5 response status codes;
4. Top 5 user agents.

This script is lightweight, easy to use, and ideal for quickly analyzing log files from the command line. 

## Prerequisites ##

- A Unix/Linux-based system with Bash shell.
- Standard command-line tools: awk, sort, uniq, and head.
- An Nginx access log file to analyze.
   In this case, the log file `access.log` was provided at this link:
   (https://gist.githubusercontent.com/kamranahmedse/e66c3b9ea89a1a030d3b739eeeef22d0/raw/77fb3ac837a73c4f0206e78a236d885590b7ae35/nginx-access.log)

## Usage ##

1. Clone or download this repository and make the script executable:
   ```bash 
   chmod +x analyze_logs.sh

3. Run the script, passing the Nginx log file as an argument:
   ```bash
   ./analyze_logs.sh <log_file>

5. Replace <log_file> with the path to your Nginx access log file (e.g., access.log).
Example command:
   ```bash
   ./analyze_logs.sh access.log

7. View the output in your terminal, which includes:
- Top 5 IP addresses;
- Top 5 requested paths;
- Top 5 response status codes;
- Top 5 user agents.

## Notes ## 

- The script assumes that the log file follows the standard Nginx access log format. If the log format differs, adjustments to the awk commands may be required.
- Ensure the log file is accessible and readable by the user running the script.

## Limitations ##

- The script is designed for basic log analysis and may not handle extremely large log files efficiently. For processing large logs, consider using tools like grep or specialized log analysis software.
- It does not validate the format of the input log file.

## Contribution ##

Fork the project.

1. Create a branch for your feature:
   ```bash
   git checkout -b `my-feature`

2. Make your changes and commit:
   ```bash
   git commit -m "Added feature X"

3. Push your changes:
   ```bash
   git push origin my-feature

Open a Pull Request.
