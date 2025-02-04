# ToDoAPI

## Prerequisites
- Python 3.11
- Virtualenv
- Postgres 16

# Getting started

## Setup Configuration Files
- Create .env file following .env.example template in "config"

```bash
DATABASE_URL=postgres://{your_user}:{your_password}@{your_host}:{your_port}/{databse_name}
```

## virtualenv
```bash
# 1. Create virtual env
cd api
python -m venv virtualenv
. virtualenv\Scripts\activate

# 2. Install dependency
pip install -r requirements/base.txt

# 3. Migrate database
python ./manage.py migrate

# 4. Start Django
python ./manage.py runserver
```

## Run Test Case
```bash
cd api
python ./manage.py test # run testcase all module
python ./manage.py test <module> # run testcase of module
```
## Django Admin
- URL: http://localhost/admin

## Swagger Document
- URL: http://localhost/docs

## API Authentication
- JWT are supported
