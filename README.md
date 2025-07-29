# Wanderluster

Wanderluster is a modern, featured hotel listing and review platform built on the MongoDB, Express.js, Node.js. It allows users to explore hotels, leave reviews, and manage their own listings—all with secure authentication and user validation.

## 🚀 Features

🔐 User Authentication
  Sign up and log in securely using JWT.
  Protected routes for logged-in users only.

🏨 Hotel Listing Management
  Add new hotel listings with details like name, location, description, and image.
  Edit or delete listings—only by the user who created them.
  Validation to ensure no duplicate or invalid data is stored.

⭐ Review System
  Authenticated users can leave reviews on hotels.
  Users can edit or delete their own reviews only.

✅ Access Control & Validation
  All user actions (edit/delete) are validated against the logged-in user.
  Input validation for all forms (e.g., required fields, rating bounds).

⚙️ Backend API
  RESTful API using Express.js and MongoDB
  Cleanly structured controller, route, and model layers

##  Installation

1.  Clone the repository:

   ```bash
   git clone https://github.com/abhishekkr8/Wonderluster.git
   ```

2.  Navigate to the project directory:

   ```bash
   cd Wonderluster
   ```

3. Install dependencies for both the client and server:

   ```bash
   cd client && npm install
   ```

4. Create a `.env` file in the `server` directory and add the following:

   ```env
   ATLASDB_URL=<Your MongoDB URI>
   JWT_SECRET=<Your JWT Secret>
   MAP_TOKEN=<Your MAP_TOKEN>
   CLOUD_NAME=<Your CLOUD_NAME>
   CLOUD_API_KEY=<Your CLOUD_API_KEY>
   CLOUD_API_SECRET=<Your CLOUD_API_SECRET>
   ```

   Replace `<Your MongoDB URI>` with your MongoDB connection string and `<Your JWT Secret>` with a secure string for JWT token generation.

5. Start the server:

   ```bash
   cd wnaderluster && npm start
   ```

   This will start the server on `http://localhost:8080`.

## Contributing

Contributions are welcome! If you'd like to contribute to Notekeep, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature: `git checkout -b feature-name`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to your branch: `git push origin feature-name`.
5. Submit a pull request.
