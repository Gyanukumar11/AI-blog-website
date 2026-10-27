# AI Blog Website

A full-stack AI-powered blogging platform built using the **MERN stack**. Users can explore blog posts, while administrators can create, edit, and manage content through an admin dashboard. The application also integrates AI-powered content generation.

## 🌐 Live Demo

**[Visit AI Blog Website](https://quickblog-gs.vercel.app/)**

## ✨ Features

- **Blog Reading:** Browse and read published blog posts.
- **Admin Dashboard:** Manage blog content from a dedicated dashboard.
- **Create, Edit & Delete Blogs:** Add new posts and manage existing content.
- **AI Content Generation:** Generate blog content with AI assistance.
- **Authentication:** Secure admin access using authentication.
- **Image Management:** Upload and manage blog images using ImageKit.
- **Responsive UI:** Access the website across different screen sizes.

## 🛠️ Tech Stack

**Frontend**
- React
- Vite
- Tailwind CSS
- JavaScript

**Backend**
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Tokens (JWT)

**Services & Integrations**
- Google Gemini API for AI-powered content generation
- ImageKit for image hosting and optimization
- MongoDB for database storage
- Vercel for frontend deployment

## 📁 Project Structure

```text
AI-blog-website/
├── client/                 # React frontend
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── .env.example
│
├── server/                 # Express backend
│   ├── configs/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── package.json
│   └── .env.example
│
├── .gitignore
└── README.md
```

*The exact files and folders may vary slightly depending on the project version.*

## ⚙️ Run Locally

### Prerequisites

- Node.js and npm
- MongoDB connection string
- Google Gemini API key
- ImageKit account and API credentials

### 1. Clone the Repository

```bash
git clone https://github.com/Gyanukumar11/AI-blog-website.git
cd AI-blog-website
```

### 2. Set Up the Backend

```bash
cd server
npm install
```

Create a `.env` file inside the `server/` directory and configure the required environment variables:

```env
PORT=3000
MONGODB_URI=your_mongodb_connection_string
ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_admin_password
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
```

Use the variable names expected by the actual backend code. If the application appends a database name to `MONGODB_URI`, configure the connection string accordingly.

Start the backend using the script defined in `server/package.json`. For this project, the command is:

```bash
npm run server
```

### 3. Set Up the Frontend

Open a new terminal:

```bash
cd client
npm install
```

Create a `.env` file inside `client/` and configure the backend API URL using the environment variable name expected by the frontend.

For a Vite application, frontend environment variables exposed to browser code generally need the `VITE_` prefix. For example:

```env
VITE_BASE_URL=http://localhost:3000
```

Replace `VITE_BASE_URL` with the actual variable name used by the project if it differs.

Start the frontend:

```bash
npm run dev
```

Open the local URL displayed by Vite, usually `http://localhost:5173`.

## 🚀 Deployment

The frontend is deployed on Vercel.

**Live application:** https://quickblog-gs.vercel.app/

The backend and database must also be configured correctly for all features to work in production. Set production environment variables in the relevant hosting dashboard, configure the backend API URL, and allow the deployed frontend origin in the backend's CORS settings.

## 🔐 Security

- Never commit `.env` files, API keys, database credentials, or admin passwords.
- Configure secrets through environment variables in your hosting provider.
- Use strong admin credentials and a secure JWT secret.
- Rotate any credentials that may have been exposed in a public repository.

## 👨‍💻 Author

**GyanuKumar11**

- GitHub: [Gyanukumar11](https://github.com/Gyanukumar11)
- Project Repository: [AI-blog-website](https://github.com/Gyanukumar11/AI-blog-website)
- Live Demo: [quickblog-gs.vercel.app](https://quickblog-gs.vercel.app/)

## 📄 License

Add a license before redistributing this project. If you obtained the source code from a paid template or course, check its license and redistribution terms before publishing it publicly.
