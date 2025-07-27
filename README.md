# QuickBlog-FullStack

A fullstack blog platform with a modern React frontend and an Express/MongoDB backend. Features include blog creation, AI-powered content generation, image uploads, comments, and an admin dashboard.

## Demo

[Live App](https://blog-app-navy-eta.vercel.app/)

---

## Features

- 📝 Create, edit, and delete blog posts (admin)
- 🖼️ Upload blog images (ImageKit integration)
- 🤖 Generate blog content using Google Gemini AI
- 💬 Comment on blog posts (with approval system)
- 📊 Admin dashboard for managing blogs and comments
- 🔒 Admin authentication
- 🌐 Responsive, modern UI (React + Tailwind CSS)

---

## Tech Stack

- **Frontend:** React, Vite, Tailwind CSS, Axios, Quill, Marked
- **Backend:** Node.js, Express, MongoDB (Mongoose), JWT, Multer, ImageKit, Google Gemini AI

---

## Directory Structure

```
QuickBlog-FullStack/
  client/      # React frontend
  server/      # Express backend
```

---

## Setup Instructions

### Prerequisites
- Node.js (v18+ recommended)
- MongoDB instance (local or cloud)
- ImageKit account (for image uploads)
- Google Gemini API key (for AI content)

### 1. Clone the repository
```bash
git clone <repo-url>
cd QuickBlog-FullStack
```

### 2. Backend Setup (server)
```bash
cd server
npm install
```

#### Create a `.env` file in `server/` with the following variables:
```
MONGODB_URI=your_mongodb_connection_string
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
GEMINI_API_KEY=your_google_gemini_api_key
PORT=3000 # or any port
```

#### Start the backend server:
```bash
npm run server
```

### 3. Frontend Setup (client)
```bash
cd ../client
npm install
```

#### Start the frontend dev server:
```bash
npm run dev
```

- The frontend will run on [http://localhost:5173](http://localhost:5173) by default.
- The backend will run on [http://localhost:3000](http://localhost:3000) by default.

---

## Usage

- Visit the homepage to browse blogs.
- Click a blog to read and comment.
- Admins can log in at `/admin` to manage blogs and comments.
- Use the "Add Blog" page for AI-powered content generation and image upload.

---

## Deployment

- Both `client` and `server` have `vercel.json` for Vercel deployment.
- Set environment variables in your deployment platform as per `.env` above.

---

## Credits

- Built by Swatika
- [React](https://react.dev/), [Vite](https://vitejs.dev/), [Tailwind CSS](https://tailwindcss.com/), [Express](https://expressjs.com/), [MongoDB](https://www.mongodb.com/), [ImageKit](https://imagekit.io/), [Google Gemini](https://ai.google.dev/)

---

## License

This project is for educational/demo purposes.
