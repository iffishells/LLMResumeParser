# LLM Resume Parser Powerby OpenAI

This tool streamlines the extraction of key information from resumes in both PDF and Word formats, offering a convenient command-line interface (CLI) script as well as an intuitive Streamlit web application for easy interaction

The tool uses the OpenAI API, requiring an API key to function correctly. Be sure to keep your API key secure and adhere to OpenAI’s usage guidelines.

## Table of Contents
- [Installation](#installation)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
  - [Command Line Interface](#command-line-interface-cli)
  - [Streamlit Application](#streamlit-application)
- [Notes](#notes)

## Installation

Clone the repository and navigate into the project directory:

```bash
git clone <your-repo-url>
cd <your-repo-name>
```

## Requirements

The following Python packages are required:

- `openai`
- `streamlit`
- `PyMuPDF`
- `python-docx`

Install these dependencies using:

```bash
pip install -r requirements.txt
```

## Setup

1. **Get an OpenAI API Key**  
   Sign up on [OpenAI’s website](https://openai.com/) if you haven’t already, and retrieve your API key.

2. **Configure Environment Variables**  
   Create a `.env` file in the project root and add your OpenAI API key:
   
   ```plaintext
   OPENAI_API_KEY=your_openai_api_key_here
   ```

3. **Environment Setup**  
   Load environment variables by sourcing the `.env` file or using a package like `python-dotenv` (recommended if using a virtual environment).

## Usage

### Command Line Interface (CLI)

To run the tool from the command line, use the following command:

```bash
python cli_extractor.py --file <path-to-resume-file>
```

Replace `<path-to-resume-file>` with the path to the PDF or Word file you want to process.

### Streamlit Application

Run the Streamlit application for a web-based interface:

```bash
streamlit run app.py
```

Once launched, access the application through your browser (usually at `http://localhost:8501`).

## Notes

- **Secure API Key**  
  Ensure your API key remains secure by not sharing it in code repositories or public spaces.
  
- **OpenAI Usage**  
  Follow OpenAI’s guidelines for API usage to avoid any restrictions on your account.

## Troubleshooting

For issues or questions, please refer to the documentation or submit an issue on this repository.
