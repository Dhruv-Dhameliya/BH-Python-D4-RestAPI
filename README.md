# Flask REST API - User Management

This is a simple **REST API** built with **Flask** to manage user data.  
It supports basic CRUD operations (Create, Read, Update, Delete) on users.  

---

## 🚀 Features
- **GET** all users
- **GET** a single user by ID
- **POST** create a new user
- **PUT** update an existing user
- **DELETE** remove a user  
- In-memory storage (dictionary) — no external database required

---

## 🛠️ Tech Stack
- **Python 3**
- **Flask**
- **Postman** or **cURL/PowerShell** for testing

---

## Installation and Setup
1. Clone this repository:
```bash
git clone https://github.com/Dhruv-Dhameliya/BH-Python-D4-RestAPI.git
cd BH-Python-D4-RestAPI
```

2. Install dependencies:
```bash
pip install flask
```

3. Run the file:
```bash
python restapi.py
```

The server will start at:
`http://127.0.0.1:5000`

---

## API Handeling
1. Create User (POST)
```powershell
Invoke-RestMethod -Uri "http://127.0.0.1:5000/users" `
  -Method POST `
  -Headers @{ "Content-Type" = "application/json" } `
  -Body '{"id":1,"name":"Amitabh"}'
```

2. Get All Users (GET)
```powershell
Invoke-RestMethod -Uri "http://127.0.0.1:5000/users" -Method GET
```

3. Update User (PUT)
```powershell
Invoke-RestMethod -Uri "http://127.0.0.1:5000/users/1" `
  -Method PUT `
  -Headers @{ "Content-Type" = "application/json" } `
  -Body '{"name":"Ajay"}'
```

4. Delete User (DELETE)
```powershell
Invoke-RestMethod -Uri "http://127.0.0.1:5000/users/1" -Method DELETE
```
---
