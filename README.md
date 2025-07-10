# 🛍️ Uplyft AI-Powered E-commerce Chatbot

A full-stack AI-assisted shopping chatbot application built with Django (backend) and vanilla HTML/CSS/JS (frontend). Users can chat to search products, filter by category/price, and view real-time results.

---

## ✨ Features

- 🔐 User sign-up & login system (frontend only using localStorage)
- 💬 Chat interface to search products
- 🎯 Product filtering by category and price
- 🖼️ Product listing with dynamic images
- 💾 Chat logs saved to Django backend
- 📦 Product data loaded from CSV file

---

## 🧠 Tech Stack

| Frontend     | Backend     | Database | Auth                 |
|--------------|-------------|----------|----------------------|
| HTML, CSS, JS| Django + DRF| SQLite   | localStorage (demo)  |

---

## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ecommerce-chatbot.git
cd ecommerce-chatbot
```

### 2. Backend Setup

```bash
cd backend
python -m venv venv
venv\Scripts\activate  # Windows
# OR
source venv/bin/activate  # macOS/Linux

pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py load_products
```

### 3. Start Backend Server

```bash
python manage.py runserver
```

Visit: http://127.0.0.1:8000/api/products/

---

### 4. Frontend Setup

Open `frontend/index.html` directly in your browser  
Or use VS Code Live Server

---

## 🧪 Demo Credentials

```text
Email: user@example.com
Password: test123
```

Or sign up via `signup.html`

---

## 🗂️ Project Structure

```
E-commerce_Chatbot/
├── backend/
│   ├── salesbot/
│   ├── mock_products_with_images.csv
│   └── manage.py
├── frontend/
│   ├── index.html
│   ├── login.html
│   ├── signup.html
│   ├── script.js
│   └── styles.css
```

---

## ✅ Sample API URL

Test this:
```
http://127.0.0.1:8000/api/products/?search=saree&price_lte=3000
```

---

## 🛠 Future Improvements

- Real user auth with Django
- Add cart & checkout system
- Use AI/NLP for natural language chat
- Connect to real e-commerce APIs

---

## 📄 License

This project is part of the **Uplyft Full Stack Internship Case Study**.