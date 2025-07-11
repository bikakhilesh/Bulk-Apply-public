📈 MeroShare IPO Bulk Application Automation

This Python script automates the process of applying for IPOs (Initial Public Offerings) through the MeroShare portal for multiple accounts using data from an Excel file.

🔍 Features

Reads account data (CRN, PIN, Demat ID, password, bank, and name) from an Excel sheet.

Logs into each MeroShare account using API requests.

Fetches the list of currently available IPOs.

Applies for selected IPOs for each account.

Outputs and saves the results of each application attempt to an Excel file.

📁 Input Format

An Excel file named accounts.xlsx with the following columns is expected:

crn

pin

demat_id

password

Bank

Name

Each row corresponds to a separate user account.

⚙️ How It Works

Load Account Data: Reads the accounts.xlsx file using pandas.

Class-Based MeroShare Automation: A MeroShare class handles:

Authentication

IPO listing

IPO application

Batch IPO Application: Using a loop, it logs into each account and applies for the user-specified IPO.

Result Logging: Saves the result of the application attempt (success or failure) in a new Excel file.

🚀 How to Run

Install Dependencies:

pip install pandas openpyxl tenacity

**Prepare **``: Populate the required fields for each account.

Run the Script:

python Bulk_apply_.ipynb

You’ll be prompted to input:

The IPO script code (e.g., "NRIC")

Quantity to apply

View Results: A file like share_application_results_NRIC.xlsx will be saved with the application status.

🧠 Note

The script uses a reverse-engineered approach to simulate browser requests to MeroShare.

Use responsibly and ensure you comply with MeroShare’s terms of service.

Application failures may be due to incorrect credentials, invalid CRN or PIN, or closed IPOs.

📌 Disclaimer

This tool is intended for educational purposes. Use it at your own risk. The author is not responsible for any misuse or violation of platform terms.
