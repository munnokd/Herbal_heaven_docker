# 🌿 Herbal Heaven - E-commerce Platform (Dockerised)

Herbal Heaven is a full-stack e-commerce platform for selling herbal products, built with Node.js, Express, MongoDB Atlas, and Materialize CSS. This version includes Docker and Docker Compose configuration for containerized development and testing environments.

---

## 🐳 Docker Instructions

To run this application in a Docker container:

### ✅ Step 1: Clone the Repository

```bash
git clone https://github.com/munnokd/Herbal_heaven_docker.git
cd Herbal_heaven_docker
```

### ✅ Step 2: Run with Docker Compose

```bash
docker-compose up --build
```

### ✅ Step 3: Stop All Containers

```bash
docker-compose down
```

---

## 🌐 Accessing the App

After running the container, open your browser and navigate to:

- **Main App**: [http://localhost:3000](http://localhost:3000)
- **Student API Endpoint**: [http://localhost:3000/api/student](http://localhost:3000/api/student)

---

## 🎓 API Identity Endpoint

To verify the individual contribution, this Dockerised app includes a REST API route at `/api/student` that returns the following JSON:

```json
{
  "name": "Kalp Prajapati",
  "studentId": "224834542"
}
```

---

## 📦 Features

- **User Authentication**: Register, login, role-based access, password reset
- **Product Management**: Search, filter, admin control, image uploads
- **Shopping Cart**: Add/update/remove, promo codes, persistent cart
- **Checkout**: Stripe integration, payment options, confirmations
- **Order Management**: Order tracking, invoices, shipping updates
- **Blog System**: Articles, categories, comments, likes
- **Admin Dashboard**: Analytics, content & inventory management

---

## 🧱 Docker Compose Setup

This setup runs the app and test services using MongoDB Atlas as the remote database.

### 🔧 Prerequisites

Ensure the app uses `process.env.MONGO_URI` to connect to MongoDB.

### 🔧 Run All Services

```bash
docker-compose up --build
```

### ❌ Tear Down Services

```bash
docker-compose down
```

### 📡 Services Included

- `app`: Node.js Express backend + frontend static assets
- `test`: Test runner service
- `herbal_net`: Docker internal network

---

## 🛠 Tech Stack

**Frontend**: HTML5, CSS3 (Materialize), JS  
**Backend**: Node.js, Express, MongoDB, Mongoose  
**Auth**: JWT, bcrypt  
**Payments**: Stripe  
**Media**: Cloudinary, Multer  
**Mail**: Nodemailer  

---

## 📁 Project Structure

[Content omitted for brevity — same as your original readme project structure section]

---

## 🔐 Environment Variables

Create a `.env` file with:
```
NODE_ENV=development
PORT=3000
MONGO_URI=mongodb+srv://kalp2002prajapati:yourpassword@cluster0.xfojzlh.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_key
...
```

---

## 🚀 Running Locally (Non-Docker Option)

```bash
npm install
npm run dev
```

---

## 🧪 API Documentation

API endpoints available at `/api-docs` (if configured)

[Your full endpoint list remains unchanged — not repeated here]

---

## 🤝 Contributing

[Same content as your original]

---

## 📜 License

MIT License

---

## 🙏 Acknowledgments

- MongoDB Atlas
- Stripe
- Materialize CSS
- Cloudinary
- Docker & Compose
