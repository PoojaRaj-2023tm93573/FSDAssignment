# FSDAssignment
Assignment-1 Full Stack Application Development

A full-stack web application that allows users to list, search, and exchange books. The platform supports user authentication, book management, and messaging between users.

Features

    User Authentication: Register and log in securely using JWT.
    Book Management: Add, edit, delete, and list books for exchange.
    Search and Filter: Find books by title, author, genre, or condition.
  
User Authentication:

Method	Endpoint	        Description
POST	/api/users/register	Register a new user
POST	/api/users/login	Login user and get JWT
GET	/api/users/profile	Get user profile

Delete a book

GET	/api/books	List all books
POST	/api/books	Add a new book
PUT	/api/books/:id	Update an existing book
DELETE	/api/books/:id	Delete a book

Future Enhancements

    Mobile App Integration: Use the same API for mobile platforms.
    Book Recommendations: Based on user preferences.
    Notifications: For exchange requests or messages.
    Admin Dashboard: For platform management.

    Scalability and Modularity

    Component-Based Frontend:
        React components are modular, reusable, and follow a structured hierarchy.
        Lazy loading for faster performance.

    Decoupled Backend:
        RESTful APIs allow the backend to be reused for mobile apps.
        Separation of concerns (routes, controllers, services).

    Database Scalability:
        MongoDB supports sharding for horizontal scaling.
        Flexible schema design for adding fields without breaking the application.

    Microservices-Ready:
        Backend can be extended to microservices for notifications, recommendations, etc.

        Tech Stack
Frontend:

    HTML5, CSS3, JavaScript: Responsive and user-friendly UI.
    Bootstrap: For styling and responsive design.

Backend:

    Django: Backend framework with Django REST Framework (DRF) for APIs.
    MySQL: Relational database for structured data storage.

Tools:

    Visual Studio Code: IDE for development.
    Postman: For testing APIs.
    Git/GitHub: Version control.

Installation and Setup

Prerequisites:

    Python (3.8+): Download from python.org.
    MySQL: Install and set up a MySQL server.
    Django: Install using pip.

Configure Database:

    Open book_exchange/settings.py and update the database configuration:
    DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'book_exchange',
        'USER': 'your_mysql_user',
        'PASSWORD': 'your_mysql_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}


Apply Migrations:
python manage.py makemigrations
python manage.py migrate

Run the Development Server:

python manage.py runserver

Access the Application: Open http://127.0.0.1:8000 in your browser.

    
