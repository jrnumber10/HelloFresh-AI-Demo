# 🥕 HelloFresh GenAI Demo

Welcome to the HelloFresh GenAI Recipe Recommendation Demo!  
Find the best recipes based on your fridge ingredients, and chat with an AI chef about each recipe.

---

## 🚀 Features

- **Ingredient-based Recipe Matching:**  
  Get top HelloFresh recipes based on what you have, ranked by ingredient match (primary/secondary weighted).

- **Pantry Detection:**  
  Knows common pantry items (like oil, butter, salt).

- **Synonym Matching:**  
  Smart ingredient synonym logic — “scallion” = “green onion”, etc.

- **Interactive Widgets:**  
  Clean Jupyter notebook UI with search, result display, and recipe Q&A chat (OpenAI powered).

---

## 🛠️ Requirements

- **Python:** 3.10+ recommended (works on 3.13.5)
- **Jupyter Notebook** (run locally or on Colab)
- **See [`requirements.txt`](./requirements.txt) for libraries:**
  - `fuzzywuzzy`
  - `ipywidgets`
  - `gradio`
  - `python-dotenv`
  - `openai`

---

## 🔑 OpenAI API Key Required

To use the AI features (recipe chat/Q&A), you’ll need your own [OpenAI API key](https://platform.openai.com/account/api-keys):

1. Create a file named `.env` in the project root.
2. Add this line (replace with your key):
    ```
    OPENAI_API_KEY=sk-...
    ```
3. Save the file.

Your key will be **loaded automatically** when you run the notebook.

> **Never share your real API key publicly!  
> The `.env` file is not included in this repo for your safety.**

---

💻 How to Run
You can run this project either by using Jupyter Notebook directly or setting up a Python virtual environment for isolation.

🅰️ If You Already Have Jupyter Installed:
bash
Copy
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
# Create a .env file in this folder
# Add your OpenAI key: OPENAI_API_KEY=your-key-here
jupyter notebook
Then open HelloFresh_GenAi_demo_final.ipynb and follow the prompts.

🅱️ Set Up with Virtual Environment (Recommended):
For a clean install without interfering with global packages:

bash
Copy
# 1. Clone the repo
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# 2. Create a virtual environment
python -m venv venv

# 3. Activate it
venv\Scripts\activate         # On Windows
# OR
source venv/bin/activate     # On macOS/Linux

# 4. Install dependencies
pip install -r requirements.txt

# 5. Add your OpenAI key in a .env file
echo OPENAI_API_KEY=your-key-here > .env

# 6. Launch Jupyter
jupyter notebook

## 📚 Project Files

- `HelloFresh_GenAi_demo_final.ipynb` — Main interactive notebook
- `requirements.txt` — All required Python packages
- `README.md` — This file!

- ## 🙏 Credits

- HelloFresh for recipes & images (used for educational demo purposes)
- [OpenAI](https://platform.openai.com/) for LLM-powered chat

## 🛡️ License

MIT License 
