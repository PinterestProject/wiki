# Pinterest API
----------

### Users API

1. Signup and get an auth token 
```HTTP
POST /users/signup/
```
2. Login a user and get an auth token
```HTTP
POST /users/login/
```
3. Logout a user using the auth token
```HTTP
POST /users/logout/
````

----------

### Pin(s) API

1. User can create a pin 
```HTTP
POST /pins/api/v1/pins/
```

2. User can view all pins
```HTTP
GET /pins/api/v1/pins/
```

3. User can view a specific pin
````HTTP
GET /pins/api/v1/pins/<int:pin_id>/
````

4. User can partially update a pin they made.
````HTTP
PATCH /pins/api/v1/pins/<int:pin_id>/
````

4. User can update a pin they made.
````HTTP
PUT /pins/api/v1/pins/<int:pin_id>/
````

5. User can delete a pin they made.
````HTTP
DELETE /pins/api/v1/pins/<int:pin_id>/
````