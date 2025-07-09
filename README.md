# 🥕 HelloFresh GenAI Demo

Welcome to the **HelloFresh GenAI Recipe Recommendation Demo**!  
Find the best recipes based on your fridge ingredients, and chat with an AI chef about each recipe.

---

## 🚀 Features

- **Ingredient-based Recipe Matching**  
  Get top HelloFresh recipes based on what you have, ranked by ingredient match (primary/secondary weighted).

- **Pantry Detection**  
  Recognizes common pantry items (e.g., oil, butter, salt) and excludes them from matching penalties.

- **Synonym Matching**  
  Smart ingredient matching logic — “scallion” = “green onion”, etc.

- **Interactive Widgets**  
  Clean **Jupyter Notebook UI** with:
  - Ingredient search  
  - Match display with score breakdown  
  - AI-powered recipe Q&A using OpenAI

---

## 🛠️ Requirements

- **Python**: 3.10+ recommended (tested on 3.13.5)  
- **Jupyter Notebook**: Run locally or in a compatible environment  
- **Dependencies** (in `requirements.txt`):

```
fuzzywuzzy
ipywidgets
gradio
python-dotenv
openai
```

---

## 🔑 OpenAI API Key Required

To use AI features (recipe Q&A), you’ll need your own **OpenAI API key**.

1. Create a file named `.env` in the root of the project.
2. Add this line (replace with your key):

```
OPENAI_API_KEY=sk-...
```

3. Save the file.  
   Your key will be loaded automatically when running the notebook.

> ⚠️ **Never share your real API key publicly.**  
> The `.env` file is excluded from version control.

---

## 💻 How to Run

You can run this project using Jupyter Notebook or a virtual environment.

---

### 🅰️ If You Already Have Jupyter Installed

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt

# Add your API key
echo OPENAI_API_KEY=your-key-here > .env

# Launch notebook
jupyter notebook
```

Then open `HelloFresh_GenAi_demo_final.ipynb` and follow the prompts.

---

### 🅱️ Recommended: Virtual Environment Setup

For clean dependency isolation:

```bash
# Clone repo
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# Create & activate virtual environment
python -m venv venv
venv\Scripts\activate       # On Windows
# OR
source venv/bin/activate    # On macOS/Linux

# Install dependencies
pip install -r requirements.txt

# Add your API key
echo OPENAI_API_KEY=your-key-here > .env

# Launch notebook
jupyter notebook
```

💡 Use your system terminal (PowerShell, Terminal, bash, etc.) to run these commands.

---

## 📚 Project Files

- `HelloFresh_GenAi_demo_final.ipynb` — Main interactive notebook  
- `requirements.txt` — All required packages  
- `README.md` — This file!

---

## 🙏 Credits

- **HelloFresh** — Recipes & images (educational/demo use only)  
- **OpenAI** — GPT-powered chat assistant

---

## 🛡️ License

**MIT License**
