# ✍️ Review Maker – Game Review Generator with AI & BBCode Output

**Review Maker** is a cross-platform, Python-powered utility that helps you write, format, and enhance structured game reviews — especially useful for forums or personal archives.

It offers:
- 📝 Clean, consistent review structure
- 📋 Auto-generated **BBCode** for forum posting
- 📄 Plain text output for archiving or sharing
- 🤖 Optional AI-enhancement using [Groq + LLaMA 3](https://console.groq.com/)
- 🖥️ Cross-platform support via `.bat` (Windows) or `.sh` (Linux/macOS)

---

## 📦 Features

- Interactive prompt to choose AI-enhanced or manual review mode
- Opens your system’s default editor for a friendly writing experience
- Parses structured input (`### section`) into full formatted output
- Generates both:
  - `compiled_review.txt` (plain text)
  - `compiled_review_bbcode.txt` (forum-ready BBCode)
- Copies BBCode output to clipboard automatically (Windows only)
- Respects OS and editor differences
- Automatically checks and installs Python dependencies

---

## 🧰 Requirements

- Python 3.8+
- [Groq API Key](https://console.groq.com/) (optional, for AI)
- Dependencies (installed via script):
  - `pyperclip`
  - `groq`

---

## 🚀 Quick Start

### 1. Clone or Download This Repository

```bash
git clone https://github.com/your-username/review-maker.git
cd review-maker
```
### 2. Install Dependencies
```bash
python install_requirements.py
```
This will install the required Python packages automatically.

### 3. Run the Tool
On Windows
Double-click run_review.bat or run:
```bash
run_review.bat
```
You'll be prompted:
Do you want to use AI for review enhancement? Press Y for Yes, N for No.

On Linux / macOS (Optional)
Make run_review.sh executable:
```bash
chmod +x run_review.sh
./run_review.sh
```
---
📝 Writing Your Review
The tool will open a file (review.txt) in your system's text editor with this format:
```shell
### Game
My Cool Visual Novel

### Main
This is my personal impression...

### Gameplay
Choices matter, and pacing is solid...

### Combat
(Not applicable)

### Art
Character art is clean and expressive...

### Story
Engaging plot with a few unexpected twists.

### H-Content
Mild, optional, tasteful.

### Pros
Great soundtrack
Meaningful choices

### Cons
Short runtime
No gallery mode

### TLDR
A solid short VN with heart.
```
---
📄 Output Files
After editing, the tool creates:

- compiled_review.txt – plain text version
- compiled_review_bbcode.txt – ready-to-paste forum version
- Clipboard will be updated with BBCode (Windows only)
---
🤖 Optional: Use AI to Enhance Writing
If you choose Y during the prompt, the script will:
Use Groq's LLaMA 3 backend to rephrase or enhance your sections
To enable AI:
- Get your API key from https://console.groq.com/
- Paste it into a file named token.txt in the root directory

That's it! The AI-enhanced version will be used automatically
