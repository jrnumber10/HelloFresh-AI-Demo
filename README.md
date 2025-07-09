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

## 💻 How to Run

1. **Clone or Download** this repo.
2. Install dependencies:
    ```sh
    pip install -r requirements.txt
    ```
3. Add your `.env` file with API key (see above).
4. Launch Jupyter:
    ```sh
    jupyter notebook
    ```
5. Open `HelloFresh_GenAi_demo_final.ipynb` and follow the prompts.

---

## 📚 Project Files

- `HelloFresh_GenAi_demo_final.ipynb` — Main interactive notebook
- `requirements.txt` — All required Python packages
- `README.md` — This file!

- ## 🙏 Credits

- HelloFresh for recipes & images (used for educational demo purposes)
- [OpenAI](https://platform.openai.com/) for LLM-powered chat

## 🛡️ License

MIT License 
