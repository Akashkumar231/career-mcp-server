# 🚀 Career MCP Server

An AI-powered **Model Context Protocol (MCP) Server** built using Python that provides intelligent tools to assist developers in career growth, productivity, and code quality improvement.

This project exposes multiple tools such as job search, resume analysis, interview preparation, code review, and GitHub repository insights through the MCP interface, enabling seamless integration with AI clients like Cursor, Claude Desktop, or other MCP-compatible systems.

---

## 🧠 Features

The MCP server provides the following tools:

### 🔍 LinkedIn Job Fetcher
- Fetches latest job opportunities based on keywords and location
- Helps developers discover relevant job openings quickly

### 📄 Resume Analyzer
- Analyzes resume content
- Identifies strengths and missing skills
- Provides improvement suggestions

### 🎯 Interview Question Generator
- Generates role-based interview questions
- Supports different experience levels

### 🧑‍💻 Code Reviewer
- Reviews code snippets
- Detects issues and improvements
- Suggests best practices

### 📊 GitHub Repository Analyzer
- Analyzes public GitHub repositories
- Detects tech stack and complexity
- Provides optimization suggestions

---

## 🏗️ Architecture

AI Client (Cursor / Claude / MCP Client)
                │
                ▼
     MCP Protocol Interface
                │
                ▼
        Python MCP Server
                │
   ┌────────────┼────────────┐
   ▼            ▼            ▼
Job APIs  LLM Engine   GitHub API

## ⚙️ Tech Stack

- Python 3.10+
- MCP Python SDK
- OpenAI API (LLM integration)
- Requests / BeautifulSoup (Web scraping)
- PyGithub (GitHub API)
- Docker (Containerization)
- Virtual Environment (venv)

## 📁 Project Structure

career-mcp-server/
│
├── server.py
├── tools/
│ ├── linkedin_jobs.py
│ ├── resume_analyzer.py
│ ├── interview_generator.py
│ ├── code_reviewer.py
│ └── github_analyzer.py
│
├── utils/
│ ├── llm_client.py
│ └── parser.py
│
├── .env
├── requirements.txt
├── Dockerfile
└── README.md


---

## 🔧 Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/career-mcp-server.git
cd career-mcp-server
2️⃣ Create Virtual Environment
python -m venv venv
Activate:

Windows
venv\Scripts\activate

Linux / Mac
source venv/bin/activate

3️⃣ Install Dependencies
pip install -r requirements.txt


4️⃣ Environment Variables
Create .env file:

OPENAI_API_KEY=your_api_key
GITHUB_TOKEN=your_github_token


▶️ Running the MCP Server
python server.py

🐳 Running with Docker
Build Image:

docker build -t career-mcp .
Run Container:

docker run career-mcp
🔌 Connecting to MCP Client
Example configuration:

{
  "mcpServers": {
    "career-mcp": {
      "command": "python",
      "args": ["server.py"]
    }
  }
}

🎯 Use Cases
Developer productivity assistant

Career preparation automation

AI-powered coding mentor

Resume optimization

Interview preparation system

GitHub project evaluation

🚀 Future Enhancements
Email job alerts automation

WhatsApp notifications

Multi-agent orchestration

Skill gap analysis dashboard

Web UI interface

Cloud deployment (AWS/GCP)

👨‍💻 Author
Akashkumar Yadav

Backend Engineer

Java | Spring Boot | Microservices | Python

GitHub: https://github.com/Akashkumar231

LinkedIn: https://linkedin.com/in/akashkumaryadav1

⭐ Contribution
Contributions, issues, and feature requests are welcome!

