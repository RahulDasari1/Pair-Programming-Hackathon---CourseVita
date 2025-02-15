# 📚 **Book Sharing Platform**  
_A peer-to-peer web application for book lovers to lend, exchange, and chat with local readers._  

![Book Sharing Platform](https://cdn.pixabay.com/photo/2017/06/30/22/38/books-2458025_1280.jpg)  

---

## **🚀 Features**
✅ **List & Find Books** – Users can list books they own and find books available nearby.  
✅ **Geolocation & Maps** – Google Maps integration to locate book-sharing partners.  
✅ **Real-Time Chat** – Built-in messaging using Socket.io.  
✅ **User Authentication** – Secure login & registration with JWT.  
✅ **Ratings & Reviews** – Rate users after book exchanges.  

---

## **🛠️ Tech Stack**
| Layer      | Technology   |
|------------|-------------|
| Frontend   | React.js (Material UI, TailwindCSS) |
| Backend    | Node.js, Express.js |
| Database   | MongoDB (Mongoose ORM) |
| Authentication | JWT (JSON Web Token) |
| Maps & Location | Google Maps API, Geolocation API |
| Messaging | Socket.io for real-time chat |
| Deployment | Vercel (Frontend), Render (Backend) |

---

## **📂 Project Structure**
```
📦 book-sharing-platform
 ┣ 📂 backend
 ┃ ┣ 📂 models
 ┃ ┃ ┣ 📜 User.js
 ┃ ┃ ┣ 📜 Book.js
 ┃ ┣ 📂 routes
 ┃ ┃ ┣ 📜 auth.js
 ┃ ┃ ┣ 📜 books.js
 ┃ ┣ 📜 server.js
 ┃ ┣ 📜 .env
 ┃ ┣ 📜 package.json
 ┣ 📂 frontend
 ┃ ┣ 📂 src
 ┃ ┃ ┣ 📂 components
 ┃ ┃ ┃ ┣ 📜 BookList.js
 ┃ ┃ ┃ ┣ 📜 Chat.js
 ┃ ┃ ┃ ┣ 📜 MapComponent.js
 ┃ ┃ ┣ 📂 pages
 ┃ ┃ ┃ ┣ 📜 Register.js
 ┃ ┃ ┃ ┣ 📜 Login.js
 ┃ ┃ ┣ 📜 App.js
 ┃ ┃ ┣ 📜 index.js
 ┃ ┣ 📜 package.json
 ┣ 📜 README.md
```

---

## **🛠️ Setup Instructions**
### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/RahulDasari1/book-sharing-platform.git
cd book-sharing-platform
```

### **2️⃣ Backend Setup**
```bash
cd backend
npm install
```
Create a `.env` file in `backend/`:
```
MONGO_URI = your_mongodb_connection_string
JWT_SECRET = your_jwt_secret
```
Start the server:
```bash
node server.js
```

### **3️⃣ Frontend Setup**
```bash
cd frontend
npm install
```
Update **Google Maps API Key** in `src/components/MapComponent.js`:
```js
<LoadScript googleMapsApiKey="YOUR_GOOGLE_MAPS_API_KEY">
```
Start the frontend:
```bash
npm start
```

---

## **📡 Deployment**
### **🚀 Deploy Backend to Render**
1. Create a **[Render](https://render.com/)** account.
2. Click **New Web Service** → **Connect GitHub Repo** or **Upload Code**.
3. Add environment variables in **Render dashboard**:
   ```
   MONGO_URI = your_mongodb_connection_string
   JWT_SECRET = your_jwt_secret
   ```
4. Deploy & get backend URL (e.g., `https://book-share-backend.onrender.com`).

### **🚀 Deploy Frontend to Vercel**
1. Install **Vercel CLI**:
   ```bash
   npm install -g vercel
   ```
2. Deploy:
   ```bash
   cd frontend
   vercel
   ```
3. Get frontend URL (e.g., `https://book-share.vercel.app`).

---

## **📝 API Endpoints**
### **User Authentication**
| Method | Endpoint | Description |
|--------|----------|------------|
| POST   | `/auth/register` | Register new user |
| POST   | `/auth/login` | Login user |

### **Book Management**
| Method | Endpoint | Description |
|--------|----------|------------|
| POST   | `/books/add` | Add a new book |
| GET    | `/books/nearby?lat={latitude}&lng={longitude}` | Get books nearby |

---

## **🎨 Screenshots**
| Home Page | Chat System |
|-----------|------------|
| ![Home Page](https://via.placeholder.com/400) | ![Chat System](https://via.placeholder.com/400) |

---

## **👨‍💻 Contributing**
🙌 Contributions are welcome!  
1. **Fork the repo**  
2. **Create a feature branch** (`git checkout -b feature-name`)  
3. **Commit changes** (`git commit -m "Added feature XYZ"`)  
4. **Push to GitHub** (`git push origin feature-name`)  
5. **Create a Pull Request**  

---

## **🛡️ License**
📜 MIT License – Free to use & modify.  

---

## **📞 Contact**
📧 **Email:** [dasarirahulpatel.drp@gmail.com](mailto:dasarirahulpatel.drp@gmail.com)  
👔 **LinkedIn:** [Rahul Dasari](https://www.linkedin.com/in/rahul-dasari-drp/)  
🐙 **GitHub:** [RahulDasari1](https://github.com/RahulDasari1)  

---

🚀 **Live Demo:** [https://book-share.vercel.app](https://book-share.vercel.app)  

---

🎉 **This README is ready for GitHub!** Would you like me to generate a **logo for your project** or help with **GitHub repository setup**? 😊
