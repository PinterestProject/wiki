# Hide Database configs
----------

### 1. Install [python-dotenv](https://github.com/theskumar/python-dotenv) 

```bash
pip install -U python-dotenv
```

### 2. Add config data to .env file

```txt
NAME='pinterestdb'
USER='markgm'
PASSWORD='$uperHarDP@$sw0rD'
HOST='localhost'
PORT='5432'

BASE_DIR='/home/sedosona/Documents/'
FRONT_NAME='Frontend'
STATIC='/build/static'
BUILD='/build'
```

### 3. Load secrets in your django app

````python
# project/settings.py

from dotenv import dotenv_values

secrets = dotenv_values(f'{BASE_DIR}/.env')

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': secrets['DATABASE'],
        'USER': secrets['USER'],
        'PASSWORD': secrets['PASSWORD'],
        'HOST': secrets['HOST'],
        'PORT': secrets['PORT'],
    }
}
````
