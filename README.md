# 📚 Library Management System

A RESTful Library Management System built using **Node.js**, **Express.js**, **MongoDB**, and **Mongoose**. This project provides APIs to manage books in a library, including adding, viewing, updating, and deleting books with proper validation and HTTP status codes.

---

## 🚀 Features

- Add a new book
- View all books
- View a single book by ID
- Update book details
- Delete a book
- Input validation
- Proper HTTP status codes
- MongoDB database integration
- RESTful API architecture

---

## 🛠️ Tech Stack

- **Backend:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB
- **ODM:** Mongoose
- **Testing Tool:** Thunder Client / Postman

---

## 📂 Project Structure

```
library-management-system/
│
├── controllers/
│   └── bookController.js
│
├── models/
│   └── Book.js
│
├── routes/
│   └── bookRoutes.js
│
├── config/
│   └── db.js
│
├── .env
├── server.js
├── package.json
└── README.md
```

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/library-management-system.git
```

### 2. Navigate to the project folder

```bash
cd library-management-system
```

### 3. Install dependencies

```bash
npm install
```

### 4. Create a `.env` file

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

### 5. Start the server

```bash
npm start
```

or

```bash
nodemon server.js
```

---

## 📖 API Endpoints

### Add Book

**POST**

```
/api/books
```

Example Request Body

```json
{
  "title": "The Alchemist",
  "author": "Paulo Coelho",
  "category": "Fiction",
  "isbn": "9780061122415",
  "availableCopies": 10
}
```

---

### Get All Books

**GET**

```
/api/books
```

---

### Get Book By ID

**GET**

```
/api/books/:id
```

---

### Update Book

**PUT**

```
/api/books/:id
```

Example Request Body

```json
{
  "title": "The Alchemist",
  "author": "Paulo Coelho",
  "category": "Novel",
  "isbn": "9780061122415",
  "availableCopies": 8
}
```

---

### Delete Book

**DELETE**

```
/api/books/:id
```

---

## 📚 Book Schema

| Field | Type | Required |
|--------|------|----------|
| title | String | Yes |
| author | String | Yes |
| category | String | Yes |
| isbn | String | Yes |
| availableCopies | Number | Yes |

---

## ✅ HTTP Status Codes

| Status Code | Description |
|-------------|-------------|
| 200 | Success |
| 201 | Created |
| 400 | Bad Request |
| 404 | Not Found |
| 500 | Internal Server Error |

---

## 🧪 Testing

You can test the APIs using:

- Thunder Client (VS Code)
- Postman

---

## 📌 Future Enhancements

- User Authentication (JWT)
- Borrow Book API
- Return Book API
- Search Books
- Pagination
- Role-Based Access Control
- Fine Calculation
- Due Date Tracking
---

## ⭐ Conclusion

The Library Management System is a simple REST API project that demonstrates CRUD operations using Node.js, Express.js, MongoDB, and Mongoose. It provides a strong foundation for building more advanced library management applications with authentication, book borrowing, and user management features.
