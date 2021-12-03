# Pinterest API

---

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
```

4. Get all users

```HTTP
GET /users/users/
```

5. Get a user

```HTTP
GET /users/users/<int:user_id>/
```

6. Partially update a user data

```HTTP
PATCH /users/users/<int:user_id>/
```

7. Change user password

```HTTP
POST /users/users/changepassword/
```

8. List all user relations

```HTTP
GET /users/relation/list
```

9. Delete relations

```HTTP
DELETE /users/relation/delete
```

10. List people whom the user follows

```HTTP
GET /users/relation/followed/<int:pk>
```

11. List people who follow the user

```HTTP
GET /users/relation/follower/<int:pk>
```

12. A logged-in user can view their own account data

```HTTP
GET /users/user-details/
```

---

### Pin(s) API

1. User can create a pin

```HTTP
POST /pins/api/v1/pins/
```

2. User can view all pins

```HTTP
GET /pins/api/v1/pins/
```

3. Get pins of a board

```HTTP
GET /pins/api/v1/boards/<int:board_id>/pins/
```

4. User can view a specific pin

```HTTP
GET /pins/api/v1/pins/<int:pin_id>/
```

5. User can partially update a pin they made.

```HTTP
PATCH /pins/api/v1/pins/<int:pin_id>/
```

6. User can update a pin they made.

```HTTP
PUT /pins/api/v1/pins/<int:pin_id>/
```

7. User can delete a pin they made.

```HTTP
DELETE /pins/api/v1/pins/<int:pin_id>/
```

---

### Board(s) API

1. User can create a board

```HTTP
POST /boards/api/v1/boards/
```

2. User can view their own boards

```HTTP
GET /boards/api/v1/boards/
```

3. User can view a specific board

```HTTP
GET /boards/api/v1/boards/<int:board_id>/
```

4. User can partially update a board they made.

```HTTP
PATCH /boards/api/v1/boards/<int:board_id>/
```

5. User can update a board they made.

```HTTP
PUT /boards/api/v1/boards/<int:board_id>/
```

6. User can delete a board they made.

```HTTP
DELETE /boards/api/v1/boards/<int:board_id>/
```

---

### Comment(s) API

1. Get all comments on a pin

```HTTP
GET /comments/comment/
```

2. Post a comment on a pin

```HTTP
POST /comments/comment/
```

3. Get a comment

```HTTP
GET /comments/comment/<int:pk>
```

4. Edit a comment

```HTTP
PATCH /comments/comment/<int:pk>
```

5. Delete a comment

```HTTP
DELETE /comments/comment/<int:pk>
```
