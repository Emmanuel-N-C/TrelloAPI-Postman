# 📋 Trello API Automation with Postman

This repository contains a comprehensive Postman test collection for **Trello's REST API**, using dynamic variables and environment configuration. It allows you to automate the entire lifecycle of a Trello board — from creation, list and card management, to updates and deletion.

---

## 🌍 Environment Setup

The included Postman environment (`Trello APIs Environment`) contains dynamic and reusable variables used throughout the collection:

| Variable         | Description                                |
|------------------|--------------------------------------------|
| `base_url`       | Base URL for Trello API (`https://api.trello.com`) |
| `key`            | Your Trello API key                        |
| `token`          | Your Trello access token                   |
| `boardID`        | Auto-generated board ID                    |
| `myboardname`    | Dynamic board name                         |
| `listID`         | Auto-generated list ID                     |
| `mylistname`     | Dynamic list name                          |
| `cardID`         | Auto-generated card ID                     |
| `mycardname`     | Dynamic card name                          |


---

## 📂 Collection Overview

The Postman collection (`Trello APIs.postman_collection.json`) includes requests grouped by feature:

### ✅ Core Features Covered

| Operation            | Description                                     |
|----------------------|-------------------------------------------------|
| **Create Board**     | Dynamically create a new Trello board           |
| **Get Board**        | Retrieve the created board by ID                |
| **Update Board**     | Change board title and description              |
| **Delete Board**     | Remove the created board                        |
| **Create List**      | Add a new list to the board                     |
| **Get List**         | Retrieve a specific list by ID                  |
| **Update List**      | Rename an existing list                         |
| **Archive List**     | Archive all cards in the list                   |
| **Create Card**      | Add a card to the list                          |
| **Update Card**      | Rename or edit card data                        |
| **Delete Card**      | Permanently delete a card                       |
| **Get Deleted/Archived** | Validate deletion or archive behavior      |

Each request includes:
- 🔒 API Key/Token authentication
- 🧪 Built-in **test scripts** to validate:
  - Status codes (e.g. `200 OK`, `404 Not Found`)
  - Data structure integrity
  - Dynamic variable storage (e.g. `boardID`, `listID`, `cardID`)
  - Response time checks

---

## ▶️ Getting Started

### 1. **Import into Postman**

- Open Postman
- Click **Import**
- Upload:
  - `Trello APIs.postman_collection.json`
  - `Trello APIs Environment.postman_environment.json`

### 2. **Select the Environment**
In the top-right of Postman, select `Trello APIs Environment`.

### 3. **Run the Collection**
- Use the **Collection Runner** to execute all requests in sequence.
- Or run requests one by one to observe test results and variable updates.

---

