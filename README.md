🤖 AI-Powered Email Enrichment Tool

A smart Streamlit-based AI application that enriches email or communication datasets by automatically extracting:

🏢 Company name

🏭 Business sector

⏰ Deadlines with urgency status

🚨 Attention requirements

This app integrates Ollama (local LLMs like Llama 3, Mistral, or Gemma) to analyze text data intelligently and outputs structured, enriched insights with downloadable Excel reports.

🌟 Features

📤 Upload CSV or Excel files with email or text data

🧠 AI-based data enrichment using Ollama language models

🗓️ Deadline parsing & urgency color-coding

🔴 Urgent (< 3 days)

🟡 Soon (< 7 days)

🟢 Future (> 7 days)

⚫ Overdue

⚪ No deadline

🚨 Detects emails that need attention (e.g., “urgent”, “asap”, “reply needed”)

📊 Dashboard summaries & visual analytics (metrics + bar charts)

📥 Export enriched results as Excel files

🧩 Tech Stack
Component	Description
Python	Core programming language
Streamlit	Frontend framework for web app
Pandas	Data processing and analysis
Ollama	Local LLM inference engine
xlsxwriter	Excel export
Matplotlib (via Streamlit)	Data visualization
🚀 Installation
1️⃣ Clone the Repository
git clone https://github.com/<your-username>/email-enrichment-tool.git
cd email-enrichment-tool

2️⃣ Install Dependencies

Make sure you have Python 3.9+ installed, then run:

pip install -r requirements.txt


If you don’t have a requirements.txt, create one with:

streamlit
pandas
ollama
xlsxwriter

3️⃣ Install & Run Ollama

Download and install Ollama from https://ollama.com
.

Pull a model (for example, Llama 3):

ollama pull llama3:8b


You can also try other compatible models:

ollama pull mistral
ollama pull gemma:7b

🧠 Running the App

Start the Streamlit app:

streamlit run app4.py


Then open your browser at:
👉 http://localhost:8501

🖥️ How It Works

Upload your CSV/XLSX file containing email or communication data.

Select which columns provide relevant context for AI analysis.

Click "✨ Enrich Data" to process all rows using your selected Ollama model.

The app:

Extracts company name, sector, and deadlines.

Classifies emails based on urgency or required attention.

Displays metrics and charts summarizing insights.

Download the enriched dataset as an Excel file.

📊 Example Output
company_name	sector	deadline	deadline_status	attention_required
LinkedIn	Technology	2024-12-15	Future (45 days) 🟢	Yes
NVIDIA	Technology	No deadline	⚪ No Deadline	No
Bank of America	Finance	01/15/2025	Future (78 days) 🟢	Yes
⚙️ Configuration

In the sidebar, you can:

Select the LLM model from your local Ollama installation

View legend for deadline color codes

Check the app’s about info

🧾 Example Use Cases

✅ Analyzing incoming business emails
✅ Filtering emails that need urgent response
✅ Organizing tasks based on deadlines
✅ Extracting structured metadata from communication logs

🧰 Future Improvements

Integration with LangChain for advanced contextual parsing

Support for email attachments

Enhanced deadline recognition for relative dates (e.g., “next Friday”)

Multi-model comparison option

📜 License

This project is licensed under the MIT License.
Feel free to use, modify, and share with attribution.
