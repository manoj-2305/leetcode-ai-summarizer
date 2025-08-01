3. Install Dependencies
bash
Copy
Edit
pip install pandas requests
4. Add Your OpenAI API Key
Set your key as an environment variable:

bash
Copy
Edit
export OPENAI_API_KEY='your_api_key_here'  # macOS/Linux
# or
set OPENAI_API_KEY='your_api_key_here'     # Windows
🚀 Usage
Add LeetCode problems to prompt_arguments.csv under a column named problem.

Run the summarizer script:

bash
Copy
Edit
python main.py
Summarized outputs will be stored in a CSV file. Logs will be written to the logs/ folder.

📁 Project Structure
text
Copy
Edit
leetcode-summarizer/
│
├── main.py                  # Core script
├── prompt_arguments.csv     # Input file with problems to summarize
├── logs/
│   ├── app.log              # Execution logs
│   └── prompts.log          # Prompt logs
└── README.md
🔧 Notes on OpenAI Integration
Uses the https://api.openai.com/v1/chat/completions endpoint.

Compatible with models like gpt-3.5-turbo.

If you see error 429 or 404:

Check billing/account status.

Try using a VPN if facing regional access issues.

Ensure you're using the correct API key and endpoint.

🧰 Recommended Tools
Visual Studio Code for editing and debugging.

Git and GitHub for version control.

✅ Use Cases
Quickly summarize daily LeetCode problems.

Build a personal problem-summary database.

Practice prompt engineering with real-world coding tasks.

📣 Attribution
This project was developed independently for educational and internship purposes using Python and OpenAI’s API services.

markdown
Copy
Edit

Let me know if you want a **badge section**, **screenshot preview**, or **contribution guidelines** 
