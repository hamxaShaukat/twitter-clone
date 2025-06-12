# 🐦 Twitter Clone - Minimalist Microblogging Platform  
*A lightweight Next.js Twitter clone with text-only tweets, follows, and profile customization.*  


## ▶ **Video Demo**  
🎥 **[Watch Walkthrough](https://youtu.be/y5n5v_43y4I?feature=shared)** *(Show tweet posting, comments, and profile updates)*  

---

## ✨ **Key Features**  
- **Text-Only Tweets**: Post and delete your tweets (no media).  
- **Interactions**: Like tweets, comment, and delete comments.  
- **Follow System**: Follow/unfollow other users.  
- **Profile Customization**:  
  - Update profile picture, cover photo, bio, and DOB.  
- **Future Improvements**:  
  - Search functionality.  
  - User suggestions based on bio/keyword matching.
- **Notifications**:  
  - Simple notification is implemented for like/follow functionality.  

---

## 🛠️ **Tech Stack**  
- **Frontend**: Next.js, TailwindCSS  
- **Backend**: Next.js API Routes  
- **Database**: MongoDB (Prisma orm)  
- **Auth**: NextAuth.js (JWT)  
- **State Management**: Zustand  

---

## 🚀 **Local Setup**  

### **1. Clone & Install**  
```bash
git clone https://github.com/hamxaShaukat/twitter-clone.git
cd twitter-clone
npm install
```

### **2. Environment Variables**  
Create a `.env` file in the root and add:  

```env
NEXTAUTH_JWT_SECRET="your_jwt_secret"
NEXTAUTH_SECRET="your_nextauth_secret"
DATABASE_URL="mongodb_connection_uri"
```

#### 🔑 **How to Get These Keys**  
- **NextAuth Secrets**:  
  Generate via terminal:  
  ```bash
  openssl rand -base64 32  # For NEXTAUTH_JWT_SECRET and NEXTAUTH_SECRET
  ```  
- **MongoDB URI**:  
  Create a free cluster on [MongoDB Atlas](https://www.mongodb.com/atlas/database).  

### **3. Run the App**  
```bash
npm run dev
```
Open `http://localhost:3000` in your browser.  

---

## 🛑 **Planned Improvements**  
- [ ] **Search**: Find users/tweets by keywords.  
- [ ] **Suggestions**: Recommend users based on bio/activity.  
- [ ] **Notifications**: Real-time like/comment alerts.  

---


## 💡 **Challenges & Solutions**  
- **Challenge**: Real-time comment updates.  
  **Solution**: Used MongoDB change streams to refresh the UI.  
- **Challenge**: Follow system scalability.  
  **Solution**: Optimized DB queries with indexing.  

---

## 📜 **License**  
MIT  

## 📩 **Contact**  
Email: **hamzashaukat714@gmail.com**
