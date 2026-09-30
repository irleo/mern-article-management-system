# MERN Article Management System

A full-stack content-management application built with React, Node.js, Express, and MongoDB. The project includes public article views and an administration interface for managing articles and users.

## Features

- Public article listing and article detail views
- Article creation, editing, and deletion
- User creation, editing, activation state, and deletion
- JWT login
- Password hashing with bcrypt
- Admin, editor, and viewer account types
- Material UI data tables and charts
- REST API backed by MongoDB

## Technology Stack

**Frontend:** React, Vite, Material UI, MUI Data Grid, MUI X Charts, React Router, Axios, React Leaflet

**Backend:** Node.js, Express, MongoDB, Mongoose, JSON Web Tokens, bcrypt, CORS

## Project Structure

```text
mern-article-management-system/
├── garzon-client/
└── garzon-server/
```

## API Overview

### Articles
```text
GET    /api/articles
GET    /api/articles/name/:name
POST   /api/articles
PUT    /api/articles/:id
DELETE /api/articles/:id
```

### Users
```text
GET    /api/users
POST   /api/users
PUT    /api/users/:id
DELETE /api/users/:id
POST   /api/users/login
```

## Local Setup

### Backend
```bash
cd garzon-server
npm install
npm run dev
```

Create `garzon-server/.env` with `MONGO_URI`, `JWT_SECRET`, and optionally `PORT`.

### Frontend
```bash
cd garzon-client
npm install
npm run dev
```

## Known Limitations

JWT authentication and user-role data are implemented, but the current CRUD routes require further server-side authorization hardening before production use. Production CORS should also be restricted to trusted origins.
