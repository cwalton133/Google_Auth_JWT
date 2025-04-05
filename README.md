# BookAPI with JWT Authentication

This Django application serves as a Book API with JWT (JSON Web Token) authentication. It enables users to manage authors and courses efficiently, with features tailored for educational purposes.

## Features

- Create, retrieve, update, and delete (CRUD) author information.
- Manage courses associated with each author.
- Secure JWT authentication for user sessions.

## Models

The application defines two primary models: `Author` and `Course`.

### Author Model

Represents an author in the system.

#### Fields

- **id**: UUIDField (Primary Key) - Unique identifier for each author, automatically generated.
- **firstname**: CharField - Author's first name (max length: 55).
- **lastname**: CharField - Author's last name (max length: 55).
- **image**: ImageField - Upload field for author images.
- **othername**: CharField - Author's other name (optional).
- **email**: EmailField - Author's email address.
- **phone_number_1**: CharField - Primary phone number (max length: 20).
- **phone_number_2**: CharField - Secondary phone number (optional, max length: 20).
- **created_at**: DateTimeField - Timestamp when the author record was created.

#### Meta

- Orders authors by `created_at`, latest first.

#### String Representation

Returns the author's first name when the object is represented as a string.

### Course Model

Represents a course related to an author.

#### Fields

- **id**: UUIDField (Primary Key) - Unique identifier for each course, automatically generated.
- **name**: CharField - Name of the course (max length: 150).
- **description**: TextField - Detailed description of the course.
- **author**: ForeignKey - Link to the `Author` model, establishes a relationship.
- **created_at**: DateTimeField - Timestamp when the course record was created.

## Installation

Follow these steps to set up the project locally:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/cwalton133/Google_Auth_JWT.git
   cd to BookAPI_JWT
   ```

2. Create a virtual environment:

python -m venv venv
source venv/bin/activate # For Mac/Linux
venv\Scripts\activate # On Windows

Install the required packages:

pip install -r requirements.txt

Set up the database:

python manage.py makemigrations
python manage.py migrate

Create a superuser (optional, for accessing the admin panel):

python manage.py createsuperuser

Run the server:

python manage.py runserver

Visit http://127.0.0.1:8000 to access the application. Use the admin panel at http://127.0.0.1:8000/admin for managing authors and courses.

Endpoints (Example)
Authors

GET /authors/: Retrieve the list of authors.
POST /authors/: Create a new author.
GET /authors/{id}/: Retrieve a specific author by ID.
PUT/PATCH /authors/{id}/: Update an existing author.
DELETE /authors/{id}/: Delete an author.
Courses

GET /courses/: Retrieve the list of courses.
POST /courses/: Create a new course.
GET /courses/{id}/: Retrieve a specific course by ID.
PUT/PATCH /courses/{id}/: Update an existing course.
DELETE /courses/{id}/: Delete a course.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Contributing
If you wish to contribute to this project, please fork the repository and submit a pull request. All contributions are welcome!

Acknowledgements
Django
Django REST Framework
JSON Web Tokens

Contributing

1. I welcome contributions! To contribute:
2. Fork the repository.
3. Create a feature branch (git checkout -b feature-name).
4. Commit your changes (git commit -m "Add feature").
5. Push to GitHub (git push origin feature-name).
6. Create a Pull Request (PR) for review.

License
This project is licensed under the MIT License.
MIT License
Copyright (c) 2025

Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Fork the repository.
Create a feature branch (git checkout -b feature/YourFeature).
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature/YourFeature).
Open a pull request.

Contact Us
For any questions or feedback, please contact:

Charles Walton - cwalton1335@gmail.com
GitHub: cwalton133

Thank you for checking out the BookAPI_JWT Application!
