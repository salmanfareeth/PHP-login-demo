# PHP Login Demo

This is a simple PHP login system that demonstrates user authentication and session management using PHP and MySQL. The application uses prepared statements to prevent SQL injection attacks and includes basic features such as user registration, login, and session handling.

## Features

- User registration with password hashing
- User login with session management
- Prepared statements to prevent SQL injection
- Secure password storage using `password_hash` and `password_verify`

## Setup

### Prerequisites

- PHP installed on your local machine
- MySQL server installed and running
- A web server (e.g., Apache, Nginx) or PHP built-in server

### Steps

1. **Clone the repository:**

```bash
git clone https://github.com/salmanfareeth/PHP-login-demo.git
```

2. **Navigate to the project directory:**

```bash
cd php-login-demo
```

3. **Import the SQL database:**

- Create a database named login_demo in your MySQL server.
- Import the SQL script from the `addusers.sql` file to create the users table and insert a sample user.

4. **Update the database configuration:**

- Open config.php and update the database connection details if necessary.

5. **Start Your Web Server:**

- Ensure your web server (Apache, Nginx, etc.) or PHP built-in server is running.
  
6. **Open your web browser and navigate to `http://localhost:8000/register.php` to register a new user.**

7. **Navigate to `http://localhost:8000/login.php` to log in with the registered user.**


### Explanation of the Project Files

- **`config.php`**: Contains the database connection details.
- **`login.php`**: Handles user login with prepared statements to prevent SQL injection.
- **`register.php`**: Allows users to register by hashing their passwords and storing them securely.
- **`welcome.php`**: Displays a welcome message with the logged-in user's username.
- **`logout.php`**: Handles user logout by destroying the session.
- **`addusers.sql`**: SQL script to set up the database and create the `users` table with a sample user.


## Usage
- **`Register`**: Go to the registration page (register.php) to create a new user.
- **`Login`**: Go to the login page (login.php) to authenticate with your username and password.
- **`Welcome`**: After a successful login, you'll be redirected to the welcome page (welcome.php), where you can see a personalized greeting.
- **`Logout`**: Click the logout link on the welcome page to end your session.


## Important Note

This project is for demonstration and learning purposes only. Do not use this code in a production environment without proper security measures.

