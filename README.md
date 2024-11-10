# Flask Blog

A simple, dynamic blog application built using Flask. This project features essential blog functionalities like user authentication, post creation, updating, deletion, and more. It provides a clean, intuitive UI for easy navigation and user interaction.

## Features

- **User Authentication**: Sign up, log in, and log out functionalities.
- **Blog Posts**: Create, read, update, and delete blog posts.
- **User Profiles**: Manage profiles with a personalized dashboard.
- **Responsive Design**: User-friendly and responsive UI for an improved experience on all devices.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/RustedSwords/Flask_blog.git
    cd Flask_blog
    ```

2. **Set up a virtual environment**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:

   Create a `.env` file in the project root and add the following configuration:

    ```plaintext
    SECRET_KEY=<Your_Secret_Key>
    SQLALCHEMY_DATABASE_URI=sqlite:///site.db
    ```

5. **Initialize the database**:
    ```bash
    flask db init
    flask db migrate
    flask db upgrade
    ```

6. **Run the application**:
    ```bash
    flask run
    ```

   The application will start locally at `http://127.0.0.1:5000`.

## Usage

- **Homepage**: View recent blog posts.
- **User Registration**: Sign up with a new account.
- **Login/Logout**: Securely log in or out.
- **Create/Update/Delete Posts**: Create new posts, update existing ones, or delete posts.
- **Profile Management**: Update your profile and view your posts.

## Project Structure

```plaintext
Flask_blog/
├── flaskblog/
│   ├── __init__.py            # Initializes Flask app and configures extensions
│   ├── forms.py               # Contains forms for user login, registration, and posts
│   ├── models.py              # Defines database models (User, Post)
│   ├── routes.py              # Application routes and views
│   └── static/                # Static files (CSS, JS, images)
│   └── templates/             # HTML templates for different pages
├── migrations/                # Database migrations
├── .env                       # Environment variables (add your secret keys here)
├── config.py                  # Configuration settings for Flask app
└── run.py                     # Run the application
```

## Dependencies

All required dependencies are listed in the requirements.txt file. They include:

- Flask
- Flask-SQLAlchemy
- Flask-Bcrypt
- Flask-Login
- Flask-WTF\
\
Install them with:
    ```bash
    pip install -r requirements.txt
    ```