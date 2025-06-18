
# 📚 Zotero to Google Sheets

This Google Apps Script allows you to fetch **journal articles** from selected **Zotero subcollections** and export them into a **Google Sheet**, sorted by title. It is especially useful for researchers, students, or librarians who want to organize Zotero data in spreadsheets.

---

## ✅ Features

- Connects to your **Zotero library** via API.
- Retrieves **journal articles** from specified **subcollections** under a **parent collection**.
- Sorts items alphabetically by **title**.
- Displays **first author name**, **year**, and **title**.
- Writes results directly into a Google Sheet.
- Fetches up to **500 articles per subcollection**.

---

## 📦 Setup Instructions

### 1. Open a Google Sheet

Create a new or use an existing Google Sheet where you want to export your Zotero data.

### 2. Open Apps Script Editor

- Go to **Extensions > Apps Script**
- Delete any sample code and **paste the full script** from [`fetchZoteroItems.gs`](fetchZoteroItems.gs)

### 3. Customize the Script

Inside the script, replace the placeholders:

```js
const apiKey = 'REPLACE_WITH_YOUR_ZOTERO_API_KEY';
const userId = 'REPLACE_WITH_YOUR_ZOTERO_USER_ID';
const parentCollectionName = '6 Challenges';
const targetSubNames = ["Challenge 1", "Challenge 2", "Challenge 3", "Challenge 4", "Challenge 5", "Challenge 6"];
