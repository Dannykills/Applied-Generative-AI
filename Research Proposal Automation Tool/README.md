# 🧠 AI NIH Proposal Assistant

This tool uses large language models (LLMs) to help researchers align their past work with new NIH funding opportunities (NOFOs). It reads the NOFO, scans a publication archive, suggests aligned research directions, and drafts proposal sections — like having a smart research co-pilot during grant season.

## 📁 What’s in This Folder

- `NOFO_Proposal_Assistant.ipynb` — Main notebook that runs the assistant workflow.
- `sample_NOFO.pdf` — A sample Notice of Funding Opportunity from the National Institute of Mental Health.
- `ian_publications.txt` — Example text from Dr. Ian McCulloh’s past research portfolio.
- `config_template.json` — A blank config file where you can enter your OpenAI API key and settings.

## 💡 What It Actually Does

- Loads a NOFO document and a body of past research (PDF or plain text).
- Uses embeddings and semantic search to match past work with NOFO priorities.
- Suggests possible research directions aligned with the funding call.
- Drafts key NIH proposal sections like Significance, Innovation, and Approach.
- Can cite relevant prior work to justify the proposal’s foundation.

## 🛠 Requirements

- Python 3.x  
- `openai`, `langchain`, `faiss-cpu`, `PyMuPDF` or `pdfminer.six`

Install dependencies:
```bash
pip install openai langchain faiss-cpu pymupdf

## 🔒 API Config

Use the `config_template.json` file to insert your own OpenAI API credentials. Replace the placeholder string with your actual key (do **not** share the real key in public repos).

```json
{
  "API_KEY": "your-api-key-here",
  "OPENAI_API_BASE": "https://api.openai.com/v1"
}
```

## 🚀 How to Run

1. Open the notebook in Jupyter or Google Colab.
2. Fill out your config_template.json file with valid credentials.
3. Upload a NOFO PDF and your past work (or use the samples provided).
4. Run each cell — the assistant will analyze the NOFO, match it to your archive, and generate proposal drafts.
5. Review, refine, and submit high-quality grant text with less stress.