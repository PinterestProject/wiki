 ### Installation Instructions:

#### Clone project (Backend)

 ````bash
 git clone -b dev https://github.com/PinterestProject/pinterest
 ````

#### Install Python dependencies
 ````bash
 python3 -m venv pinterst_env
 source pinterst_env/bin/activate
 pip install -U pip setuptools wheel
 pip install -r pinterest/backend/requirements.txt
 ````

#### Install Python dependencies
 
 ````bash
 python3 manage.py makemigrations
 python3 manage.py migrate
 python3 manage.py createsuperuser
 ````
