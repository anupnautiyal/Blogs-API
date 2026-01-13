# Blogs API (Backend 6.1) ✅

**Small Express.js API for managing blog posts (in-memory).** The project includes simple CRUD endpoints and EJS views for a minimal UI.

---

## Prerequisites ⚙️
- Node.js (v14+ recommended)
- npm

## Install 📦
```bash
npm install
```

## Run ▶️
Start the server with:
```bash
node index.js
```

Tip: you can add a start script in `package.json`:
```json
"scripts": {
  "start": "node index.js"
}
```

The app listens on port **4000** by default (http://localhost:4000).

## Endpoints 🔧
- `GET /posts` — List all posts
- `GET /posts/:id` — Get a single post by id
- `POST /posts` — Create a new post (body: `title`, `content`, `author`)
- `PATCH /posts/:id` — Update one or more fields of a post
- `DELETE /posts/:id` — Delete a post

Example (curl):
```bash
curl http://localhost:4000/posts

curl -X POST -H "Content-Type: application/json" \
  -d '{"title":"Hello","content":"World","author":"You"}' \
  http://localhost:4000/posts
```

## Project structure 📁
- `index.js` — main server & API routes
- `server.js` / `solution.js` — supporting files (if present)
- `views/` — EJS templates (`index.ejs`, `modify.ejs`)
- `public/` — static assets (`styles/main.css`)

> Note: Data is stored in memory and resets on server restart.

## License & Notes 📝
Simple educational project for the Web Development course. Modify freely for learning and experimentation.
