# Description

API service for working with the YaTube application

# Install
## How to start a project:
Clone the repository and change into it on the command line:

```
git clone https://github.com/VladBorisof/api_final_yatube.git

cd api_final_yatube
```

## Create and activate virtual environment:

```
python3 -m venv venv

source venv/bin/activate

python3 -m pip install --upgrade pip
```


## Install dependencies from requirements.txt file:

```pip install -r requirements.txt```

## Run migrations:

```python3 manage.py migrate```

## Run project:

```python3 manage.py runserver```

# Examples

run to get posts:

```GET http://127.0.0.1:8000/api/v1/posts/```

run to create posts:

```POST http://127.0.0.1:8000/api/v1/posts/```

with body

{
    "text": "post 1"
}

run to get groups:

```GET http://127.0.0.1:8000/api/v1/groups/```

run to create comments for first post:

```POST http://127.0.0.1:8000/api/v1/posts/1/comments/```

with body

{
    "text": "comment for post",
    "post": 1
}
