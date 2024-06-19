# Food Delivery App - Tomato

This repository contains the source code for a food delivery application with a frontend, backend, and admin panel. Each part of the application is containerized using Docker and can be easily set up using Docker Compose.

## Follow the steps to setup the application in your local machine

Before you begin, ensure you have the following installed on your system:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Project Structure

The project consists of three main directories:

- `backend`: The backend server built with Node.js and Express.
- `frontend`: The user-facing frontend built with Vite.
- `admin`: The admin panel also built with Vite.

## Environment Variables

Create a `.env` file in the root of your project directory with the following content:

```env
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
USER_FRONTEND_URL=http://localhost:5173
VITE_BACKEND_URL=http://localhost:4000
BACKEND_PORT=4000
FRONTEND_PORT=5173
ADMIN_PORT=5174

Replace your_jwt_secret and your_stripe_secret_key with your actual secret keys.
```

## Create Docker Compose File
Copy paste the `docker-compose.yml` code from my github repository to your project directory.
So currently your project directory contains 2 files, `.env` and `docker-compose.yml`

And yes !!. Now you can run the command `docker-compose up --build` to start the application
To stop you can use `docker-compose down` command


