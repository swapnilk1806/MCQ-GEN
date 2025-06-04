# 📝 MCQ Generator

## Introduction
MCQ Generator is a dynamic web application designed to automate the creation of multiple-choice questions (MCQs) using advanced AI technologies. Hosted on an Ubuntu server via AWS EC2, this tool leverages the power of OpenAI’s language models combined with a user-friendly Streamlit interface to generate high-quality, context-aware MCQs across a variety of subjects.

This project is ideal for educators, trainers, and learners who want to accelerate quiz preparation, reduce manual effort, and ensure consistent question quality by harnessing AI-driven content creation.

---

## Purpose
The primary goal of the MCQ Generator project is to facilitate rapid, scalable, and intelligent question generation that adapts to diverse educational needs. Manual question creation is often time-consuming and prone to inconsistencies. This application addresses these challenges by:

- ⚡ Providing an automated, AI-based system to generate relevant and varied MCQs.
- 🎓 Enabling educators to focus on teaching rather than content creation.
- 🌐 Offering an accessible web platform that requires minimal technical setup.
- ☁️ Supporting seamless integration with cloud infrastructure to ensure availability and performance.

By delivering a robust, easy-to-use tool, the project aims to transform traditional assessment design workflows and empower users worldwide.

---

## Features
- ☁️ **Cloud-Hosted Deployment:** Runs on AWS EC2 Ubuntu instances to ensure scalability, security, and availability.
- 🤖 **AI-Powered Question Generation:** Uses OpenAI’s GPT models to create contextually accurate and diverse MCQs.
- 🎨 **Interactive Streamlit Interface:** Provides an intuitive, responsive UI for users to generate and review questions instantly.
- 🔧 **Environment Management:** Automated setup scripts handle dependency installation, environment configuration, and updates.
- 🔐 **Secure API Key Handling:** Supports environment variable management via `.env` files, protecting sensitive credentials.
- 🛠️ **Customizable & Extensible:** Modular codebase allows easy enhancements, including new question formats and AI fine-tuning.
- 🔓 **Port Accessibility:** Configurable AWS security groups enable secure access through custom ports (default Streamlit port: 8501).

---

## Installation and Deployment Guide

### 1. Launch AWS EC2 Instance
- 🔗 Login to [AWS Console](https://aws.amazon.com/console/).
- 🔎 Navigate to EC2 service.
- 🚀 Launch a new instance using Ubuntu Server (recommended latest LTS version).
- ⚙️ Configure instance details, storage, and security groups.
- 🔓 Ensure inbound rules allow SSH (port 22) and Streamlit default port (8501).

## 4)  Libraries Used 📦

| Library | Why It's Used | Link |
|--------|---------------|------|
| `os` | To interact with the operating system, such as accessing file paths and environment variables. | [os – Python Docs](https://docs.python.org/3/library/os.html) |
| `json` | For reading and writing JSON files, especially when dealing with structured data like questions. | [json – Python Docs](https://docs.python.org/3/library/json.html) |
| `traceback` | Helps with debugging by printing detailed error logs during exceptions. | [traceback – Python Docs](https://docs.python.org/3/library/traceback.html) |
| `pandas` | Used to read and manipulate tabular data (e.g., `.csv` files). | [Pandas Documentation](https://pandas.pydata.org/docs/) |
| `dotenv` (`python-dotenv`) | Loads environment variables from a `.env` file securely (like your OpenAI API key). | [python-dotenv GitHub](https://github.com/theskumar/python-dotenv) |
| `streamlit` | Provides the interactive web interface for uploading files and generating MCQs. | [Streamlit Documentation](https://docs.streamlit.io/) |
| `langchain` | Interfaces with OpenAI models and helps organize prompts and outputs logically. | [LangChain Docs](https://docs.langchain.com/) |
| `mcqgenrator.utils` | Custom module for reading files and extracting table data. | (Your own module) |
| `mcqgenrator.MCQGenrator` | Custom module that contains logic for generating and evaluating MCQs using OpenAI API. | (Your own module) |
| `mcqgenrator.logger` | Custom logger for saving debug or application logs. | (Your own module) |

---


### Prerequisites

- Python 3.8 or later
- OpenAI API Key

### Steps

1. **Clone the repository**
Clone project
```bash
git clone https://github.com/yourusername/mcq-generator-ai.git
```

Inside that Folder
```bash
cd mcq-generator-ai
```

Run Project Command 
```bash
streamlit run Streamlit.py
```

MIT License

Copyright (c) 2025 https://github.com/swapnilk1806/

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions: ...
