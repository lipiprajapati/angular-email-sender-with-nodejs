# Angular Email Sender with Node.js

This repository contains a full-stack application that demonstrates how to send emails from an Angular frontend using a Node.js backend and Nodemailer.

---

## 🚀 Features
- **Angular Material UI**: Clean and responsive user interface for composing emails.
- **Node.js & Express**: A lightweight server to handle email requests.
- **Nodemailer**: Integrated SMTP transport for reliable email delivery.
- **CORS Enabled**: Ready for cross-origin communication between frontend and backend.

---

## 🛠️ Tech Stack
- **Frontend**: Angular 
- **Backend**: Node.js, Express.js
- **Email Library**: Nodemailer

---

## 📂 Project Structure
```text
angular-email-sender-with-nodejs/
├── backend/            # Express Server
│   ├── app.js          # Main API logic
│   └── package.json    # Backend dependencies
└── frontend/           # Angular App
    ├── src/            # Angular source files
    └── package.json    # Frontend dependencies
```
---

## 🔧 Getting Started

### Prerequisites
- [Node.js (LTS version)](https://nodejs.org/)
- [Angular CLI](https://angular.io/cli) (`npm install -g @angular/cli`)

### 1. Clone the Repository
```bash
git clone [https://github.com/lipiprajapati/angular-email-sender-by-nodejs.git](https://github.com/lipiprajapati/angular-email-sender-by-nodejs.git)
cd angular-email-sender-by-nodejs
```
### 2. Backend Setup (Node.js)

Navigate to the backend folder and install dependencies:
```bash
cd backend
npm install
```
Configure your email credentials: Open app.js (or your config file) and update the Nodemailer transporter with your details:

```javaScript

const transporter = nodemailer.createTransport({
  service: 'gmail',
  auth: {
    user: 'your-email@gmail.com',
    pass: 'your-app-password' // Use an App Password if using Gmail
  }
});
```

Start the server:
```bash
node server.js
```
The backend will typically run on http://localhost:3000.

### 3. Frontend Setup (Angular)

Navigate to the frontend folder and install dependencies:
```bash
cd ../frontend
npm install
```
Start the Angular app:
```bash
ng serve
```
Open your browser and navigate to http://localhost:4200.

---

### 📝 Usage

    Fill out the "To", "Subject", and "Message" fields in the web form.

    Click the Send button.

    The Angular app sends a POST request to the Node.js backend.

    The backend uses Nodemailer to dispatch the email and returns a success or error message.
    
---

### 🔒 Security Note

If you are using Gmail, you must use an App Password rather than your regular account password. Ensure "Less Secure Apps" access is handled or use OAuth2 for production environments.

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.



1.  **Fork** the Project.
2.  **Create** your Feature Branch:
    ```bash
    git checkout -b feature/AmazingFeature
    ```
3.  **Commit** your Changes:
    ```bash
    git commit -m 'Add some AmazingFeature'
    ```
4.  **Push** to the Branch:
    ```bash
    git push origin feature/AmazingFeature
    ```
5.  **Open** a Pull Request.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

### 👤 Author: **Lipi Prajapati**


---
