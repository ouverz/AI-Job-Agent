# 🤖 AI Job Application Agent

Stop sending the same cover letter to every application. This agent reads your CV, understands a job description, and generates a tailored cover letter — one that speaks directly to what the role is asking for, emphasising your work experience over education.

Built with **LangChain**, **Anthropic Claude 3**, and **ChromaDB**.

---

## How it works

1. Your PDF resume is parsed and indexed into a ChromaDB vector store
2. Vector similarity matching identifies which parts of your experience are most relevant to the job description
3. Claude 3 generates a tailored cover letter grounded in that matched content — prioritising work experience over education or internships

The result is a first draft that's genuinely personalised, not just a template with your name swapped in.

---

## 🛠️ Stack

| Component | Technology |
|---|---|
| LLM | Anthropic Claude 3 |
| Orchestration | LangChain |
| Vector Store | ChromaDB |
| PDF Parsing | PyPDF |
| Language | Python |

---

## ✨ Features

- 📄 Parse PDF resumes into searchable vector knowledge
- 🧠 Vector similarity matching between resume content and job description
- ✍️ Tailored cover letter generation — emphasises work experience over education
- ✅ Input validation and error handling
- 💬 Simple prompt interface

---

## 📦 Setup

```bash
# Clone the repo
git clone https://github.com/ouverz/AI-Job-Agent.git
cd AI-Job-Agent

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp .env.example .env
# Add your Anthropic API key to .env

# Add your resume
mkdir data
# Place your resume.pdf in the data/ folder

# Run
python cover_letter.py
```

---

## 💡 Usage

When prompted, paste in the job description you're applying for. The agent will match it against your resume and output a tailored cover letter.

---

## 🗺️ Roadmap

- Support for multiple output formats (PDF, DOCX)
- Multi-provider LLM support (OpenAI, Gemini)
- Batch processing for multiple job descriptions
- Web UI

---

## 📄 License

MIT License — see LICENSE file for details.

---

Built by [Ofer Kulka](https://www.oferkulka.com) — Senior Data & AI Engineer, Frankfurt.  
[LinkedIn](https://linkedin.com/in/oferkulka) · [GitHub](https://github.com/ouverz)
