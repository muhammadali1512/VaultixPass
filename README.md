# 🔐 Vaultix — Password Manager Projects

> **From LocalStorage to MongoDB — Building Vaultix step by step.**

Welcome to the **Vaultix** project repository.

This repository contains **two versions** of my password manager project:

-  **Vaultix** — Version 1 using React, Tailwind CSS, and LocalStorage
-  **VaultixMongo** — Version 2 upgraded with Express.js and MongoDB

The purpose of this project is to demonstrate my progression from building a frontend-only application to developing a **full-stack MERN-style application**.

---

#  Projects

| Version | Project | Frontend | Storage | Backend |
|---|---|---|---|---|
| 01 |  VaultixPass | React + Tailwind CSS | LocalStorage | — |
| 02 |  VaultixMongo | React + Tailwind CSS | MongoDB | Express.js |

---

# 🔐 Version 1 — VaultixPass

**VaultixPass** is the first version of the password manager.

It focuses on building the complete frontend experience and storing credentials using the browser's `localStorage`.

###  Features

-  Save passwords
-  Store usernames
-  Store website URLs
-  Show / hide password
-  Copy credentials
-  Edit credentials
-  Delete credentials
-  LocalStorage persistence
-  Toast notifications
-  Responsive design
-  Tailwind CSS UI

###  Architecture

```text
        VaultixPass
             │
             ▼
        React.js
             │
             ▼
       Tailwind CSS
             │
             ▼
        LocalStorage
```

###  Technologies

- React.js
- Tailwind CSS
- JavaScript
- Vite
- React Toastify
- UUID
- LocalStorage

---

#  Version 2 — VaultixMongo

**VaultixMongo** is the second version of Vaultix.

The main goal of this version was to move from browser-based storage to a real backend and database.

###  Features

-  Save passwords
-  Store usernames
-  Store website URLs
-  Show / hide password
-  Copy credentials
-  Edit credentials
-  Delete credentials
-  MongoDB storage
-  REST API communication
-  Toast notifications
-  Responsive design
-  Tailwind CSS UI

###  Architecture

```text
              VaultixMongo
                   │
                   ▼
             React.js
                   │
                   ▼
           Tailwind CSS
                   │
              HTTP Requests
                   │
                   ▼
             Express.js
                   │
                   ▼
              MongoDB
```

###  Technologies

**Frontend**

- React.js
- Tailwind CSS
- JavaScript
- Vite
- React Toastify
- UUID

**Backend**

- Node.js
- Express.js
- REST API
- CORS

**Database**

- MongoDB

---

#  Repository Structure

```text
Vaultix/
│
├── VaultixPass/
│   │
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Manager.jsx
│   │   │   └── Footer.jsx
│   │   │
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── index.css
│   │   └── main.jsx
│   │
│   ├── package.json
│   ├── package-lock.json
│   ├── vite.config.js
│   └── README.md
│
│
├── VaultixMongo/
│   │
│   ├── backend/
│   │   ├── server.js
│   │   ├── package.json
│   │   └── package-lock.json
│   │
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Manager.jsx
│   │   │   └── Footer.jsx
│   │   │
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── index.css
│   │   └── main.jsx
│   │
│   ├── package.json
│   ├── package-lock.json
│   ├── vite.config.js
│   └── README.md
│
│
└── README.md
```

> `node_modules` and `.env` files are intentionally excluded from the repository.

---

#  Project Evolution

The Vaultix project was developed in stages.

## Version 1

```text
React
  │
  ▼
Tailwind CSS
  │
  ▼
LocalStorage
```


## Version 2

```text
React
  │
  ▼
Tailwind CSS
  │
  ▼
Express.js
  │
  ▼
MongoDB
```

This progression represents the move from a **frontend project** to a **full-stack application**.

---

#  CRUD Operations in VaultixMongo

VaultixMongo communicates with the Express.js backend through HTTP requests.

```text
GET
 │
 └── Fetch passwords

POST
 │
 └── Save password

DELETE
 │
 └── Delete password

UPDATE
 │
 └── Edit existing password
```

---

#  Password Management

Both versions provide a simple interface for managing credentials.

A credential contains:

```javascript
{
    site: "https://example.com",
    username: "username",
    password: "your-password",
    id: "unique-id"
}
```

Passwords are displayed in masked form:

```text
••••••••••
```

Users can copy the original password using the copy button.

> **Security note:** Password masking in the interface does not provide encryption. A production-ready password manager would require encryption, authentication, secure key management, and other security controls.

---

#  Responsive Design

Both versions are designed to work across different screen sizes.

```text
💻 Desktop
      │
      ▼
💻 Laptop
      │
      ▼
📱 Tablet
      │
      ▼
📱 Mobile
```

The password table supports horizontal scrolling on smaller screens to keep all important information accessible.

---

#  UI Highlights

Vaultix uses a consistent visual style across both versions:

-  Green-themed interface
-  Dark footer
-  Rounded input fields
-  Hover effects
-  Toast notifications
-  Copy icons
-  Edit icons
-  Delete icons
-  Password visibility control
-  Responsive layouts

---

#  Getting Started

## VaultixPass

Go to the project directory:

```bash
cd VaultixPass
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

---

## VaultixMongo

Go to the frontend:

```bash
cd VaultixMongo
```

Install dependencies:

```bash
npm install
```

Then install the backend dependencies:

```bash
cd backend
npm install
```

Make sure MongoDB is running and configure your `.env` file locally.

Start the backend:

```bash
npm run dev
```

Then start the frontend from the `VaultixMongo` directory:

```bash
npm run dev
```

---

# 📊 Project Comparison

| Feature | VaultixPass | VaultixMongo |
|---|---:|---:|
| React.js | ✅ | ✅ |
| Tailwind CSS | ✅ | ✅ |
| Responsive UI | ✅ | ✅ |
| Password Masking | ✅ | ✅ |
| Copy to Clipboard | ✅ | ✅ |
| Edit | ✅ | ✅ |
| Delete | ✅ | ✅ |
| Toast Notifications | ✅ | ✅ |


---

# 📌 Project Status

### 🔐 VaultixPass

```text
Frontend          ✅ Completed
React             ✅ Completed
Tailwind CSS      ✅ Completed
LocalStorage      ✅ Completed
Responsive UI     ✅ Completed
```

### 🚀 VaultixMongo

```text
Frontend          ✅ Completed
React             ✅ Completed
Tailwind CSS      ✅ Completed
Responsive UI     ✅ Completed
Express.js        ✅ Connected
REST API          ✅ Implemented
MongoDB           ✅ Connected
```


# 👨‍💻 Author

## Muhammad Ali

**Full Stack Developer | MERN Stack Developer**

I am building practical projects to strengthen my skills in modern web development and full-stack application development.

### Technologies

```text
React.js
Next.js
Node.js
Express.js
MongoDB
Tailwind CSS
JavaScript
C++
Git & GitHub
```

---

# 🌐 Connect With Me

### GitHub

[https://github.com/muhammadali1512](https://github.com/muhammadali1512)

### LinkedIn

[https://www.linkedin.com/in/muhammad-ali-0b126642a/](https://www.linkedin.com/in/muhammad-ali-0b126642a/)

---

#  Support

If you find the project interesting, consider giving the repository a ⭐ on GitHub.

Every project is another step toward becoming a better developer. 

---

# 🔐 Vaultix

> **Your passwords. Your control.**

### From Version 1 to Version 2

```text
VaultixPass
    ↓
LocalStorage
    ↓
VaultixMongo
    ↓
Express.js + MongoDB
```

**Built with ❤️ using React.js, Tailwind CSS, Express.js, and MongoDB.**
