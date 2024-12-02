# UiPath Invoice Processing Automation

This repository showcases a UiPath project designed to automate invoice processing using the Document Understanding model. Below is an overview of how the solution operates:

### 1️⃣ Email Integration
- The bot reads new emails with a specific subject line.
- Downloads the invoice attachment and saves it to a designated local folder for processing.

### 2️⃣ Document Understanding Workflow
- **Taxonomy Definition**: Structures the data extraction process, including key fields like invoice details (e.g., number, date, total) and an orders table.
- **Digitization**: Leverages OCR to convert the invoice into a machine-readable format.
- **Classification**: Ensures the document type matches the invoice category.
- **Data Extraction**: Handles unstructured data challenges within the orders table, including cells spanning multiple rows and columns, by employing:
  - Regex Extractor
  - Form Extractor

### 3️⃣ Data Storage
- Extracted data is consolidated and saved into an Excel file for easy access and further use.

### 4️⃣ Automated Email Response
- The bot replies to the original email, attaching the processed Excel sheet containing the extracted details.

## Challenges
One of the most significant hurdles was accurately extracting data from the unstructured orders table. By combining multiple extractors, the bot achieved a high level of accuracy and reliability in data capture.


Feel free to explore, suggest improvements, or share similar projects! Contributions are welcome.
