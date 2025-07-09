# 📬 Mail Merge Project - Personalized Letter Generator

This project uses Python to automate the process of creating personalized letters for multiple recipients. It reads a list of names from a `.txt` file, merges each name into a template letter, and generates a custom letter for each person.

---

## 📁 Project Structure

project_folder/
├── Input/
│   ├── Names/
│   │   └── invited_names.txt
│   └── Letters/
│       └── starting_letter.txt
├── Output/
│   └── ReadyToSend/
│       └── letter_for_Alice.docx
├── mail_merge.py



---

## 📌 Features

- Reads a list of names from `invited_names.txt`
- Loads a template letter containing a placeholder `[name]`
- Replaces the placeholder with each person's name
- Saves a custom letter as `letter_for_<name>.docx` in the `Output` folder

---

## ⚙️ How It Works

1. The placeholder `[name]` in the template is used as a marker.
2. Each name is stripped of whitespace (`stripped_name = name.strip()`).
3. The template letter is updated using `.replace(PLACEHOLDER, stripped_name)`.
4. The final letter is saved in the `Output/ReadyToSend/` directory.

---

## 📄 Example

**Template Letter (`starting_letter.txt`):**



**Generated Files:**
- `letter_for_Alice.docx`
- `letter_for_Bob.docx`
- `letter_for_Charlie.docx`

---

## 🚀 How to Run

1. Make sure you have Python installed (preferably 3.x).
2. Place your name list and letter template in the `Input` folder.
3. Run the script:

```bash
python main.py

