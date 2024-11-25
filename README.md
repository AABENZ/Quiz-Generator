# 🚀 Quiz App Generator

This is a **Streamlit-based web application** that allows users to generate, answer, and evaluate quizzes on any topic using AI-powered question generation. The app integrates with **Supabase** for storing quiz data and utilizes **Educhain** to generate questions with a custom AI model hosted on Cerebras.

![App Screenshot](https://i.ibb.co/m07RtsG/2024-11-25-01-48.png)
---

## 📝 Features

### User Features
- **Customizable Quiz Generation**:
  - Define the quiz topic.
  - Specify the number of questions (1–50).
  - Add custom instructions for more tailored question generation.
- **Interactive Quiz Interface**:
  - Answer multiple-choice questions.
  - Submit answers and receive instant feedback.
  - View correct and incorrect answers with explanations.
- **Performance Tracking**:
  - Displays final score and percentage after submission.
  - Option to retake quizzes.

### Administrative Features
- **Data Persistence**:
  - Saves quiz metadata (topic, latency, etc.) to Supabase.
  - Provides retry logic for database operations to ensure data integrity.
- **Quiz Statistics**:
  - Average quiz generation time.
  - Total quizzes generated.

---

## 🛠️ Technology Stack

### Backend
- **Educhain**: AI-powered question generation.
- **Supabase**: Database for storing quiz data.
- **Cerebras AI API**: Language model hosting for generating questions.

### Frontend
- **Streamlit**: Simple and interactive web UI.

### Programming and Libraries
- **Python**: Core programming language.
- **Key Libraries**:
  - `langchain_openai`: Manages the AI model and handles requests.
  - `dotenv`: Loads environment variables.
  - `supabase`: Integrates the Supabase database.

---

## 🖥️ Setup and Installation

### Prerequisites
- Python 3.8+
- Streamlit installed
- A Supabase account
- Access to the Cerebras AI API

### Installation Steps
1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo-name/quiz-app-generator.git
   cd quiz-app-generator
2. Install dependencies:

   ```bash
	pip install -r requirements.txt

3. Create a `.env` file to store environment variables:

   ```bash
	SUPABASE_URL=your_supabase_url
	SUPABASE_API_KEY=your_supabase_api_key
	CEREBRAS_API_KEY=your_cerebras_api_key

4. Run the app:

   ```bash
	streamlit run app.py