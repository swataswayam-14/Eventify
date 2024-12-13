# 🎉 Eventify: Event Management Backend API 🚀

Eventify is a **scalable** and **modular** backend API designed to simplify event management, bookings, and payments. It provides features like **secure user authentication**, **real-time seat availability**, **automated email notifications**, and **payment integration** (Razorpay coming soon).

---

## 📑 Table of Contents
- [⚙️ Installation](#%EF%B8%8F-installation)
- [🎯 Usage Instructions](#-usage-instructions)
- [🚀 Features](#-features)
- [💻 Technologies Used](#-technologies-used)
- [🚀 Future Improvements](#-future-improvements)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ⚙️ Installation

```bash
# 1️⃣ Clone the Repository  
git clone https://github.com/yourusername/eventify.git  
cd eventify  

# 2️⃣ Install Dependencies  
npm install  

# 3️⃣ Set Up Environment Variables  
# Create a .env file in the root directory and add the following:
PORT=<your-port-number>  
URL=<your-mongodb-uri>  
JWT_KEY=<your-jwt-secret-key>  
EMAIL_ID=<your-email-id>  
EMAIL_PASSWORD=<your-email-password>  
RAZORPAY_KEY_ID=<your-razorpay-key-id>  
RAZORPAY_KEY_SECRET=<your-razorpay-key-secret>  

# 4️⃣ Database Setup  
# Ensure MongoDB is running locally or use MongoDB Atlas.  
# Collections (Users, Events, Bookings, Payments) are auto-created on server start.

# 5️⃣ Run the Server  
node server.js  

# 6️⃣ Run the Server in Development Mode  
# Use nodemon for automatic restarts during development.  
nodemon server.js  

## 🎯 Usage Instructions

1. **Register or Login:**  
   - Users can register and log in to explore available events. Use the `/register` and `/login` endpoints for this process.

2. **Admin Actions:**  
   - Admins have exclusive access to create, update, and delete events via the `/admin/events` endpoint.  
   - Admins can also manage bookings and payments.

3. **Book Events:**  
   - Users can browse events and book tickets using the `/events` and `/book` endpoints.  
   - Seat availability is checked in real-time to ensure no overbooking.

4. **Email Notifications:**  
   - Once a user successfully books an event, they will receive a confirmation email with details. This is managed by Nodemailer.

5. **Payments (Coming Soon):**  
   - Razorpay payment integration 


## 🚀 Features

- 🔒 **Secure Authentication:**  
  - User authentication is handled via **JWT** (JSON Web Tokens), ensuring secure and stateless sessions.

- 🎟️ **Event Management:**  
  - Admins can **create**, **update**, and **delete** events through the admin panel.  
  - Users can browse a list of events and check detailed information.

- ⚡ **Real-Time Seat Availability:**  
  - The system dynamically updates seat availability in real-time to prevent overbooking and ensure accurate booking status.

- 🛡️ **Role-Based Access Control:**  
  - The application has separate roles for **users** and **admins**, ensuring secure and efficient operations.  
  - Admins have exclusive access to manage events, bookings, and payments.

- 💳 **Payment Gateway Integration (Coming Soon):**  
  - Razorpay integration (to be completed) for secure and seamless payment processing for event bookings.

- 📧 **Email Notifications:**  
  - **Nodemailer** is integrated to send automated transactional emails for booking confirmations and updates.

- ✅ **Data Validation:**  
  - **Zod** is used to validate input data, ensuring that only correct and valid data enters the system.

- 🔐 **Password Security:**  
  - User passwords are securely hashed using **bcrypt**, ensuring sensitive information is stored safely.

- 📈 **Scalable Design:**  
  - The modular architecture is designed for easy expansion, allowing new features to be added effortlessly.

--- 
## 💻 Technologies Used

| **Category**         | **Technology**         |  
|----------------------|------------------------|  
| **Backend Framework** | Node.js + Express.js   |  
| **Database**          | MongoDB + Mongoose     |  
| **Authentication**    | JWT (JSON Web Tokens)  |  
| **Validation**        | Zod                    |  
| **Password Hashing**  | Bcrypt                 |  
| **Email Notifications**| Nodemailer             |  
| **Payment Gateway**   | Razorpay (WIP)         |  
| **Deployment**        | Cloud Service (WIP)    |
  

## 🚀 Future Improvements

1. **Razorpay Integration:**  
   - Complete the integration of Razorpay for secure payment processing to handle event bookings seamlessly.

2. **Cloud Deployment:**  
   - Deploy the API to cloud platforms like **AWS**, **Heroku**, or **Vercel** to make the system production-ready and globally accessible.

3. **Advanced Admin Tools:**  
   - Implement advanced features for admins, such as **analytics**, **event insights**, and detailed **booking reports** to enhance decision-making.

4. **Frontend Development:**  
   - Build a user-friendly frontend to complement the backend, providing a seamless experience for both users and admins.

5. **Event Recommendations:**  
   - Implement an intelligent **recommendation system** for users based on their previous bookings or preferences.

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can contribute:

1. **Fork the Repository:**  
   - Click the "Fork" button at the top-right of the repository page to create a copy under your own GitHub account.

2. **Create a Branch:**  
   - Use `git checkout -b feature-name` to create a new branch for your feature.

3. **Make Changes:**  
   - Implement your feature or fix the bug. Write clear, concise commit messages.

4. **Commit Your Changes:**  
   - Use `git commit -m "Add feature-name"` to commit your changes.

5. **Push to Your Branch:**  
   - Push your changes to your forked repository using `git push origin feature-name`.

6. **Open a Pull Request:**  
   - Go to the original repository and click on "New Pull Request" to submit your changes for review.

---

We appreciate all kinds of contributions, including **bug fixes**, **feature suggestions**, and **documentation improvements**. If you encounter any issues or have ideas for new features, please open an **issue** or **pull request** in the repository.

---

## 🎉 Conclusion

Eventify is designed to make event management seamless, scalable, and efficient. With robust features, flexible architecture, and an active community, we're excited to see how you contribute to making Eventify the go-to solution for event-driven applications. Join us in building the future of event management! 🚀

