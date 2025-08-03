# AI-Powered Marketing Brochure Generator

Welcome to the **AI-Powered Marketing Brochure Generator** — a tool that automatically creates well-structured marketing brochures by intelligently scraping company websites and summarizing content using OpenAI's GPT-4.

Whether you're showcasing a company to investors, introducing it to potential hires, or compiling research, this tool helps automate the process using the power of AI.

## What It Does

- Scrapes a company’s website (landing page + relevant subpages)
- Identifies key pages (About, Careers, etc.)
- Extracts and cleans content using BeautifulSoup
- Summarizes using OpenAI GPT-4 API
- Outputs a clean, markdown-formatted brochure
- Supports live streaming of the response in Jupyter/IPython

## Example Use Case

Imagine you want a quick summary of a company like Hugging Face for a pitch deck or student research. Instead of browsing multiple pages, this tool fetches and summarizes everything in seconds.

## Tech Stack

- **Python 3.10+**
- [OpenAI API (GPT-4)](https://platform.openai.com/)
- `requests` – HTTP requests
- `beautifulsoup4` – Web scraping
- `python-dotenv` – Manage your API key securely
- `IPython.display` – Streamed markdown output

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/ujjesha1312/AI-powered-Marketing-Brochure-with-OpenAI.git
cd AI-powered-Marketing-Brochure-with-OpenAI
2. (Optional) Create a Virtual Environment
bash
Copy
Edit
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Add Your OpenAI API Key
Create a .env file in the root directory:

ini
Copy
Edit
OPENAI_API_KEY=sk-proj-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
Replace with your actual key from OpenAI dashboard

🛠 How It Works (Under the Hood)
Scrape – The tool extracts visible text from a company’s homepage and its relevant links (e.g., About, Careers).

Analyze – GPT-4 is used to select only brochure-relevant links.

Summarize – Content from those pages is summarized into human-readable markdown.

Display – Results are printed or streamed live using Markdown for clean visualization.

Project Structure
bash
Copy
Edit
AI-powered-Marketing-Brochure/
│
├── brochure_generator.py      # Main script
├── requirements.txt           # Python dependencies
├── .env                       # API key file (not committed)
└── README.md                  # Project documentation

Sample Output:
file:///C:/Users/ujjes/Downloads/Hugging_Face_Brochure.pdf

Future Enhancements
Export brochure as PDF

Add CLI interface

Support multilingual output

Option to scrape deeper levels of content

Disclaimer
This tool is for educational and demonstration purposes. Always verify the accuracy of summaries before using them for professional or business use.

Acknowledgements
OpenAI – for the GPT models

BeautifulSoup – for scraping made easy

Hugging Face – used as a sample test case

