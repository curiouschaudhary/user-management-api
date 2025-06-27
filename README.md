User Management API
A RESTful Flask API for managing users with JSON storage.

https://img.shields.io/badge/Python-3.8%252B-blue
https://img.shields.io/badge/Flask-2.0%252B-lightgrey
https://img.shields.io/badge/License-MIT-green

📌 Overview
This project is a Flask-based REST API that allows you to:
✅ Create, Read, Update, Delete (CRUD) users
✅ Search users by name
✅ Store data in a JSON file (data.json)
✅ Simple, lightweight, and easy to extend

🚀 Features
Endpoint	Method	Description
/	GET	Welcome page (API docs)
/users	GET	List all users
/users	POST	Add a new user
/users/<user_id>	GET	Get a single user by ID
/users/<user_id>	PUT	Update a user by ID
/users/<user_id>	DELETE	Delete a user by ID
/search?name=<name>	GET	Search users by name (case-insensitive)
/count	GET	Get total number of users
🛠️ Setup & Installation
1. Clone the Repository
sh
git clone https://github.com/yourusername/flask-user-api.git
cd flask-user-api
2. Install Dependencies
sh
pip install flask
3. Run the API
sh
python app.py
➡️ Access the API at: http://127.0.0.1:5000

📝 API Usage Examples
Create a User (POST)
sh
curl -X POST http://127.0.0.1:5000/users \
  -H "Content-Type: application/json" \
  -d '{"name": "John Doe", "email": "john@example.com", "age": 30, "phone": "+1234567890"}'
Response:

json
{
  "message": "User created",
  "user_id": 1
}
Get All Users (GET)
sh
curl http://127.0.0.1:5000/users
Response:

json
{
  "1": {
    "name": "John Doe",
    "email": "john@example.com",
    "age": 30,
    "phone": "+1234567890"
  }
}
Search Users (GET)
sh
curl http://127.0.0.1:5000/search?name=john
🔧 Project Structure
text
flask-user-api/
├── app.py           # Main Flask application
├── data.json        # Database (auto-created)
└── README.md        # This file
📜 License
This project is licensed under the MIT License. See LICENSE for details.

![screenshot](https://github.com/user-attachments/assets/3f3956af-f02f-4c3e-b0c1-c03b4fb859cc)


🤝 Contributing
Feel free to:

Report bugs (Open an Issue)

Suggest features (Submit a Pull Request)

📬 Contact
👤 Vineet Kumar Chaudhary
📧 chaudharyvineet730@gmail.com
🌐 https://github.com/curiouschaudhary

✨ Happy Coding!
Give it a ⭐ if you found this useful! 🚀

