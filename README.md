# 🧪 Automated REST API Validation Suite

## 📌 Project Overview
A comprehensive QA testing framework built using Postman. This suite automates the validation of RESTful backend endpoints across the CRUD (Create, Read, Delete) lifecycle, ensuring data integrity and correct HTTP status code responses.

## ⚙️ Tech Stack
* **Tool:** Postman
* **Architecture:** REST APIs
* **Data Format:** JSON
* **Automation:** JavaScript (Postman Sandbox API)

## 🚀 Testing Scope
This suite validates the following endpoints against a user database API (`reqres.in`), utilizing custom header authorization (`x-api-key`):

1. **GET (Read):** Retrieves user data.
   * *Assertion:* Validates HTTP `200 OK`.
2. **POST (Create):** Ingests JSON payload to create a new user record.
   * *Assertion:* Validates HTTP `201 Created` to ensure database insertion logic fired correctly and an ID was generated.
3. **DELETE (Delete):** Removes user record.
   * *Assertion:* Validates HTTP `204 No Content` for graceful deletion handling.

## 💻 How to Run the Tests Locally
1. Clone this repository or download the `.json` file.
2. Open Postman and click `Import` in the top left corner.
3. Drag and drop the `.json` file into the Postman window.
4. Open the imported collection and click `Run` to execute the automated JavaScript assertions.
