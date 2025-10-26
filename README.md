# Resume RAG Parser

A simple tool that converts resume files (PDF/DOCX) into structured JSON using LangChain and OpenAI.

## What It Does

Parses resumes and extracts:
- Contact information and links
- Education and qualifications
- Work experience
- Projects and tech stacks
- Skills (languages, frameworks, tools)
- Extracurricular activities

## Tech Stack

- LangChain for RAG pipeline
- OpenAI GPT-4o-mini
- FAISS vector store
- Pydantic for validation
- pdfplumber & python-docx

## Setup

```bash
git clone https://github.com/Aneeba-Waseem/Resume-Parser/.git
cd Resume-Parser
pip install -r requirements.txt
```

Set your OpenAI API key:
```bash
export OPENAI_API_KEY="your_api_key_here"
```

## Usage

Open and run the Jupyter notebook:
```bash
jupyter notebook ResumeParsing.ipynb
```

Update the file path in the notebook to point to your resume, then run all cells.

## Example Output

```json
{
  "name": "John Doe",
  "contact_info": {
    "phone": "123456789",
    "email": "example@gmail.com"
  },
  "qualification": "Bachelors of Software Engineering",
  "university": "Stanford University",
  "experience": [...],
  "projects": [...],
  "skills_summary": {
    "languages": ["C", "C++", "Python"],
    "frameworks_libraries": ["ASP.NET Core", "Bootstrap CSS"],
    "tools_platforms": ["Git", "MySQL", "Azure"]
  }
}
```

**Aneeba Waseem** 

📅 2025

🎓 Project: Resume Parsing
