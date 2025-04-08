# 🧠 Student Database RAG Assistant

This project is a **Retrieval-Augmented Generation (RAG)** chatbot built using **LangGraph**, **LangChain**, and **Google Gemini**. It allows users to interactively query and analyze student data stored in a local SQLite database.

---

## 🚀 Features

- Conversational interface to query student information
- Uses a tool-augmented language model (LLM + SQL)
- Executes real-time queries on a SQLite database
- Built with LangGraph for dialogue flow management
- Includes sample student data for quick testing

---

## 🛠️ Technologies Used

- Python
- SQLite
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [LangChain](https://www.langchain.com/)
- [Google Generative AI (Gemini)](https://ai.google.dev/)
- Google Colab

---

## 📁 Project Structure

| File / Section        | Description                                      |
|------------------------|--------------------------------------------------|
| `DatabaseManager`      | Handles SQLite connection and queries            |
| `ask_students_db`      | LangChain tool for querying student database     |
| `chatbot_node`         | Generates assistant replies using Gemini         |
| `human_node`           | Handles user input                               |
| `build_graph()`        | Creates LangGraph flow with nodes and edges      |
| `setup_database()`     | Initializes and populates sample data            |
| `main()`               | Runs the full application                        |

---

## ▶️ How to Run

1. Open the notebook in **Google Colab**.
2. Set your `GOOGLE_API_KEY` using `userdata.get()` (already in code).
3. Run all cells.
4. The assistant will greet you with:
   Welcome to the Student Database Assistant...
5. Ask questions like:
- `How many students are studying Computer Engineering?`
- `Who has the highest GPA?`
- `Show me all married students in PhD.`

---

## 💡 Example Questions

- `List all students over the age of 25.`
- `What is the average GPA for Physics majors?`
- `How many single students are there?`

---

## ⚠️ Notes

- **Important:** Use `check_same_thread=False` when connecting to SQLite to avoid thread-related errors.
- A **Google Gemini API key** is required to use the assistant.

---

## 📌 License

MIT License (feel free to modify or extend)

---
