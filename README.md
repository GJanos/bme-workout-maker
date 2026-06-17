# Workout Maker

A web app for building and managing workout routines: register an account, create a
library of exercises, and arrange them into customizable workout tables. One of my
earliest full-stack projects (2022).

**Tech stack:** Node.js · Express · EJS templates · MongoDB (Mongoose) · vanilla JS/CSS
frontend

## Features

- **User accounts** with authentication middleware.
- **Exercise library** — create, edit, view, list, and delete exercises.
- **Workout builder** — arrange exercises into workout tables with configurable size and
  placement.
- Server-rendered UI with reusable EJS partials (navbar, header, footer, dropdowns,
  workout table).

## Project structure

```
├── index.js              # app entry point
├── config/db.js          # database connection
├── routes/route.js       # route definitions
├── middleware/           # exercise / workout / user / auth handlers
├── models/               # exercise, user, workout schemas
├── views/                # EJS templates (+ reusable partials)
├── public/               # css, js, images
└── test/                 # tests for table placement / creation
```

## Build & run

```bash
npm install
# configure your MongoDB connection (see config/db.js)
npm run dev        # starts with nodemon
```

---

*Early full-stack project (2022). Express + EJS + MongoDB, organized around a
middleware-per-action structure.*
