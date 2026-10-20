SAP-Standardizer
Helps standardize mass records in compliance with SAP policies (Philippines), reducing processing time.

What it does
Standardizes company names (removes special characters, fixes suffixes such as INC and CORP)
Splits individual names into salutation, first name, last name
Cleans Philippine phone numbers and reports whether each is valid
Exports results as CSV
Privacy notice
This is a public demo. Do not paste confidential or personal data. Use sample data only.

Run locally
Install Python 3.[VERSION]+
In a terminal inside the project folder:
```bash
python -m venv .venv
.venv\Scripts\activate # Windows
pip install -r requirements.txt
streamlit run app.py
```

Example
Input	                    Output

Company! Incorporated     Company Inc.

+639512124311             0951 212 4311

Jane Dela Cruz            First Name - Jane Last Name - Dela Cruz

Known limitations
Salutations are guessed from first names and can be wrong.
Foreign contact number cannot be standardized.
Tech stack

Python, Streamlit, pandas, nameparser, gender-guesser

Author
Joshua Layug - https://www.linkedin.com/in/joshua-layug-2406292b2/
