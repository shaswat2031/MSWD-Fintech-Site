
---

# **SplitEasy: Simplifying Group Expenses and Personal Loans**

SplitEasy is a web application designed to simplify the management of group expenses, personal loans, and financial tracking for friends and small groups. The app provides easy-to-use tools and an AI-powered chatbot for splitting costs, tracking debts, and managing payments seamlessly.

## **Table of Contents**

1. [Introduction](#introduction)
2. [Features](#features)
   1. [Expense Splitting](#expense-splitting)
   2. [Loan Management Between Friends](#loan-management-between-friends)
   3. [AI Chatbot Integration](#ai-chatbot-integration)
   4. [Simple Credit Score](#simple-credit-score)
   5. [Seamless Payment Integration](#seamless-payment-integration)
3. [Tech Stack](#tech-stack)
   1. [Frontend](#frontend)
   2. [Backend](#backend)
   3. [AI Chatbot](#ai-chatbot)
4. [Monetization Strategy](#monetization-strategy)
5. [Folder Structure](#folder-structure)
   1. [Frontend Folder Structure](#frontend-folder-structure)
   2. [Backend Folder Structure](#backend-folder-structure)
6. [Installation and Setup](#installation-and-setup)
   1. [Frontend Setup](#frontend-setup)
   2. [Backend Setup](#backend-setup)
7. [Running the App](#running-the-app)
8. [Testing](#testing)
9. [Contributing](#contributing)
10. [License](#license)
11. [Acknowledgements](#acknowledgements)

---

## **Introduction**

SplitEasy is a web-based application created to solve the everyday problems people face when managing shared expenses and personal loans with friends or small groups. The app helps users effortlessly split expenses, track who owes what, manage small loans, and even integrate seamless payments—all with the help of an intuitive chatbot.

This project is a perfect blend of practical problem-solving, modern web technologies, and user-friendly design.

---

## **Features**

### **1. Expense Splitting**
- **Description**: Easily split shared expenses such as dinners, rent, or trips. The app calculates and displays who owes whom with precise amounts.
- **Group Tracking**: Perfect for group activities like vacations or shared housing where expenses need to be tracked and split.
- **Example**: *Mike paid Rs1000 for dinner; Anna and Joe need to pay their shares.*
- **Benefit**: Saves time and avoids awkward conversations about money.

### **2. Loan Management Between Friends**
- **Description**: Users can borrow money from friends and set repayment schedules. The app tracks loan amounts, repayment deadlines, and sends reminders.
- **Example**: *"You borrowed Rs500 from Sam. Repayment is due in 3 weeks."*
- **Benefit**: Helps manage small loans and maintain clear, transparent records.

### **3. AI Chatbot Integration**
- **Description**: The chatbot helps users manage finances through conversational commands. It can add expenses, check balances, and track loans.
- **Key Features**:
  - Add expenses: *"Add Rs200 for dinner with Mike."*
  - Check balances: *"How much do I owe Anna?"*
  - Track loans: *"Show my pending loans."*
- **Benefit**: Makes financial management effortless and intuitive, even for those unfamiliar with complex apps.

### **4. Simple Credit Score**
- **Description**: Users can build a basic credit score based on their repayment history. Timely repayments increase the score, while delays can reduce it.
- **Benefit**: Encourages responsible financial behavior, promotes trust between users, and gamifies the repayment process.

### **5. Seamless Payment Integration**
- **Description**: Direct payments can be made through the app using popular payment gateways like **PayPal**, **Stripe**, and **UPI**.
- **Example**: *"Pay Rs300 to Joe using UPI."*
- **Benefit**: Saves time by keeping all transactions within the app and ensures secure and quick payments.

---

## **Tech Stack**

### **Frontend**:
- **React.js**: For building a dynamic and responsive user interface.
- **Tailwind CSS**: Provides fast and clean styling for a modern, mobile-friendly design.
- **Chart.js**: Used to visualize expenses and balances through graphs and charts.

### **Backend**:
- **Node.js with Express.js**: Handles the app logic, routes, and API calls.
- **MongoDB**: Stores user data, expenses, loans, and credit scores.

### **AI Chatbot**:
- **Dialogflow or Rasa**: Powers the AI chatbot for natural language processing and interaction.

### **Payment Integration**:
- **Stripe/PayPal/UPI**: Securely processes payments.

### **Authentication**:
- **JWT (JSON Web Tokens)**: Ensures secure authentication and data protection.

---

## **Monetization Strategy**

1. **Subscription Model**:
   - Charge users **Rs100-150/month** for premium features, such as higher loan limits, advanced analytics, and priority support.
   
2. **Transaction Fees**:
   - Charge a small fee for processing payments and loan management.

---

## **Folder Structure**

### **Frontend Folder Structure**

```
frontend/
├── public/                 # Static files (index.html, favicon, etc.)
│   ├── index.html          # Main HTML file
│   └── assets/             # Images, icons, and other assets
├── src/
│   ├── components/         # Reusable UI components
│   │   ├── Expense/        # Components for the Expense feature
│   │   ├── Loan/           # Components for Loan feature
│   │   ├── Chatbot/        # Chatbot components
│   │   └── Shared/         # Shared components (Navbar, Footer, etc.)
│   ├── pages/              # Page-level components (Home, Dashboard, etc.)
│   ├── services/           # API call functions
│   ├── context/            # Context and state management
│   ├── styles/             # Global and reusable styles
│   ├── utils/              # Helper functions and utilities
│   ├── App.jsx             # Main React component
│   ├── index.jsx           # React entry point
│   └── config.js           # App configuration (API URLs)
├── package.json            # Dependencies and scripts
└── tailwind.config.js      # Tailwind CSS configuration file
```

### **Backend Folder Structure**

```
backend/
├── src/
│   ├── controllers/        # Business logic for handling routes
│   ├── routes/             # API routes
│   ├── models/             # MongoDB schemas
│   ├── middlewares/        # Middleware for authentication, validation, etc.
│   ├── config/             # Configuration files for DB, JWT, etc.
│   ├── utils/              # Helper functions
│   ├── app.js              # Express app setup
│   ├── server.js           # Server entry point
│   └── config.env          # Environment variables
├── tests/                  # Test files
├── package.json            # Dependencies and scripts
└── README.md               # Documentation
```

---

## **Installation and Setup**

### **Frontend Setup**

1. Clone the repository:
   ```bash
   git clone https://github.com/shaswat2031/SplitEasy.git
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the frontend:
   ```bash
   npm start
   ```

### **Backend Setup**

1. Clone the repository:
   ```bash
   git clone https://github.com/shaswat2031/SplitEasy.git
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the root of the backend folder and configure necessary variables (e.g., MongoDB URI, JWT secret).

4. Run the backend server:
   ```bash
   npm start
   ```

---

## **Running the App**

1. Start the backend server.
2. Start the frontend application.
3. Open the app in your browser at `http://localhost:3000` (or the appropriate URL).

---

## **Testing**

- Backend tests can be found in the `tests/` folder. Run them using:
  ```bash
  npm test
  ```

---

## **Contributing**

Contributions are welcome! Feel free to fork the repository and submit pull requests. Please follow the coding standards and add tests where necessary.

---

## **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## **Acknowledgements**

- **React** for building the frontend.
- **Node.js** and **Express.js** for the backend server.
- **MongoDB** for the database.
- **Tailwind CSS** for styling.
- **Dialogflow/Rasa** for the AI chatbot.

---
