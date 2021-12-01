## Installation Instructions:

### 1. Backend server

#### Clone project (Backend)

```bash
git clone -b dev https://github.com/PinterestProject/pinterest
```

#### Install Python dependencies

```bash
python3 -m venv pinterst_env
source pinterst_env/bin/activate
pip install -U pip setuptools wheel
pip install -r pinterest/backend/requirements.txt
```

#### Initialize Database

```bash
cd pinterest/backend
python3 manage.py makemigrations
python3 manage.py migrate
# create an admin user
python3 manage.py createsuperuser
```

#### Run the Django API server

```bash
python3 manage.py runserver
```

---

### 2. Frontend app

#### Clone project (Frontend)

```bash
 git clone -b dev https://github.com/PinterestProject/Frontend
```

#### Install JavaScript dependencies

```bash
cd Frontend
npm install
```

#### Run the ReactJS app

```bash
npm start
```
