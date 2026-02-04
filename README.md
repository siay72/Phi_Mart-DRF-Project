# Phimart – Ecommerce API

Phimart is a full‑featured ecommerce backend built with Django Rest Framework (DRF). It provides RESTful API endpoints for managing products, categories, carts, and orders with secure JWT authentication and interactive API documentation.

---

## 🚀 Features

* Product and Category management APIs
* Shopping Cart functionality
* Order processing system
* JWT Authentication using **Djoser**
* Role‑based access control
* API documentation using **drf_yasg (Swagger UI)**
* Clean and scalable project structure
* Ready for frontend or mobile app integration

---

## 🛠 Technologies Used

* Python
* Django
* Django Rest Framework
* Djoser (JWT Authentication)
* drf_yasg (Swagger Documentation)
* SQLite / PostgreSQL

---

## 📁 Project Structure

```
phimart/
│── api/
│── products/
│── categories/
│── carts/
│── orders/
│── users/
│── config/
│── manage.py
│── requirements.txt
│── products/
│── README.md
```

---

## ⚙ Installation

### 1. Clone the repository

```
git clone <repository-url>
cd phimart
```

### 2. Create virtual environment

```
python -m venv env
source env/bin/activate   # On Windows: env\Scripts\activate
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

### 4. Apply migrations

```
python manage.py migrate
```

### 5. Create superuser

```
python manage.py createsuperuser
```

### 6. Run the server

```
python manage.py runserver
```

Server will start at:

```
http://127.0.0.1:8000/
```

---

## 🔐 Authentication

JWT authentication is implemented using **Djoser**.

### Register User

`POST api/auth/users/`

### Login

`POST api/auth/jwt/create/`

### Refresh Token

`POST api/auth/jwt/refresh/

Include the token in request headers:

```
Authorization: Bearer <your_token>
```

---

## 📌 API Endpoints

### Products

* `GET /api/products/` – List all products
* `POST /api/products/` – Create a product
* `GET /api/products/{id}/` – Product details
* `PUT /api/products/{id}/` – Update product
* `DELETE /api/products/{id}/` – Delete product

### Categories

* `GET /api/categories/`
* `POST /api/categories/`
* `GET /api/categories/{id}/`

### Cart

* `GET /api/cart/`
* `POST /api/cart/add/`
* `DELETE /api/cart/remove/`

### Orders

* `GET /api/orders/`
* `POST /api/orders/create/`

---

## 📄 API Documentation

Interactive API documentation is available using Swagger UI:

```
http://127.0.0.1:8000/swagger/
```

ReDoc documentation:

```
http://127.0.0.1:8000/redoc/
```

---

## 🧪 Testing

Run tests using:

```
python manage.py test
```

---

## 🌟 Future Improvements

* Payment gateway integration
* Product reviews and ratings
* Wishlist functionality
* Email notifications


---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 📜 License

This project is open source and available under the MIT License.

---

## 👨‍💻 Author

Developed by **Siam Hossain**

Feel free to contact for collaboration or feedback!
