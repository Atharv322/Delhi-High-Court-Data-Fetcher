# Delhi High Court Case Scraper 🏛️📄

This project automates the retrieval of case information from the Delhi High Court website using **Python**, **Selenium**, and **OCR (Tesseract)**. It includes an interactive web interface built with **Flask** where users can input case details and download the related PDF.

----------------

## 🔧 Features

- ✅ Automates dropdown selections like *W.P.(C)* and inputting case numbers and years
- 🔍 Captures and solves number-based CAPTCHA using **Tesseract OCR**
- 📥 Downloads and saves the related case PDF
- 🌐 Flask-based web interface for user interaction
- 🧠 Assisted by **ChatGPT** for troubleshooting and development support

-----------------

## 📌 Technologies Used

- **Python 3.10+**
- **Selenium** for browser automation
- **OpenCV + pytesseract** for image processing and CAPTCHA solving
- **Flask** for the web UI
- **Chrome WebDriver** (headless/visible browsing)

---------------

## 📁 Project Structure

delhi-high-court-scraper/
│
├── app.py                  # Flask application entry point
├── court_scraper.py        # Main logic for Selenium automation and OCR using pytesseract
│
├── templates/              # HTML templates used by Flask
│   ├── index.html          # Main form for user input
│   ├── success.html        # Page shown after successful scraping
│   ├── error.html          # Page shown if scraping fails
│   └── history.html        # Optional page for showing past results (if implemented)
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation with setup and usage


---------------

## ⚙️ Installation

### Prerequisites:
- [Python](https://www.python.org/downloads/)
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)

### 📦 Install Python Packages:
```bash
pip install -r requirements.txt

----------------

🧠 Add Tesseract to PATH:

# Add to environment variables:
C:\Program Files\Tesseract-OCR

-----------------

🚀 Run the Project

python app.py

----------------

🔐 CAPTCHA Solving with OCR

The Delhi High Court website presents simple digit-based CAPTCHAs. We use the following process:

Screenshot CAPTCHA using Selenium

Preprocess image using OpenCV (grayscale, thresholding)

Extract digits with pytesseract

Input the result in the form for bypass

------------------

🤖 Credits
Developed by [Atharv Singh]

Prompt engineering & debugging with ChatGPT (OpenAI)

CAPTCHA OCR using Tesseract

Automation with Selenium WebDriver


------------------

Licensed under the Apache License 2.0. 
