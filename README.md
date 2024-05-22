# Kleinanzeigen-2024-Stealth-Parser #

# Description
Kleinanzeigen 2024 Stealth Parser  is a Python-based project designed to scrape and collect links of any desired objects from the Kleinanzeigen website. This tool utilizes Selenium for web scraping, supports the use of custom user-agents and proxies to avoid detection, and logs all activities for better traceability and debugging.

# Features
- Simplicity:                          Easy to configure and run.
- Undetectability:                     Uses --disable-blink-features=AutomationControlled to prevent detection by websites.
- Custom User-Agent and Proxy Support: Allows specifying user-agents and proxies for increased anonymity.
- Logging:                             Comprehensive logging with loguru for both console and file output.
- Error Handling:                      Robust error handling ensures the script continues running and logs any issues.

# Installation
To use this tool, you need to have Python installed along with the necessary libraries. Follow the steps below to set it up:
1. Clone the repository: 
"git clone https://github.com/dmytro-skyrta/Kleinanzeigen-2024-Stealth-Parser.git"
"cd Kleinanzeigen-2024-Stealth-Parser"
2. Install the required Python packages: 
pip install -r requirements.txt
3. Ensure you have the Chrome browser installed and download the corresponding ChromeDriver.
4. Place the chromedriver executable in your system's PATH or in the project directory.

# Usage
1. Run the script: python main_script.py
2. Enter the URL from the Kleinanzeigen website you want to scrape when prompted. You can provide any URL for any type of item you are searching for.
3. The script will start the Chrome browser, navigate to the specified URL, and collect all relevant links.
4. The collected links will be saved in the file "Links of founded objekts.txt".

# Configuration
You can customize the user-agent and proxies by modifying the get_from_kleinanzeigen_with_chromedriver function:

useragent = "your-user-agent"
working_proxies_list = ["proxy1", "proxy2", "proxy3"]
Logging

# Logs are saved in two places:
Console output
File: Log.txt (rotated at 10 MB and compressed)

# Credits
# Thanks for the advice on developing this project to:
Yevhen Vlasenko

# Inspired by ideas from:
Python Today
Erik Spichak

# License
This project is licensed under the MIT License - see the LICENSE file for details.

Feel free to contribute to the project by submitting issues or pull requests. Your feedback is highly appreciated!
