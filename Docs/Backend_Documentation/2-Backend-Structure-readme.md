# ༺♦ Dawaya Backend Project Structure ♦༻

## Structure ⌗

```
Dawaya-app/
├── README.md
├── package.json
├── package-lock.json
├── .gitignore
├── index.js
├── vercel.json
├── node_modules/
├── database/
│   ├── models/
│   │   ├── user.model.js
│   │   ├── pharmacy.model.js
│   │   ├── pharmacist.model.js
│   │   ├── review.model.js
│   │   └── inventory.model.js
│   └── dbConnection.js
├── src/
│   ├── fileUpload/
│   │   └── fileUpload.js
│   ├── middlewares/
│   │   ├── catchError.js
│   │   ├── checkEmail.js
│   │   ├── globalError.js
│   │   ├── validate.js
│   │   └── verifyToken.js
│   ├── email/
│   │   ├── email.js
│   │   └── email.Html.js
│   ├── modules/
│   │   ├── user/
│   │   ├── auth/
│   │   ├── pharmacy/
│   │   ├── pharmacist/
│   │   ├── review/
│   │   ├── inventory/
│   │   ├── medicine/
│   │   └── handler/
│   └── bootstrap.js
├── uploads/
│   ├── pharmacy/
│   └── medicine/
├── utils/
│   ├── appError.js
│   └── cloud.js
└── config/
    └── .env
```

## 🚀 Features

- **User Management**: Create, update, and manage user accounts.
- **Pharmacy Management**: CRUD operations for pharmacy data.
- **Medication Inventory**: Track and manage medication stock across pharmacies.
- **Search and Filter**: Efficient search and filtering of medications and pharmacies.
- **Review System**: Allow users to leave reviews and ratings for pharmacies.
- **Authentication and Authorization**: Secure user authentication and role-based access control.
- **File Upload**: Handle image uploads for pharmacies and medications.
- **Email Notifications**: Send email notifications for various events.
- **Error Handling**: Centralized error handling and logging.
- **Database Integration**: MongoDB integration with Mongoose ODM.
- **API Documentation**: Swagger documentation for API endpoints.

## 🛠️ Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/Dawaya-Organization/Dawaya-backend.git
   ```

2. Install dependencies:

   ```bash
   cd Dawaya-backend
   npm install
   ```

3. Set up environment variables:

   - Copy `.env.example` to `.env` in the `config/` directory.
   - Update the variables as needed.

4. Run the development server:

   ```bash
   npm run dev
   ```

5. The server will start on `http://localhost:3000` (or the port specified in your .env file).

## 🧪 Testing

Run the test suite with:

```bash
npm test
```

## 🚢 Deployment

This project is configured for easy deployment on Vercel. Connect your GitHub repository to Vercel for automatic deployments on every push to the main branch.

For other deployment options, refer to the deployment documentation for Node.js applications.

## 🔑 Environment Variables

Ensure the following environment variables are set in your `.env` file:

- `PORT`: The port number for the server to listen on
- `MONGODB_URI`: MongoDB connection string
- `JWT_SECRET`: Secret key for JWT token generation
- `EMAIL_USER`: Email address for sending notifications
- `EMAIL_PASS`: Password for the email account
- `CLOUD_NAME`: Cloudinary cloud name for image uploads
- `API_KEY`: Cloudinary API key
- `API_SECRET`: Cloudinary API secret

## 🧩 Tech Stack

- **Node.js**: JavaScript runtime for server-side development
- **Express.js**: Web application framework for Node.js
- **MongoDB**: NoSQL database for data storage
- **Mongoose**: ODM library for MongoDB and Node.js
- **JSON Web Token (JWT)**: For secure authentication
- **Bcrypt**: Password hashing library
- **Multer**: Middleware for handling file uploads
- **Nodemailer**: Module for sending emails
- **Joi**: Object schema validation
- **Cloudinary**: Cloud service for image and video management
- **Swagger**: API documentation tool

## 📚 Learn More

To learn more about the technologies used in this project, check out the following resources:

- [Node.js Documentation](https://nodejs.org/en/docs/)
- [Express.js Documentation](https://expressjs.com/)
- [MongoDB Documentation](https://docs.mongodb.com/)
- [Mongoose Documentation](https://mongoosejs.com/docs/guide.html)
- [JWT.io](https://jwt.io/)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/Dawaya-Organization/Dawaya-info/blob/main/LICENSE) file for details.
