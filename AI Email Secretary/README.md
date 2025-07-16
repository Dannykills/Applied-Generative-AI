# AI Email Secretary

This project uses OpenAI's language models to transform meeting notes into professional email drafts.

## 📂 Project Structure

- `AI_Email_Secretary.ipynb` — The main notebook that processes notes and generates emails.
- `Alex_emails_march_04.csv` — A dataset of sample meeting notes.
- `config_template.json` — A config file where you can add your OpenAI API key (do not share sensitive keys publicly).

## 💡 Features

- Summarizes long meeting notes into short, professional summaries.
- Drafts email content using generative AI.
- Accepts structured and unstructured input text.

## 🛠 Requirements

- Python 3.x
- `openai` Python package
- Jupyter Notebook

Install dependencies:
```bash
pip install openai
```

## 🔒 API Config

Use the `config_template.json` file to insert your own OpenAI API credentials. Replace the placeholder string with your actual key (do **not** share the real key in public repos).

```json
{
  "API_KEY": "your-api-key-here",
  "OPENAI_API_BASE": "https://api.openai.com/v1"
}
```

## 🚀 How to Run

1. Open the Jupyter Notebook.
2. Load your meeting notes or use the provided dataset.
3. Run the cells to generate email drafts.
