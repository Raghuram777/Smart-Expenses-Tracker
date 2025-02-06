# 💼 Family Expense Tracker

A **smart and collaborative expense tracking** web app where multiple family members can track their spending, set budgets, and gain AI-powered financial insights.

---

## 📝 Features

### 🌟 **Core Features**
- **Multi-User Family Accounts** – Create a family group and invite members to join.
- **Role-Based Access** – Assign members as "Admin" or "Member".
- **Expense Management** – Add, edit, delete expenses with categories.
- **Monthly Budgeting** – Set budget limits and get spending alerts.
- **AI-Powered Insights** – Get AI-driven savings recommendations.
- **Real-Time Expense Sharing** – Family members see updates instantly.
- **Charts & Reports** – Visualize spending trends with interactive graphs.
- **Expense Splitting** – Automatically split shared expenses among family members.
- **Export Data** – Download reports in CSV or PDF format.

### 🔒 **Security & Authentication**
- **Secure User Authentication** – Firebase authentication (Email & Google Login).
- **JWT-Based API Security** – Protects backend endpoints.

### 🌐 **Deployment & Accessibility**
- **Mobile-Responsive UI** – Works seamlessly on any device.
- **Cloud Deployment** – Hosted on Vercel (Frontend) & Render (Backend).

---

## 🛠️ Tech Stack

### **Frontend:**
- React.js (with Redux for state management)
- Tailwind CSS (for styling)
- Chart.js / Recharts (for visualizing expenses)

### **Backend:**
- Spring Boot (REST API)
- PostgreSQL (for data storage)
- Firebase Authentication (for secure login)

### **Deployment:**
- **Frontend:** Vercel / Netlify
- **Backend:** Render / AWS
- **Database:** Cloud PostgreSQL / Firebase Firestore

---

## 📈 Database Schema

### **Users Table**
| Column  | Type    | Description |
|---------|--------|-------------|
| id      | UUID   | Unique user ID |
| name    | String | User's full name |
| email   | String | User's email (unique) |
| family_id | UUID  | ID of the family the user belongs to |
| role    | String | 'Admin' or 'Member' |

### **Families Table**
| Column  | Type  | Description |
|---------|------|-------------|
| id      | UUID | Unique family ID |
| name    | String | Family group name |

### **Expenses Table**
| Column  | Type   | Description |
|---------|-------|-------------|
| id      | UUID  | Unique expense ID |
| user_id | UUID  | User who added the expense |
| family_id | UUID | Family the expense belongs to |
| amount  | Float | Expense amount |
| category | String | Expense category (Food, Rent, etc.) |
| date    | Date  | Date of expense |

---

## 📚 Installation Guide

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/yourusername/family-expense-tracker.git
cd family-expense-tracker
```

### **2️⃣ Install Dependencies**
#### **Frontend:**
```bash
cd frontend
npm install
```

#### **Backend:**
```bash
cd backend
mvn clean install
```

### **3️⃣ Configure Environment Variables**
Create a `.env` file in both `frontend` and `backend` directories with the required API keys.

### **4️⃣ Run the Application**
#### **Frontend:**
```bash
npm start
```
#### **Backend:**
```bash
mvn spring-boot:run
```

---

## 🎯 Roadmap
- [ ] Add AI-based savings goals
- [ ] Implement recurring expenses feature
- [ ] Integrate mobile push notifications

---

## 💎 Why Use This App?
✅ **Family-Friendly Collaboration** – Manage household finances **together**
✅ **AI-Powered Smart Insights** – Understand spending & get better **saving tips**
✅ **Secure & Private** – Your financial data is **fully protected**

---

## 👨‍💼 Contributing
We welcome contributions! Please follow these steps:
1. **Fork the repo**
2. **Create a feature branch** (`git checkout -b feature-name`)
3. **Commit your changes** (`git commit -m "Added new feature"`)
4. **Push and create a Pull Request**

---

## 🎬 Screenshots
Coming soon...

---

## 🛠 Support
For any issues, please open a GitHub **issue** or reach out to `support@example.com`.

---

## 🌟 License
MIT License. Free for everyone to use and modify!

---

🚀 **Happy Expense Tracking!**

