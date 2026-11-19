# Course Selling Application (Backend)

REST API for an online course marketplace with separate user and admin accounts, built with Node.js, Express and MongoDB.

## Done so far

- JWT authentication for users and admins (separate middleware in `middleware/`)
- **User routes:** `POST /signup`, `POST /signin`, `GET /purchases`
- **Course routes:** `POST /purchase`, `GET /preview`
- **Admin routes:** `POST /signup`, `POST /signin`, `POST /course`, `PUT /course`, `GET /course/bulk`
- MongoDB models through Mongoose (`db.js`), configuration through environment variables (`.env.example`)

## Stack

Node.js, Express, MongoDB (Mongoose), JSON Web Tokens, dotenv

## Run locally

```bash
npm install
cp .env.example .env   # fill in your MongoDB connection string and JWT secrets
node index.js
```

## Future scope

- Input validation and password hashing checks with a schema library (for example Zod)
- Payments integration for course purchases
- Pagination, search and course categories
- Tests and API documentation (OpenAPI)
- A React front end for students and admins
