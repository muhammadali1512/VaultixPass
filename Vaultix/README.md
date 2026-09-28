# 🔐 VaultixPass

> **Your Own Password Manager**

VaultixPass is a modern and responsive password manager built with **React.js** and **Tailwind CSS**. It provides a clean interface for securely managing website credentials, with features like password masking, copy-to-clipboard, editing, deleting, and persistent local storage.

**Express.js + MongoDB integration is coming soon in 2nd version - VaultixMongo.**

---

## Features

-  Save website credentials
-  Store usernames
-  Store passwords securely in masked form
-  Show / hide password while entering
-  Copy website, username, and password with one click
-  Edit saved credentials
-  Delete credentials with confirmation
-  Persistent data using browser `localStorage`
-  Responsive design for desktop and mobile
-  Attractive toast notifications
-  Modern UI built with Tailwind CSS
-  Fast and smooth React interface

---

##  Tech Stack

### Frontend

-  React.js
-  Tailwind CSS
-  React Toastify
-  UUID
-  JavaScript
-  Vite

### Current Storage

-  Browser LocalStorage

### Coming Soon

-  Express.js
-  MongoDB
-  REST API
-  Backend-based password management

---

##  Project Preview

### VaultixPass

VaultixPass provides a simple dashboard where you can add and manage your credentials.

**Main interface includes:**

- Website URL input
- Username input
- Password input
- Show/hide password button
- Save Password button
- Saved passwords table
- Copy buttons
- Edit button
- Delete button

---

##  Project Structure

```text
VaultixPass/
│
├── public/
│   ├── copy.gif
│   ├── doodle-motif-49-plus-circle-hover-pinch (1).gif
│   ├── eyecross.png
│   ├── system-solid-35-pencil-hover-pinch.gif
│   ├── system-solid-69-eye-hover-pinch.gif
│   └── system-solid-185-trash-bin-hover-pinch.gif
│
├── src/
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── Manager.jsx
│   │   └── Footer.jsx
│   │
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
│
├── package.json
├── vite.config.js
└── README.md
```

---

##  Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/muhammadali1512/VaultixPass.git
```

### 2. Open the project

```bash
cd Vaultix
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

Open the local development URL shown in your terminal.

---

##  How It Works

VaultixPass stores password entries in the browser's `localStorage`.

Each saved credential contains:

```javascript
{
    site: "https://example.com",
    username: "username",
    password: "your-password",
    id: "unique-id"
}
```

When a password is saved, VaultixPass generates a unique ID using `UUID` and stores the updated password array in LocalStorage.

---

##  Password Protection

Passwords are not displayed as plain text in the password table.

Instead, VaultixPass displays password bullets:

```text
••••••••••
```

Users can still copy the original password directly using the copy button.

---

##  Copy to Clipboard

VaultixPass allows users to quickly copy:

- Website URL
- Username
- Password

The Clipboard API is used to copy the selected value:

```javascript
navigator.clipboard.writeText(text);
```

A toast notification is displayed after copying.

---

##  Edit Credentials

Clicking the edit icon loads the selected credential back into the form so it can be modified.

After editing, the credential can be saved again.

---

##  Delete Credentials

Users can delete individual credentials from VaultixPass.

Before deletion, the application asks for confirmation:

```text
Do you really want to delete this password?
```

After deletion, the updated data is saved back to LocalStorage.

---

##  Responsive Design

VaultixPass is designed to work across different screen sizes.

The password table uses horizontal scrolling on smaller screens so that important columns remain accessible.

Supported layouts include:

- 💻 Desktop
- 💻 Laptop
- 📱 Tablet
- 📱 Mobile

---

##  UI Highlights

VaultixPass uses a clean green-themed interface with:

- Rounded input fields
- Responsive tables
- Gradient-style background effects
- Interactive icons
- Toast notifications
- Hover effects
- Mobile-friendly&#x20;

---

## 🧑‍💻 Author

### Muhammad Ali

**Full Stack Developer | MERN Stack Developer**

I am currently building my skills in modern web development with a focus on creating practical and real-world applications.

### Tech I am working with

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

## 🌐 Connect With Me

**GitHub:**
[https://github.com/muhammadali1512](https://github.com/muhammadali1512)

**LinkedIn:**
[https://www.linkedin.com/in/muhammad-ali-0b126642a/](https://www.linkedin.com/in/muhammad-ali-0b126642a/)

---

##  Support

If you find VaultixPass interesting, consider giving the repository a ⭐ on GitHub.

Your support motivates me to keep learning and building 

---

## 📌 Project Status

```text
Frontend       ✅ Completed
React          ✅ Completed
Tailwind CSS   ✅ Completed
LocalStorage   ✅ Completed
Responsive UI  ✅ Completed

```

> 🚀 **VaultixPass is an ongoing project. The complete full-stack version with Express.js and MongoDB will be coming soon.**

---

### 🔐 VaultixPass

**Manage your passwords. Keep your credentials organized.**

Built with ❤️ using React.js and Tailwind CSS.
