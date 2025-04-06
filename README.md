<p align="left">
  <a href="https://www.linkedin.com/in/cwalton1335" target="_blank"><img alt="LinkedIn" title="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>

<a href="https://www.youtube.com/channel/UCYesptHRU1QZ2pHZkAqdQTw/videos" target="_blank"><img alt="YouTube" title="YouTube" src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/></a>

<a href="https://www.buymeacoffee.com/calton1335" target="_blank"><img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me A Coffee"></a>

<a href="https://www.udemy.com/course/#" target="_blank"><img src="https://img.shields.io/badge/Udemy-EC5252?style=for-the-badge&logo=Udemy&logoColor=white" alt="Udemy"></a>

</p>

# About The Project - BookAPI with JWT Authentication

GreatKart is an eCommerce application built with Python Django This Django application serves as a Book API with JWT (JSON Web Token) authentication. It enables users to manage authors and courses efficiently, with features tailored for educational purposes.

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

[Check Demo](http://djangogreatkart.com/)

_Learn how to build these [complex functionalities from the scratch](https://www.udemy.com/course/django-ecommerce-project-based-course-python-django-web-development/?referralCode=BAD74EA99BCC2E331D13)_

<p align="left">
  <a href="https://www.udemy.com/course/django-ecommerce-project-based-course-python-django-web-development/?referralCode=BAD74EA99BCC2E331D13" target="_blank"><img src="https://img.shields.io/badge/Udemy-5624D0?style=for-the-badge&logo=Udemy&logoColor=white" alt="Udemy"></a>
</p>

<img src="https://github.com/dev-rathankumar/greatkart-pre-deploy/blob/main/media/greatkart-screenshot.jpg">

# Setup Instructions

Follow these steps to set up the project locally:

1. Clone the repository `git clone https://github.com/cwalton133/Google_Auth_JWT.git`
2. Navigrate to the working directory `cd BookAPI_JWT`
3. Open the project from the code editor `code .` or `atom .`
4. Create virtual environment `python -m venv env`
5. Activate the virtual environment `source env/Scripts/activate`
6. Install required packages to run the project `pip install -r requirements.txt`
7. Rename _.env-sample_ to _.env_
8. Fill up the environment variables:
   _Generate your own Secret key using this tool [https://djecrety.ir/](https://djecrety.ir/), copy and paste the secret key in the SECRET_KEY field._

   _Your configuration should look something like this:_

   ```sh
   SECRET_KEY=47d)n05#ei0rg4#)*@fuhc%$5+0n(t%jgxg$)!1pkegsi*l4c%
   DEBUG=True
   EMAIL_HOST=smtp.gmail.com
   EMAIL_PORT=587
   EMAIL_HOST_USER=youremailaddress@gmail.com
   EMAIL_HOST_PASSWORD=yourStrongPassword
   EMAIL_USE_TLS=True
   ```

   _Note: If you are using gmail account, make sure to [use app password](https://support.google.com/accounts/answer/185833)_

9. Create database tables
   ```sh
   python manage.py migrate
   ```
10. Create a super user
    ```sh
    python manage.py createsuperuser
    ```
    _GitBash users may have to run this to create a super user - `winpty python manage.py createsuperuser`_
11. Run server
    ```sh
    python manage.py runserver
    ```
12. Login to admin panel - (`http://127.0.0.1:8000/admin/`)
13. Add Author, Course, add Book, register user, login, and EXPLORE SO MANY FEATURES

[Checkout me out on my Githhub](https://github.com/cwalton133/)

_Learn how to build these [complex functionalities from my Github Page](https://github.com/cwalton133)_

## Support

💙 If you like this project, give it a ⭐ and share it with friends!

<p align="left">
Endpoints (Example) Authors

GET /authors/: Retrieve the list of authors. POST /authors/: Create a new author. GET /authors/{id}/: Retrieve a specific author by ID. PUT/PATCH /authors/{id}/: Update an existing author. DELETE /authors/{id}/: Delete an author. Courses

GET /courses/: Retrieve the list of courses. POST /courses/: Create a new course. GET /courses/{id}/: Retrieve a specific course by ID. PUT/PATCH /courses/{id}/: Update an existing course. DELETE /courses/{id}/: Delete a course. License This project is licensed under the MIT License - see the LICENSE file for details.

Contributing If you wish to contribute to this project, please fork the repository and submit a pull request. All contributions are welcome!

Acknowledgements Django Django REST Framework JSON Web Tokens

</p>

<p align="left">

## Contributing

I welcome contributions! To contribute:
Fork the repository.
Create a feature branch (git checkout -b feature-name).
Commit your changes (git commit -m "Add feature").
Push to GitHub (git push origin feature-name).
Create a Pull Request (PR) for review.
License This project is licensed under the MIT License. MIT License Copyright (c) 2025

Contributing Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Fork the repository. Create a feature branch (git checkout -b feature/YourFeature). Commit your changes (git commit -m 'Add some feature'). Push to the branch (git push origin feature/YourFeature). Open a pull request.

</p>

## Contact Me

Contact Us For any questions or feedback, please contact:

<p align="left">Charles Walton</p>

<p align="left">
  <a href="https://www.linkedin.com/in/cwalton1335"><img alt="LinkedIn" title="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>

<a href="mailto:cwalton1335@gmail.com"><img alt="Gmail" title="Gmail" src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>

</p>
##
Made with ❤️ and Django-Python
