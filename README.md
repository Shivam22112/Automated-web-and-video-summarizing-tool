# Automated Web & Video Summarizing Tool

> A browser extension and REST API that generates concise, human-like summaries from **web pages** and **YouTube videos**. Supports **translation** and **text-to-speech** for better accessibility.  
> Built with **Python (Flask)**, **Hugging Face BART**, **BeautifulSoup**, **pytube**, **AssemblyAI**, and **Google APIs**.

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)  
[![Flask](https://img.shields.io/badge/Flask-API-green)](https://flask.palletsprojects.com/)  
[![HuggingFace](https://img.shields.io/badge/HuggingFace-BART-orange)](https://huggingface.co/)  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 📌 Project Overview

With the massive growth of online content, users often face **information overload** when reading blogs or watching videos.  
This project solves that problem by:  
- **Summarizing web articles & YouTube videos** automatically  
- **Translating summaries** into multiple languages  
- **Converting summaries into speech** for accessibility  
- Offering a **browser extension** for one-click summarization  

---

## ✨ Features

- 🌐 **Webpage Summarization**: Extracts and summarizes key points from online articles.  
- 📹 **YouTube Summarization**: Downloads audio, generates transcript, and produces concise summaries.  
- 🌍 **Translation Support**: Summaries can be translated into different languages.  
- 🔊 **Text-to-Speech**: Converts summaries into speech for better accessibility.  
- 🖥️ **Browser Extension**: Lightweight extension (Manifest V3) for Chrome/Edge.  

---

## 🧱 Tech Stack

- **Backend**: Python, Flask  
- **NLP**: Hugging Face BART (`transformers`)  
- **Scraping**: BeautifulSoup4  
- **YouTube Processing**: pytube, AssemblyAI (speech-to-text)  
- **Translation**: deep-translator (Google Translate API)  
- **Frontend (Extension)**: HTML, CSS, JavaScript (Manifest V3)  

---

## 🗂 Project Structure

```bash
Automated-web-and-video-summarizing-tool/
├── app.py                 # Flask API endpoints
├── Audiodownloader.py     # YouTube audio extraction
├── Transcriptgenerator.py # Audio-to-text (AssemblyAI)
├── Summarizer.py          # HuggingFace BART summarizer
├── Summarize.py           # Alternative summarization (HugChat)
├── Translation.py         # Google Translator integration
├── BE_project Report.pdf  # Final year project report
├── BE- Project Final Review.pptx # Project presentation
├── requirements.txt       # Project dependencies
├── extension/             # Chrome/Edge browser extension
│   ├── manifest.json
│   ├── popup.html
│   ├── popup.js
│   ├── popup.css
│   └── content.js
└── README.md              # Documentation
