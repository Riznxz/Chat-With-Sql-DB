# 💬 LangChain: Chat with SQL Database

An AI-powered conversational interface to interact with SQL databases using natural language. Ask questions in plain English and get instant answers from your SQLite or MySQL databases.

<!-- Add your screenshot here -->
![App Demo](sqlchat.png)

## ✨ Features

- 🗣️ **Natural Language Queries**: Ask questions in plain English
- 🗄️ **Multi-Database Support**: SQLite 3 and MySQL
- 🤖 **Intelligent SQL Agent**: Automatically generates and executes SQL queries
- ⚡ **Real-time Streaming**: Live response generation
- 💬 **Chat Interface**: Conversational UI with message history
- 🔒 **Secure**: Password-protected database credentials
- 🎯 **Zero-Shot Learning**: No training required

## 🚀 Quick Start

### Prerequisites

```bash
Python 3.8+
Groq API Key
SQLite3 or MySQL Database
```

### Installation

```bash
# Clone the repository
git clone https://github.com/Riznxz/Chat-With-Sql-DB
cd chat-with-sql-db

# Install dependencies
pip install -r requirements.txt
```

### Setup Database

**Option 1: SQLite (Included)**
```bash
# Create sample student database
python sqlite.py
```

**Option 2: MySQL**
- Have your MySQL credentials ready
- Configure in the app sidebar

### Run the App

```bash
streamlit run app.py
```

## 💡 Usage Examples

### Sample Questions

**For Student Database:**
```
❓ "How many students are there?"
❓ "Who scored the highest marks?"
❓ "Show all students in Data Science class"
❓ "What is the average marks in section A?"
❓ "List students who scored above 85"
```

### How It Works

1. **Select Database**: Choose SQLite or MySQL from sidebar
2. **Enter Credentials**: Provide database connection details
3. **Add Groq API Key**: Enter your Groq API key
4. **Start Chatting**: Ask questions in natural language
5. **Get Answers**: Receive formatted responses instantly

## 🗄️ Database Schema

### Student Database (SQLite)

```sql
CREATE TABLE STUDENT(
    NAME VARCHAR(25),
    CLASS VARCHAR(25),
    SECTION VARCHAR(25),
    MARKS INT
)
```

**Sample Data:**
| NAME | CLASS | SECTION | MARKS |
|------|-------|---------|-------|
| Krish | Data Science | A | 90 |
| John | Data Science | B | 100 |
| Mukesh | Data Science | A | 86 |
| Jacob | DEVOPS | A | 50 |
| Dipesh | DEVOPS | A | 35 |

## 🔧 Configuration

### Groq API Key

Get your free API key from [Groq Console](https://console.groq.com/)

### MySQL Setup

If using MySQL, provide:
- **Host**: MySQL server address
- **User**: Database username
- **Password**: Database password
- **Database**: Database name

## 🛠️ Tech Stack

- **Frontend**: Streamlit
- **LLM**: Groq (llama-3.1-8b-instant)
- **Framework**: LangChain
- **Databases**: SQLite3, MySQL
- **Agent**: Zero-Shot React Description Agent

## 📦 Dependencies

```txt
streamlit
langchain
langchain_groq
langchain_community
sqlalchemy
sqlite3
mysql-connector-python
python-dotenv
```

## 🎯 Features in Detail

### 🤖 SQL Agent
- Automatically generates SQL queries from natural language
- Validates and executes queries safely
- Interprets results into human-readable answers

### 💬 Chat Interface
- Clean, intuitive UI
- Message history preservation
- Clear history option
- Real-time streaming responses

### 🔒 Security
- Read-only database access for SQLite
- Password masking for sensitive data
- Secure connection handling

## 🚦 Project Structure

```
chat-with-sql-db/
│
├── app.py                 # Main Streamlit application
├── sqlite.py              # SQLite database setup
├── student.db             # Sample database (generated)
├── requirements.txt       # Python dependencies
├── README.md             # Documentation
│
└── screenshots/          # App screenshots
    ├── app_demo.png
    └── ...
```

## 📝 How to Add Screenshots

1. Create a `screenshots` folder in your project root
2. Take screenshots of your app
3. Save them with descriptive names:
   - `app_demo.png` - Main interface
   - `chat_example.png` - Sample conversation
   - `mysql_config.png` - MySQL configuration
   - `results.png` - Query results

4. Update README with actual screenshot paths:
```markdown
![Main Interface](./screenshots/app_demo.png)
![Chat Demo](./screenshots/chat_example.png)
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [LangChain](https://python.langchain.com/) for the amazing framework
- [Groq](https://groq.com/) for fast LLM inference
- [Streamlit](https://streamlit.io/) for the beautiful UI framework

## 📧 Contact

Your Name - [@yourtwitter](https://twitter.com/yourtwitter)

Project Link: [https://github.com/yourusername/chat-with-sql-db](https://github.com/yourusername/chat-with-sql-db)

---

⭐ **Star this repo if you find it helpful!**
