# **Backend API for Form Submission and Data Storage**

This Node.js backend application serves as an API to handle form submissions, retrieve data from an external server, and save the submitted data into a MongoDB database.

## **Table of Contents**
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [API Endpoints](#api-endpoints)
- [Environment Variables](#environment-variables)
- [How It Works](#how-it-works)
- [License](#license)

---

## **Project Overview**
This backend handles form submissions and stores the data in a MongoDB database. The form data is submitted from a frontend or external service, processed on the backend, and then saved in MongoDB. The backend listens on **port 8000**.

When the form is submitted:
1. The backend receives the data.
2. It communicates with an external server to gather additional information (if required).
3. The complete form data is then stored in the **MongoDB** database.

---

## **Technologies Used**
- **Node.js**: JavaScript runtime environment.
- **Express.js**: Fast, unopinionated web framework for Node.js.
- **MongoDB**: NoSQL database used for data storage.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB and Node.js.
- **Axios**: HTTP client for making requests to external APIs.
- **dotenv**: To manage environment variables.

---

## **Setup and Installation**

### **1. Clone the repository**
```bash
git clone https://github.com/your-repo-name.git
cd your-repo-name
```
### **2. Install Dependencies**
```bash
npm install
```
### **3. Set up the environment variables**
```bash
MONGODB_USERNAME=<your-mongodb-username>
MONGODB_PASSWORD=<your-mongodb-password>
CONNECTION_STRING='mongodb+srv://<username>:<password>@cluster0.mongodb.net/myFirstDatabase?retryWrites=true&w=majority'
PORT=8000
```
### **4. Start the server**
```bash
npm start
```