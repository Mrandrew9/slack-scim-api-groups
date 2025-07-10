# 🚀 Slack SCIM API – Group Creation Example (Postman)

This project demonstrates how to create a group in Slack using the SCIM API via Postman.

> ⚠️ This feature requires a **Slack Enterprise Grid** plan with **SCIM API access enabled**.

---

## 📦 What's Included

- ✅ Step-by-step instructions to create a group using Postman
- 🔐 Authorization setup with Bearer Token
- 📄 Example SCIM-compliant JSON payload
- 📁 Postman collection file (`.json`)

---

## 🛠 Prerequisites

- A Slack Enterprise Grid workspace
- A valid SCIM API token (you get this from your Slack admin settings)
- [Postman](https://www.postman.com/downloads/) installed

---

## 📚 Instructions

### 1. Open Postman and Create a New Request
- Set the method to `POST`
- Use the URL:  

https://api.slack.com/scim/v1/Groups



### 2. Authorization Tab
- Type: `Bearer Token`
- Token: Paste your SCIM API token

### 3. Headers Tab
| Key           | Value              |
|---------------|--------------------|
| Content-Type  | application/json   |

### 4. Body Tab
- Select `raw` and format as `JSON`
- Paste this payload:
```json
{
"schemas": ["urn:scim:schemas:core:1.0"],
"displayName": "TestGroup"
}
