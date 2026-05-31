# MERN Ecommerce

An end-to-end ecommerce platform built with the MERN stack, Redux Toolkit, and Material UI.

MERN Ecommerce is a full-stack shopping application designed to deliver a smooth experience for customers and administrators alike. It combines MongoDB, Express.js, React, and Node.js with Redux Toolkit for scalable state management and Material UI for a modern interface. The project includes secure authentication, product browsing, wishlist and cart workflows, order management, and admin tools for catalog control.

## Key Features

### Customer Experience

- Browse products and view detailed product pages
- Add items to cart and adjust quantities
- Save favorite items in a wishlist
- Write, edit, and delete product reviews
- Place orders and view order history
- Manage profile details and multiple addresses

### Admin Experience

- Create, update, delete, and soft-delete products
- Manage product stock, category, and brand data
- Review and update order status
- Maintain a clean and organized product catalog

### Security and UX

- Login, signup, logout, OTP verification, and password reset
- Protected routes for authenticated users
- JWT-based authorization with secure cookies
- Responsive UI built with Material UI
- Centralized state management with Redux Toolkit

## Tech Stack

### Frontend

- React
- Redux Toolkit
- React Router
- Material UI
- Axios
- Framer Motion
- Lottie React

### Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- Nodemailer
- Cookie Parser

## Project Structure

```text
backend/
frontend/
```

## Screenshots

Add screenshots of the homepage, product details, cart, checkout, and admin dashboard here.

## Getting Started

### Prerequisites

- Node.js v21.1.0 or later
- MongoDB running locally or a MongoDB Atlas connection string

### Clone the repository

```bash
git https://github.com/manas-techie/ecommerce.git
cd ecommerce
```

### Install dependencies

Install dependencies for the frontend and backend separately.

#### Frontend

```bash
cd frontend
npm install
```

#### Backend

```bash
cd backend
npm install
```

## Environment Variables

Create a .env file in both the backend and frontend directories.

### Backend .env

```env
MONGO_URI="your-mongodb-connection-string"
ORIGIN="http://localhost:3000"
EMAIL="your-email@example.com"
PASSWORD="your-email-password"
LOGIN_TOKEN_EXPIRATION="30d"
OTP_EXPIRATION_TIME="120000"
PASSWORD_RESET_TOKEN_EXPIRATION="2m"
COOKIE_EXPIRATION_DAYS="30"
SECRET_KEY="your-secret-key"
PRODUCTION="false"
```

### Frontend .env

```env
REACT_APP_BASE_URL="http://localhost:8000"
```

### Notes

- Replace all placeholder values with your own configuration.
- Do not commit .env files to version control.

## Available Scripts

### Backend

- npm run dev - start the backend with nodemon
- npm start - start the backend with node
- npm run seed - populate the database with sample data

### Frontend

- npm start - run the React development server
- npm run build - create a production build

## Data Seeding

The backend includes a seed script that loads sample brands, categories, products, users, addresses, wishlists, carts, reviews, and orders.

```bash
cd backend
npm run seed
```

## Running the Application

Use separate terminals for the backend and frontend.

### Start the backend server

```bash
cd backend
npm run dev
```

The backend runs on port 8000 by default.

### Start the frontend server

```bash
cd frontend
npm start
```

The frontend runs on port 3000.

## Demo Login

After seeding the database, you can explore the application with the demo account below.

```text
email: demo@gmail.com
password: helloWorld@123
```

### Demo Account Limitations

- Password reset and OTP verification are not available for the demo account because it uses a non-real email address.
- To test those flows, create a real account with a valid email address.
- The demo account is still useful for browsing, cart, wishlist, profile, and order history flows.

## Access the Application

Once both servers are running, open:

- Backend: http://localhost:8000
- Frontend: http://localhost:3000
