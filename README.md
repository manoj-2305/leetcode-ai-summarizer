# 🔍 LeetCode Problem Summarizer

A command-line tool that uses OpenAI's GPT API to automatically summarize LeetCode problems. It helps streamline technical interview prep by generating structured summaries that can be saved and reviewed later.

---

## 🧠 Features

- 📄 Auto-generates summaries of LeetCode problems using OpenAI.
- 🧾 Stores results in a structured CSV format.
- 🔁 Supports batch input for summarizing multiple problems at once.
- 📋 Maintains detailed logs of prompts and API responses.

---

## ⚙️ Setup Instructions

### 1. Prerequisites

- Python 3.7 or higher
- An OpenAI API key from [https://platform.openai.com](https://platform.openai.com)

### 2. Clone This Repository

```bash
git clone https://github.com/your-username/leetcode-summarizer.git
cd leetcode-summarizer
```

### 3. Install Dependencies

```bash
pip install pandas requests
```

### 4. Add Your OpenAI API Key

Set your key as an environment variable:

```bash
export OPENAI_API_KEY='your_api_key_here'  # macOS/Linux
# or
set OPENAI_API_KEY='your_api_key_here'     # Windows
```

---

## 🚀 Usage

1. Add LeetCode problems to `prompt_arguments.csv` under a column named `problem`.

2. Run the summarizer script:

```bash
python main.py
```

3. Summarized outputs will be stored in a CSV file. Logs will be written to the `logs/` folder.

---

## 📁 Project Structure

```text
leetcode-summarizer/
│
├── main.py                  # Core script
├── prompt_arguments.csv     # Input file with problems to summarize
├── logs/
│   ├── app.log              # Execution logs
│   └── prompts.log          # Prompt logs
└── README.md
```

---

## 🔧 Notes on OpenAI Integration

- Uses the `https://api.openai.com/v1/chat/completions` endpoint.
- Compatible with models like `gpt-3.5-turbo`.
- If you see error 429 or 404:
  - Check billing/account status.
  - Try using a VPN if facing regional access issues.
  - Ensure you're using the correct API key and endpoint.

---

## 🧰 Recommended Tools

- [Visual Studio Code](https://code.visualstudio.com/) for editing and debugging.
- Git and GitHub for version control.

---

## ✅ Use Cases

- Quickly summarize daily LeetCode problems.
- Build a personal problem-summary database.
- Practice prompt engineering with real-world coding tasks.

---

## 📣 Attribution

This project was developed independently for educational and internship purposes using Python and OpenAI’s API services.
