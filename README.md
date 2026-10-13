# Vendor Agreement Flagging Prototype for Legal Operations Support

## Project Overview

The Vendor Agreement Flagging Prototype is a Python-based document analysis tool designed to support legal operations by identifying potentially important clauses, keywords, and risk-related terms in vendor agreements. It processes PDF and Word documents and uses rule-based text matching to flag relevant sections for further review.

The prototype aims to simplify preliminary contract screening, reduce manual document review effort, and help legal operations teams identify areas that may require closer attention.

## Objectives

- Automate preliminary screening of vendor agreements.
- Identify predefined keywords and potentially risky terms.
- Extract text from PDF and Word documents.
- Flag relevant sections for further legal review.
- Improve the efficiency of document analysis workflows.

## Key Features

- **Document Processing:** Extracts text from PDF and DOCX files.
- **Keyword-Based Flagging:** Uses regular expressions to identify predefined terms and phrases.
- **Risk Identification:** Highlights text that matches configured risk-related patterns.
- **Interactive Interface:** Provides a Streamlit interface for document analysis.
- **Review Support:** Helps users locate flagged content for further investigation.

## Technologies Used

- **Python** — Core programming language.
- **Streamlit** — Interactive web interface.
- **Regex (`re`)** — Keyword and pattern matching.
- **pdfplumber** — PDF text extraction.
- **python-docx** — Word document text extraction.

## Project Workflow

1. Upload a vendor agreement in PDF or DOCX format.
2. Extract text from the uploaded document.
3. Process the extracted text using predefined keywords and regular expressions.
4. Identify and flag matching clauses or terms.
5. Review the flagged content for further investigation.

## Installation and Setup

### Prerequisites

- Python 3.10 or later
- pip package manager

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <YOUR_REPOSITORY_FOLDER>
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows**
```bash
venv\Scripts\activate
```

**macOS/Linux**
```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install streamlit pdfplumber python-docx
```

### 4. Run the Application

```bash
streamlit run app.py
```

Replace `app.py` with the actual Python filename if your entry-point file has a different name.

## Suggested Project Structure

```text
vendor-agreement-flagging/
├── app.py
├── requirements.txt
├── README.md
├── sample_documents/
└── .gitignore
```

The structure above is a suggested layout. Adjust it to match your actual repository files.

## Example Use Cases

- Preliminary review of vendor agreements.
- Identification of predefined contractual terms.
- Locating clauses that may require legal attention.
- Supporting vendor contract review workflows.

## Limitations

- Flagging depends on predefined keywords and regular-expression patterns.
- The prototype may miss risks expressed in unfamiliar language or context.
- A flagged term does not necessarily indicate a contractual violation.
- The system does not replace qualified legal review or provide legal advice.

## Future Enhancements

- Add configurable risk categories and severity levels.
- Support additional document formats.
- Improve clause classification using NLP or machine learning.
- Generate downloadable reports of flagged clauses.
- Add document comparison and clause-level explanations.

## Disclaimer

This project is intended for educational and preliminary document-review support. All flagged clauses should be reviewed by a qualified legal professional before any legal or business decision is made. Do not upload confidential vendor agreements to an unapproved environment.

## Author

**N Aishwarya**

Developed as part of the First Quadrant Labs OJT project experience.
