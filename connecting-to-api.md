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
```

| Error | Meaning | Solution |
| -------- | ------- | ------- |
| `Invalid API Key`  | Your API key is incorrect or expired.    | Double-check key & regenerate if needed. Make sure env or google colab key is set up correctly (sometimes there's just a typo in the variable name!)   |
| `Rate Limit Exceeded` | You made to many requests in a period of time.     | Wait for your quota to reset, upgrade plan, set up warnings, etc.   |
| `Connection Timeout` | API is taking too long to respond.   | Retry with [exponential backoff](https://medium.com/@suryasekhar/exponential-backoff-decorator-in-python-26ddf783aea0).   |


