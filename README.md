# Yatube REST API

A REST API for the Yatube blogging social network. It works with posts, comments, groups and follows, and uses JWT authentication.

Built in 2022 as part of the Yandex Practicum Python Developer course.

## Features

- Endpoints for the project's models: posts, groups, comments and follows.
- Supports GET, POST, PUT, PATCH and DELETE.
- Returns data in JSON.
- JWT authentication (SimpleJWT).

## Tech stack

- Python 3
- Django
- Django REST Framework
- SimpleJWT
- Pillow
- Pytest

## How to run the project

Clone the repository and go to the project folder:

```bash
git clone https://github.com/AxelVonReems/API-Yatube.git
cd API-Yatube
```

Create and activate a virtual environment:

```bash
# Windows
python -m venv venv
source venv/scripts/activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

Install the dependencies:

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

Apply the migrations and start the server:

```bash
python manage.py migrate
python manage.py runserver
```

## Example requests

API documentation:
- `/redoc/`

List all posts:
- `GET /api/v1/posts/`

All comments on post 1:
- `GET /api/v1/posts/1/comments/`

Details of group 1:
- `GET /api/v1/groups/1/`

All follows of the requesting user:
- `GET /api/v1/follow/`

## Author

Aleksei Smirnov - [GitHub](https://github.com/AxelVonReems)
