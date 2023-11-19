# Node.js Backend Authentication

This is a Node.js backend authentication project that demonstrates building a secure authentication system using MongoDB as the database. The project utilizes popular technologies such as bcrypt for password hashing, dotenv for environment variable management, Express for handling HTTP requests, jsonwebtoken for token-based authentication, and mongoose for MongoDB integration.

**Node.js** is a runtime environment that allows you to run JavaScript on the server side. It is lightweight, scalable, and perfect for building fast and scalable network applications.

### MongoDB and MongoDB Atlas

**MongoDB** is a NoSQL database that provides a flexible, scalable, and high-performance solution for storing and retrieving data. In this project, we use **MongoDB Atlas**, a cloud-based database service, to ensure seamless database management and scalability.

## Technologies Used:

- **MongoDB**
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/93/MongoDB_Logo.svg" width="124px" height="124px">

- **NodeJs**
  <img src="https://upload.wikimedia.org/wikipedia/commons/d/d9/Node.js_logo.svg" width="124px" height="124px">

- **Express**
  <img src = "https://upload.wikimedia.org/wikipedia/commons/6/64/Expressjs.png" width = "60px" height = "60px">

- **JWT (JSON Web Tokens)**
  <img src = "https://cdn.worldvectorlogo.com/logos/jwt-3.svg" width = "60px" height = "60px">

- **bcrypt**
  <img src = "https://upload.wikimedia.org/wikipedia/commons/thumb/5/58/Hash_table_4_1_1_0_0_1_0_LL.svg" width = "60px" height = "60px">

- **dotenv**
  <img src = "https://raw.githubusercontent.com/motdotla/dotenv/master/dotenv.svg" width = "60px" height = "60px">

- **mongoose**
  <img src = "https://mongoosejs.com/docs/images/mongoose5_62x30_transparent.png" width = "60px" height = "60px">

- **VSCODE**
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg" width="60px" height="60px">

## Table of Contents

- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Security Considerations](#security-considerations)
- [Contributing](#contributing)

## Dependencies

- **bcrypt** : A library for hashing and salting passwords.
- **dotenv** : A zero-dependency module that loads environment variables from a `.env` file.
- **express** : A fast, unopinionated, minimalist web framework for Node.js.
- **jsonwebtoken** : A JSON Web Token (JWT) implementation to handle authentication tokens.
- **mongoose** : A MongoDB object modeling tool designed to work in an asynchronous environment.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/abylch/auth_bcrypt_jwt.git
cd auth_bcrypt_jwt
```

2. Install dependencies:

```bash
npm install
```

3. Create a .env file in the root directory and set the following environment variables:

```env
# Example .env file
PORT=3000
MONGODB_URI=mongodb://localhost/your-database-name
JWT_SECRET=your-secret-key
```

## Usage

1. Start the server:

```bash
nodemon app.js
```
* you'll need to install nodemon, if not in the system.
* The server will be running at http://localhost:3000 (or the port you specified in the .env file).

2. Use the provided API endpoints for authentication, such as:

- /auth/register - Register a new user.
- /auth/login - Authenticate and receive a JWT token.
- /user/profile - Access a protected route using the JWT token.

## Configuration

- bcrypt: No additional configuration required. It is used for securely hashing passwords.
- dotenv: Configure environment variables in the .env file.
- express: Customize routes, middleware, and other configurations in the app.js file.
- jsonwebtoken: Set the JWT secret key in the .env file.
- mongoose: Configure MongoDB connection in the dbConnection.js file.

## Security Considerations

Building a secure authentication system involves implementing several key concepts:

1. Password Hashing: Use bcrypt to securely hash and salt user passwords before storing them in the database.

2. Environment Variables: Store sensitive information like database connection strings and secret keys in environment variables using dotenv.

3. Token-Based Authentication: Implement token-based authentication using JSON Web Tokens (JWT) to securely transmit authentication data between the client and server.

4. HTTPS: Deploy your application over HTTPS to encrypt data in transit and enhance security.

## Contributing

Feel free to contribute by opening issues or submitting pull requests.

