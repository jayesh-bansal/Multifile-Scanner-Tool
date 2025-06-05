# 📁 FileScanner

`FileScanner` is a powerful Python-based command-line tool that searches for a given keyword across various file types in a specified directory. It supports `.txt`, `.docx`, `.pdf`, and `.xlsx` files.

---

## 🔧 Features

- ✅ Search for a specific word or regex pattern in multiple file formats
- 📄 Supports `.txt`, `.docx`, `.pdf`, and `.xlsx`
- 📊 Shows match locations: line/page numbers and character positions
- 🔄 Option to scan different directories and repeat searches
- ⚙️ Minimal dependencies, easy to use CLI

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/jayesh-bansal/Multifile-scanner-tool.git
cd filescanner
```

📥 Install Dependencies
Install all required libraries via pip:

```bash
pip install -r requirements.txt
```

If you don't have a requirements.txt, you can install dependencies manually:

```bash
pip install python-docx openpyxl pypdf
```

▶️ Usage
Run the script using:

```bash
python app.py
```
You will be prompted to:

1. Enter or skip changing the directory

2. Enter a keyword or regex to search

3. View the results with file name, location, and character position

🧾 Example Output
``` pgsql
Enter 1 to change location or any key to continue: 1
Enter folder location: /path/to/your/files
Enter the word to search: confidential

Scanning: report.docx (1/10)
Found in report.docx at line 12, character 45

Scanning: summary.pdf (2/10)
Found in summary.pdf at page 3, character 123
```

📁 Supported File Types
.txt — Plain text files

.docx — Microsoft Word documents

.pdf — Portable Document Format files

.xlsx — Microsoft Excel spreadsheets

📌 Notes
Uses re.finditer() for flexible pattern matching.

Skips unreadable or unsupported files with exception handling.

Designed to be extensible if you want to add more file types.

📂 File Structure
```bash
.
├── app.py              # Main scanner script
├── README.md           # Project documentation
├── requirements.txt    # Python dependencies (optional)
```

👤 Author
Jayesh Bansal

Feel free to star ⭐ the repo, open issues 🐞, or contribute via pull requests 🛠️.
