# LockVerse - Password Manager

LockVerse is a secure password manager application that allows users to store, manage, and organize their passwords in one convenient location. Built with modern web technologies, it provides a user-friendly interface with robust functionality.

## Features

- **Password Storage**: Securely store website URLs, usernames, and passwords
- **Password Visibility**: Toggle password visibility with a click
- **Copy to Clipboard**: Easily copy site URLs, usernames, or passwords with one click
- **Edit/Delete Functionality**: Modify or remove existing password entries
- **Responsive Design**: Works on desktop and mobile devices
- **Toast Notifications**: User-friendly feedback for all actions
- **MongoDB Integration**: Backend data persistence with MongoDB

## Technology Stack

### Frontend
- **React.js**: JavaScript library for building user interfaces
- **Tailwind CSS**: Utility-first CSS framework for styling
- **React Toastify**: Notification library for React
- **UUID**: Library for generating unique identifiers
- **Lordicon**: Animated icon library

### Backend
- **Node.js**: JavaScript runtime environment
- **Express.js**: Web application framework
- **MongoDB**: NoSQL database for data persistence
- **Mongoose**: MongoDB object modeling tool

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd passop-mongo
   ```

2. **Install frontend dependencies**:
   ```bash
   npm install
   ```

3. **Install backend dependencies**:
   ```bash
   cd backend
   npm install
   ```

4. **Set up MongoDB**:
   - Create a MongoDB database
   - Update the connection string in `backend/server.js` if needed

## Usage

1. **Start the backend server**:
   ```bash
   cd backend
   node server.js
   ```
   The server will run on `http://localhost:3000`

2. **Start the frontend development server**:
   ```bash
   npm run dev
   ```
   The application will be available at `http://localhost:5173`

3. **Using the application**:
   - Enter website URL, username, and password in the input fields
   - Click "Save Password" to store your credentials
   - View saved passwords in the table below the form
   - Use the icons to copy, edit, or delete password entries

## Folder Structure

```
passop-mongo/
├── backend/
│   └── server.js        # Backend Express server
├── src/
│   ├── components/
│   │   ├── Manager.jsx  # Main password management component
│   │   ├── Navbar.jsx   # Navigation bar component
│   │   └── Footer.jsx   # Footer component
│   └── App.jsx          # Main application component
├── public/
│   └── icons/           # Icon assets
├── README.md            # This file
└── package.json         # Project dependencies and scripts
```

## API Endpoints

The backend server provides the following RESTful API endpoints:

- **GET /**: Retrieve all saved passwords
- **POST /**: Save a new password entry
- **DELETE /**: Delete a password entry by ID

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to [Lordicon](https://lordicon.com/) for the animated icons
- Built with [React](https://reactjs.org/) and [Tailwind CSS](https://tailwindcss.com/)
- Backend powered by [Node.js](https://nodejs.org/), [Express](https://expressjs.com/), and [MongoDB](https://www.mongodb.com/)
