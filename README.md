# 💸 Cashly V1.9

**Cashly V1.9** is a modern and secure **personal finance management web application** that allows users to manage income, expenses, and overall balance in one place.  
It provides a clean interface, reliable backend, and real-time financial tracking — all built with **Node.js**, **Express**, and **MongoDB**.

---

## 🚀 Features
- 🔐 Secure user registration and login using JWT authentication  
- 💰 Add, edit, and delete expenses or payments  
- 📊 Real-time balance updates  
- 🧾 Transaction history with categorized records  
- 📈 Simple analytics for income and expenses  
- 🖥️ Responsive design for desktop and mobile  

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/Cashly_V1.9.git
cd Cashly_V1.9
2️⃣ Backend Setup
bash
Kodu kopyala
cd backend
npm install
Create a .env file inside the backend directory:

env
Kodu kopyala
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
Start the backend server:

bash
Kodu kopyala
npm start
➡ The backend will run on http://localhost:5000

3️⃣ Frontend Setup
You can open the frontend directly or run it using a simple local server:

bash
Kodu kopyala
cd frontend
npx live-server
Then open http://localhost:8080 (or the port shown in your terminal) in your browser.

🧠 How to Use
Register for a new account

Log in to access your dashboard

Add income or expenses through the forms

Track your balance and view transaction history

Log out securely when finished

🧰 Technologies Used
Layer	Technologies
Frontend	HTML5, CSS3, JavaScript
Backend	Node.js, Express.js
Database	MongoDB (via Mongoose)
Authentication	JWT, bcrypt
Version Control	Git & GitHub

🧾 API Overview
Method	Endpoint	Description
POST	/api/register	Register a new user
POST	/api/login	Authenticate and return token
GET	/api/get-expenses	Retrieve user expenses
GET	/api/get-payments	Retrieve user payments
POST	/api/add-expense	Add an expense
POST	/api/add-payment	Add a payment
DELETE	/api/delete/:id	Delete a specific transaction

🔧 Environment Variables
Make sure to configure the .env file with the following values:

Variable	Description
MONGO_URI	MongoDB connection URL
JWT_SECRET	Secret key for JWT
PORT	Backend port number

🧭 Future Improvements
💹 Advanced financial charts and reports

💬 Email or notification alerts

🌙 Dark mode and visual themes

💱 Multi-currency and localization support

📜 License
This project is licensed under the MIT License.

⭐ If you like this project, consider giving it a star!
