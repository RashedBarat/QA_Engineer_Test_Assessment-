# API Test Assessment – GoREST Public API

This repository contains a set of API test cases prepared for interview assessment using the [GoREST API](https://gorest.co.in). The test cases are designed and exported from Postman as a collection file.

---

## Project Contents

- `QA Engineer Test Assessment.postman_collection.json`: Postman collection file containing 5 test requests for:
  - Creating a user (POST)
  - Verifying user status (GET)
  - Updating a user (PUT)
  - Partially updating a user (PATCH)
  - Deleting a user (DELETE)

---

## Prerequisites

- [Postman](https://www.postman.com/downloads/) (Desktop App or Web)
- A valid GoREST API Access Token (you can generate one from: [https://gorest.co.in](https://gorest.co.in))

---

## Setup Instructions

1. Open Postman.
2. Click on **Import** (top-left corner).
3. Choose **Upload Files** and select the file `QA Engineer Test Assessment.postman_collection.json`.
4. After importing, the collection named **"QA Engineer Test Assessment"** will appear in your sidebar.

---

## Configure Authorization

1. In Postman, click on the collection **"QA Engineer Test Assessment"**.
2. Go to the **Variables** tab.
3. Create a new variable:
   - Key: `access_token`
   - Initial Value: `<your_gorest_token_here>`
   - Current Value: `<your_gorest_token_here>`

 Your token will automatically be used in all request headers that need it.

---

## How to Execute the Tests

### Scenario 1: Create a New Employee (POST)

- Request: `createAUser`
- Verifies that:
  - A new user is created with random values.
  - The returned `id` is a numeric type.
  - Status code is 201 (Created).

### Scenario 2: Verify Status (GET)

- Request: `statusVerification`
- Verifies that:
  - The first user's `status` is either `"active"` or `"inactive"`.

### Additional Test Requests

- `Update_User_PUT`: Replaces user details using PUT.
- `Patch`: Updates user email using PATCH.
- `Delete`: Deletes the user by ID using DELETE.
 You can run individual requests or click on the collection and select "Run collection" to execute all.

---
