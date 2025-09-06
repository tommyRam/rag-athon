# RAG-Athon Project

This project demonstrates Retrieval-Augmented Generation (RAG) using Gemini API and Jupyter Notebook.

## 🛠️ Local Setup

### 1. Create a Python Virtual Environment

```powershell
python -m venv venv
venv\Scripts\activate
```

### 2. Get a Free Gemini API Key

- Go to [Google AI Studio](https://aistudio.google.com/app/apikey) and sign in with your Google account.
- Click **Create API Key** and copy your key.

### 3. Configure Environment Variables

- Copy `.env.example` to `.env`:
  ```powershell
  copy .env.example .env
  ```
- Open `.env` and paste your Gemini API key:
  ```env
  GEMINI_API_KEY=your_api_key_here
  ```

### 4. Install Dependencies

```powershell
pip install -r requirements.txt
```

### 5. Launch Jupyter Lab

```powershell
jupyter lab
```

- Open `rag.ipynb` and run all cells.

---

## 🚀 Run on Google Colab

1. Open [Google Colab](https://colab.research.google.com/) and upload `rag.ipynb`.
2. In the first cell, install dependencies:
   ```python
   !pip install -r requirements.txt
   # Or, if requirements.txt is not uploaded:
   !pip install pandas openai google-auth google-api-python-client python-dotenv
   ```
3. Add your Gemini API key in a cell:
   ```python
   import os
   os.environ['GEMINI_API_KEY'] = 'your_api_key_here'
   ```
4. Run all cells in the notebook.

---

## 📄 Files

- `rag.ipynb`: Main notebook
- `requirements.txt`: Python dependencies
- `.env.example`: Example environment file
- `test_data.xlsx`: Sample data
- `data/`: Data folder

---

## 🔗 Useful Links

- [Google AI Studio API Key](https://aistudio.google.com/app/apikey)
- [Google Colab](https://colab.research.google.com/)
