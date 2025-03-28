# Trust App - Food Donation Platform

## Overview
Trust App is a MERN (MongoDB, Express.js, React.js, Node.js) stack-based web platform designed to facilitate food donations by connecting users with orphanages and registered trusts. The system allows users to donate food, while trusts receive real-time notifications about available donations. Admins manage transactions and oversee the trust operations.

## Features
- **User Module**
  - User registration and authentication
  - Add available food quantity for donation
  - Send donation requests to nearby trusts
  - View donation history

- **Trust Module**
  - Receive real-time notifications of food donations
  - Accept or decline donation requests
  - View and manage received donations
  
- **Admin Module**
  - Manage users and trust accounts
  - Oversee and track donation transactions
  - Generate reports on donations and distributions

## Tech Stack
- **Frontend**: React.js
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Token)
- **Notifications**: Real-time updates via WebSockets or Firebase

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/trust-app.git
   cd trust-app
   ```

2. Install dependencies:
   ```sh
   npm install  # For backend
   cd client && npm install  # For frontend
   ```

3. Set up environment variables:
   - Create a `.env` file in the root and add the following:
     ```env
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     ```

4. Start the backend server:
   ```sh
   npm start
   ```

5. Start the frontend server:
   ```sh
   cd client
   npm start
   ```

## API Endpoints
### User Module
- `POST /api/user/register` - Register a new user
- `POST /api/user/login` - User login
- `POST /api/user/donate` - Add food donation request
- `GET /api/user/history` - View donation history

### Trust Module
- `GET /api/trust/notifications` - Get real-time donation requests
- `POST /api/trust/accept/:id` - Accept a donation request
- `POST /api/trust/reject/:id` - Reject a donation request

### Admin Module
- `GET /api/admin/users` - Manage users
- `GET /api/admin/trusts` - Manage trusts
- `GET /api/admin/donations` - View donation transactions

## Contributing
1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

## License
This project is licensed under the MIT License.

## Contact
For any issues or suggestions, feel free to contact the project maintainers.

