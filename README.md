# Amazon Review Alert (n8n Workflow)

This repository contains an n8n automation workflow that analyzes Amazon product reviews using OpenRouter's GPT-3.5-turbo API and stores the sentiment and complaint results into a Google Sheet.

---

## 🔧 Features

- 📥 Input: Amazon review text, review ID, ASIN
- 🤖 AI Analysis: Sentiment & complaint detection via LLM (OpenRouter)
- 📊 Output: Results sent to a Google Sheet
- 🔔 Optional: Slack/email alerts can be added

---

## 🛠️ Technologies

- [n8n.io](https://n8n.io)
- [OpenRouter](https://openrouter.ai)
- Google Sheets API
- GPT-3.5 Turbo (OpenAI model via OpenRouter)

---

## 📄 Example Output

| sentiment | complaint        | asin       | review                                 | date                |
|-----------|------------------|------------|----------------------------------------|---------------------|
| negative  | Stopped working  | B09XYZ1234 | The kettle stopped working after a week | 2025-07-26T10:55Z   |

---

## ⚙️ Setup Notes

- Replace `Authorization` header in the HTTP Request with your own OpenRouter key
- Ensure Google Sheets credentials are correctly configured in n8n
- Limit execution to avoid quota errors from Google API

---

## 💡 Future Enhancements

- Competitor review monitoring
- Dashboard with visualization
- Keyword clustering for complaints

---

### Created with by Ezgi
