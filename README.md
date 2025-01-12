Project: Using Gobuster for Directory and File Enumeration on a Website

Description:

The project involved using the Gobuster tool to perform a directory and file enumeration attack on a website, with the goal of identifying hidden directories and files, as well as checking for potential vulnerabilities in the web application's structure. The process consisted of several stages:

Project Objective:
The main task was to determine the directory and file structure of the target website using the Gobuster tool. This helps in identifying potential vulnerabilities such as unsecured files and directories that could be exploited by attackers for further actions.

Tool Used:
Gobuster is a command-line tool for performing directory and file enumeration on websites using wordlists. This tool can be used to find hidden URLs, subdomains, directories, and files through various methods (e.g., HTTP GET method).

Execution Process:

Directory Scanning: Using Gobuster in dir mode, a directory enumeration scan was set up for the target site. The directory-list-2.3-medium.txt wordlist was selected for this process.
Error Handling: During execution, errors were managed, and unwanted status codes (such as 405) were excluded to avoid blocking the scanning process.
File Extensions: The project also configured Gobuster to enumerate files with .php and .js extensions, checking for hidden scripts or vulnerable pages.
Performance Management: To speed up the process and prevent request blocking, the number of threads was reduced using the -t flag.
Problems Solved:

Issues with domain resolution and /etc/hosts configuration were resolved. The correct mapping of the www.offensivetools.thm domain to the local IP allowed successful connection to the target website.
The exclusion of status code 405, which could block the scanning process, allowed for uninterrupted directory analysis.
Results:

After configuring the tool and resolving network issues, the scanning was successfully completed, revealing hidden directories and files that could be of interest for further security testing.
This approach is an essential part of web application security audits, helping to identify potential weak points in a site's structure.
Conclusion:
The project demonstrated the use of a tool for testing the security of websites, focusing on identifying hidden directories and files. This approach is a critical element in security analysis, helping to uncover vulnerabilities that could be exploited in web application attacks.
