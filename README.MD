# Wallet and Transaction Management System
proof of concept to evaluate development skills in building a full-stack application.

This project is wallet and transaction management system built with:
- Backend: NestJS SQL PostgreSQL, and MongoDB.
- Frontend: Vue.js

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Features](#features)

## Prerequisites
### Frontend:
- Node.js (v16+)
- npm 

#### Key Dependencies
- 1. Vue.js (vue): Main framework.
- 2. Vue Router (vue-router): For routing in the app.
- 3. Vuex (vuex): State management.
- 4. Axios: For making HTTP requests.
- 5. Chart.js & Vue-Chart.js: For rendering charts.
- 6. JWT Decode (jwt-decode): To decode JWT tokens.
- 7. Tailwind CSS: For styling.
- 8. @vue/cli-service: Vue CLI for building and serving the app.
- 9. PostCSS and Autoprefixer: For CSS processing.
- 10. ESLint and Prettier: For code linting and formatting.


### backend: 
- Node.js (v16+)
- npm
- MongoDB (v5+) and Mongoose 10.1.0
- Redis 4.7.0
- PostgreSQL 

#### Key Dependencies:
- 1. NestJS Core Packages: @nestjs/common, @nestjs/core, etc.
- 2. MongoDB: Managed using @nestjs/mongoose and mongoose.
- 3. Redis: Managed using ioredis.
- 4. JWT Authentication: @nestjs/jwt, passport, and related packages.
- 5. TypeORM (Optional): You still have typeorm and pg installed. Ensure these are not unused.
- 6. Other Utilities:
- 7. bcrypt: For password hashing.
- 8. date-fns: For date manipulation.
- 9. axios: For HTTP requests.
- 10. ESLint and Prettier: For linting and formatting.

## Installation
1. Clone the repository:
   ```bash
   git clone 
   cd repo-name

2. Front-end installation:
- Go to the front-end directory `cd /wallet-app` 
- Also `cd /wallet-app` yes to directories.
- Install dependencies: ` npm install` 
- Run the development server: `npm run serve` 
- Access login page from: `http://localhost:8080/signin`
- Access signup page from: `http://localhost:8080/signup`
- Access dashboard page from: `http://localhost:8080/dashboard`
- Access transactions page from: `http://localhost:8080/transactons`

3. Back-end installation:
-  Go to the back-end directory in a new terminal keep the front-end terminal running: `cd .\wallet-transaction-backend\`
- Install dependencies: `npm install`
- Confirm environment variables `.env` file is located in: directory of  `\wallet-transaction-backend\` 
- Run the server: `npm run start`


## environment-variables
In case if the `.env` file is not in the `\wallet-transaction-backend\` directory,
 you can create a new `.env` and set the following:
 - a `JWT_SECRET=YOUR_JWT_SECRET`. 
 - `DB_HOST=localhost`
- `DB_PORT=5432`
- `DB_USERNAME=YOUR_DB_USERNAME`
- `DB_PASSWORD=YOUR_DB_PASSWORD`
- `DB_NAME=wallet_transaction_db`
- `MONGO_URI= YOUR_MONGO_URL/wallet_system`

## features
- this allows User to:
1. signup
2. signin
3. create a new wallet, with different currrancies. 
4. send money to other wallets with real time currancy convertion rates.
5. View Incoming, and Outoging Transactions.
6. dashboard with the following features:
- Calcaulate Available Balance of all wallets IN USD.
- Calcaulate Incoming of this Month in USD.
- Calcaulate Outgoing of this Month in USD.
- an interactive financial graph shows the Incoming and Outgoing for the last 7 days.
- a Quick look into recent Transactions.



