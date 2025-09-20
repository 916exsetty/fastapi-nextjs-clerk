# FastAPI Next.js Clerk Integration 🚀

![FastAPI](https://img.shields.io/badge/FastAPI-007ACC?style=flat&logo=fastapi&logoColor=white) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=next.js&logoColor=white) ![Clerk](https://img.shields.io/badge/Clerk-1D9BF0?style=flat&logo=clerk&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

Welcome to the **FastAPI Next.js Clerk Integration** project! This repository showcases a seamless integration between a FastAPI backend and a Next.js frontend, utilizing Clerk for user authentication. 

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)
- [Releases](#releases)

## Overview

This project demonstrates how to build a modern web application with a FastAPI backend and a Next.js frontend. Users can authenticate through Clerk, which issues JSON Web Tokens (JWTs). These tokens allow secure access to protected API endpoints in the FastAPI backend.

## Features

- User authentication using Clerk
- Secure API access with JWTs
- Responsive frontend built with Next.js
- FastAPI backend for handling requests
- Docker support for easy deployment
- Comprehensive documentation

## Technologies Used

- **Backend**: FastAPI, Python
- **Frontend**: Next.js, React, TypeScript, Tailwind CSS
- **Authentication**: Clerk
- **Containerization**: Docker, Docker Compose

## Getting Started

To get started with this project, follow these steps:

1. **Clone the Repository**

   Use the following command to clone the repository:

   ```bash
   git clone https://github.com/916exsetty/fastapi-nextjs-clerk.git
   cd fastapi-nextjs-clerk
   ```

2. **Install Dependencies**

   For the backend, navigate to the `backend` directory and install the required packages:

   ```bash
   cd backend
   pip install -r requirements.txt
   ```

   For the frontend, navigate to the `frontend` directory and install the necessary packages:

   ```bash
   cd frontend
   npm install
   ```

3. **Set Up Environment Variables**

   Create a `.env` file in the backend directory and add your Clerk API keys:

   ```plaintext
   CLERK_API_KEY=your_clerk_api_key
   ```

4. **Run the Application**

   Use Docker Compose to start the application:

   ```bash
   docker-compose up
   ```

   The backend will run on `http://localhost:8000` and the frontend will run on `http://localhost:3000`.

## Project Structure

Here is a brief overview of the project structure:

```
fastapi-nextjs-clerk/
│
├── backend/
│   ├── app/
│   ├── requirements.txt
│   └── .env
│
├── frontend/
│   ├── src/
│   ├── package.json
│   └── tailwind.config.js
│
├── docker-compose.yml
└── README.md
```

## Usage

Once the application is running, you can access the frontend at `http://localhost:3000`. The login page will allow users to authenticate using Clerk. After logging in, users can access protected resources through the FastAPI backend.

### Authentication Flow

1. The user visits the login page.
2. The user enters their credentials and submits the form.
3. Clerk verifies the credentials and issues a JWT.
4. The frontend sends the JWT to the backend for API access.
5. The backend validates the JWT and responds accordingly.

## API Endpoints

The FastAPI backend provides several endpoints for interaction. Here are some key endpoints:

- **GET /api/protected**

  This endpoint requires a valid JWT for access. It returns protected data.

- **POST /api/login**

  This endpoint allows users to log in. It expects user credentials and returns a JWT.

- **GET /api/users**

  This endpoint retrieves a list of users. It requires a valid JWT.

## Contributing

Contributions are welcome! If you have suggestions or improvements, please create a pull request or open an issue.

### Steps to Contribute

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes.
4. Commit your changes and push to your fork.
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

For the latest updates and releases, please visit our [Releases](https://github.com/916exsetty/fastapi-nextjs-clerk/releases) page. You can download and execute the files from there to get the latest features and fixes.

Feel free to explore the repository, and don't hesitate to check the "Releases" section for any updates or new features.