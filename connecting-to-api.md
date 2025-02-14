---
title: "Connecting to Gemini AI API"
parent: "Home"
nav_order: 2
---

# Connecting to Gemini AI API  

## Authenticating & Making Your First Request  

```python
import google.generativeai as genai

genai.configure(api_key="YOUR_API_KEY_HERE")

model = genai.GenerativeModel('gemini-1.5-flash')
response = model.generate_content("Summarize key trends in AI.")
print(response.text)
