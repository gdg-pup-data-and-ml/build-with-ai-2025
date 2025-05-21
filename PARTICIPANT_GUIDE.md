# 🚀 Build with AI 2025: Complete Participant Setup Guide
![Event Date](https://img.shields.io/badge/Event%20Date-May%2024%2C%202025-blue)
![Host](https://img.shields.io/badge/Host-GDG%20On%20Campus%20PUP-red)
![Focus](https://img.shields.io/badge/Focus-Gemini%20%26%20Streamlit-green)

This document provides all the information you need to prepare for the event. Make sure to complete all setup steps before the workshop!

## 📋 Quick Checklist
- [ ] Create Google AI Studio account
- [ ] Setup Google Cloud Platform account
- [ ] Access Google Colab
- [ ] Install Python 3.12
- [ ] Install Visual Studio Code
- [ ] Install UV Package Manager
- [ ] Install Git
- [ ] Setup Python Virtual Environment
- [ ] Create Streamlit Account

---

## 🔑 Essential Accounts
Before the event, please ensure you have created accounts on the following platforms:

### ![Google AI Studio](https://img.shields.io/badge/Google%20AI%20Studio-4285F4?style=flat&logo=google&logoColor=white)
- **URL**: https://aistudio.google.com/
- Sign in with your Google account
- Familiarize yourself with the interface

### ![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)
- **URL**: https://console.cloud.google.com/
- Create a new account or sign in with your Google account
- We'll set it up during the event, just make sure you have an account

### ![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=flat&logo=googlecolab&logoColor=white)
- **URL**: https://colab.research.google.com/
- Sign in with your Google account
- Try creating a new notebook to ensure your account is working (just click this link https://colab.new/)

### ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)
- **URL**: https://streamlit.io/
- Sign up for a free account
- This will be essential for deploying your AI assistant project

---

## 💻 Required Software

### ![Python](https://img.shields.io/badge/Python%203.12-3776AB?style=flat&logo=python&logoColor=white)
Installing Python
1. Open Windows PowerShell and execute:
```powershell
winget install -e --id Python.Python.3.12
```
2. During installation, ensure you check the `Add to PATH` option for a smooth workflow.
3. Verify installation by opening command prompt and running:
```powershell
python --version
```

### ![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white)
Installing Visual Studio Code
1. Open Windows PowerShell and execute:
```powershell
winget install -e --id Microsoft.VisualStudioCode
```
2. Verify installation by opening VS Code from the Start menu

### ![UV](https://img.shields.io/badge/UV%20Package%20Manager-7E57C2?style=flat&logo=astro&logoColor=white)
Installing UV Package Manager
1. Open Windows PowerShell and run:
```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```
2. Verify installation by running:
```powershell
uv --version
```

### ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
Installing Git
1. Download Git from https://git-scm.com/download/win
2. Install with default options
3. Verify installation:
```powershell
git --version
```

---

## 🛠️ Python Virtual Environment Setup

Setting up a virtual environment is crucial for isolating your project dependencies. Follow these steps to ensure your Python environment is correctly configured:

1. After installing Python and VS Code:
   - Open VS Code
   - Create and open a new project folder
   - Open the terminal in VS Code (**Ctrl+`**)

2. Create a virtual environment:
```bash
python -m venv venv
```
   - You'll notice a `.venv` folder is created in your project directory

3. Activate the virtual environment:
   - On Windows:
```bash
.\venv\Scripts\activate
```
   - On macOS/Linux:
```bash
source venv/bin/activate
```
   - Your terminal prompt should change to indicate the active environment

4. Update pip inside the virtual environment:
```bash
pip install --upgrade pip
```

5. Check installed packages:
```bash
pip list
```
   - This will show all modules in your virtual environment (initially just pip and setuptools)

6. Test your environment by installing a package:
```bash
pip install numpy
pip list
```
   - You should see numpy now listed among your installed packages

7. When you're done working in the virtual environment, you can deactivate it:
```bash
deactivate
```

**Important**: Always activate your virtual environment before working on your project!

---

## 🌟 Streamlit Account & Testing

### Creating a Streamlit Account
1. Visit https://streamlit.io/ and click "Sign up"
2. Create an account using your Google account or email
3. Verify your email if necessary

### Testing Streamlit Locally
1. In your activated virtual environment, install Streamlit:
```bash
pip install streamlit
```

2. Verify the installation:
```bash
streamlit --version
```

3. Create a test file named `streamlit_test.py` with this content:
```python
import streamlit as st

st.title("Hello Streamlit!")
st.write("This is a test of my Streamlit setup for Build with AI 2025.")

name = st.text_input("What's your name?")
if name:
    st.write(f"Hello, {name}!")
```

4. Run your Streamlit app:
```bash
streamlit run streamlit_test.py
```

5. A browser window should open showing your Streamlit app. If this works, you're all set for the workshop!

---

## 📱 Contact Information
If you encounter any issues with the setup process, please contact:
![Email](https://img.shields.io/badge/Email-gdg.pup.dataml%40gmail.com-yellow?style=flat&logo=gmail&logoColor=white)

We're looking forward to building amazing AI applications with you on May 24, 2025!

---

> *Note: This setup guide is based on Windows systems. Mac and Linux users may need to adjust installation commands accordingly. Please reach out if you need assistance with non-Windows setup.*

![Powered by Google](https://img.shields.io/badge/Powered%20by-Google%20Developer%20Groups-4285F4?style=flat&logo=google&logoColor=white)
