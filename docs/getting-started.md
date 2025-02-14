---
title: "Getting Started"
parent: "Home"
nav_order: 1
---

# Getting Started  

## Installing Python  
To follow along, install Python from [Python.org](https://www.python.org/downloads/).  

If you're using **Google Colab**, no installation is required! Just open Colab and start coding in the cloud.  

## Setting Up Your Development Environment  
- [Google Colab](https://colab.research.google.com/)  
- [Visual Studio Code (VSC)](https://code.visualstudio.com/)  

## API Key Setup  
Follow these steps to set up your **Gemini AI API key**:  

1. Sign up and generate an API key: [Gemini AI](https://ai.google.dev/)
2. If using Google Colab, follow [these instructions](https://colab.research.google.com/github/google-gemini/cookbook/blob/main/quickstarts/Authentication.ipynb).
3. If developing locally, [store your key](https://www.geeksforgeeks.org/how-to-create-and-use-env-files-in-python/) securely using an **.env file**:  

```python
from dotenv import load_dotenv
import os

load_dotenv()
API_KEY = os.getenv("GEMINI_API_KEY")
```
