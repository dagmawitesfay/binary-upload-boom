# Binary Upload Boom

A full-stack social media app built with Node.js, Express, MongoDB, and Cloudinary. Users can sign up, log in, upload photos, view a feed, like posts, comment on posts, and manage their profile.

## Features

- User authentication with Passport.js
- Create and delete photo posts
- View a feed of recent posts
- Like posts
- Comment on posts
- User profile page
- Cloudinary image uploads

## Tech Stack

- Node.js
- Express
- MongoDB + Mongoose
- EJS
- Passport.js
- Cloudinary
- Multer

## Installation

1. Install dependencies:

   ```bash
   npm install
   ```

2. Create a `.env` file inside the `config` folder:

   ```env
   PORT=2121
   MONGODB_CONNECTIION=mongodb://localhost:27017/binary-upload-boom
   CLOUD_NAME=your_cloud_name
   API_KEY=your_api_key
   API_SECRET=your_api_secret
   ```

   Replace the MongoDB and Cloudinary values with your own database URI and Cloudinary credentials.

## Run the app

```bash
npm start
```

The app will start on the port defined in `PORT` (default is 2121).

## Project Structure

```text
.
├── config/
│   ├── .env
│   ├── database.js
│   └── passport.js
├── controllers/
├── middleware/
├── models/
├── public/
├── routes/
├── views/
├── server.js
├── package.json
└── README.md
```

## Notes

- This project expects a MongoDB instance to be running or a valid MongoDB Atlas connection string.
- Cloudinary is used for image upload and storage.
- If you are running the app locally, you may need to create the database or initialize your MongoDB instance before logging in and posting content.
