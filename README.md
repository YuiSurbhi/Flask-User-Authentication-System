# Flask-User-Authentication

This project is a simple user authentication system built with Flask and SQLite. It includes user registration, login, and logout functionalities, with an optional "Remember Me" feature to keep users logged in across sessions.<br>

## Features

- User Registration: Users can create an account with a unique email and password.<br>
- Login and Logout: Users can log in and out of their accounts.<br>
- Remember Me: Option to stay logged in across browser sessions.<br>
- Dashboard: Personalized user dashboard displayed after login.<br>

## 🛠 Technologies Used

- Flask: Web framework for building the application.<br>
- SQLite: Lightweight database to store user information.<br>
- SQLAlchemy: ORM for database interactions.<br>
- bcrypt: Library for hashing and verifying passwords.<br>
- Bootstrap: Frontend framework for styling the pages.<br>

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/YuiSurbhi/Flask-User-Authentication.git
cd Flask-User-Authentication
```
2. Create a virtual environment:

```bash
python -m venv venv
```
3. Activate the virtual environment:

   - Windows:

    ```bash
    venv\Scripts\activate
    ```
    
   - macOS/Linux:

    ```bash
    source venv/bin/activate
    ```
4. Install the dependencies:

```bash
pip install -r requirements.txt
```
5 Run the application:

```bash
python app.py
```
The application will start at http://127.0.0.1:5000.<br>

## Usage

- Home Page: Access the home page at `/`. This page includes links to the login and registration pages.<br>
- Register: Navigate to `/register` to create a new account.<br>
- Login: Navigate to `/login` to log in. Optionally, check "Remember Me" to stay logged in across sessions.<br>
- Dashboard: After logging in, you will be redirected to `/dashboard`.<br>
- Logout: Access `/logout` to log out from the application<br>

## 📂 Files and Directories

- `app.py`: Main application file with routes and logic.<br>
- `templates/`: Directory containing HTML files.<br>
   - `home.html`: Home page template.<br>
   - `register.html`: User registration page template.<br>
   - `login.html`: User login page template.<br>
   - `dashboard.html`: User dashboard template.<br>
- `static/`: Directory for static files like CSS.
  - `style.css`: Custom styles for the logout button.

    ```bash
     .logout-button {
    font-size: 20px;
    padding: 10px 20px;
    background-color: #f9f6f6;
    color: black;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
    }
    ```
- `requirements.txt`: List of Python package dependencies.<br>

## ⚙️ Configuration

- Secret Key: Used for session management. Update `app.secret_key` in `app.py` with a secure key.🔐<br>
- Database URI: SQLite database path specified in `app.config['SQLALCHEMY_DATABASE_URI']`.<br>

## 🤝 Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.<br>

#

Replace `<repository-url>` and `<repository-directory>` with your actual repository URL and directory name. You can customize the content based on any additional features or changes in your application.
