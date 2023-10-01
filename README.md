# OAML

Hanya untuk pengembangan diri dibeberapa bahasa pemrograman.

Terdapat beberapa fitur yaitu:

- Login
- Register
- Edit User
- Detail User
- Change Photo Profile

### Login

Endpoint: `POST` `/api/auth/login`

Response:

```
{
  "data": "..."
}
```

Request:

```
{
  "email": "email",
  "password": "password"
}
```

### Register

Endpoint: `POST` `/api/auth/register`

Reponse:

```
{
  "data": "..."
}
```

Request:

```
{
  "email": "email",
  "password": "password",
  "name": "name"
}
```

### Edit User

Endpoint: `PATCH` `/api/user/:id`

Response:

```
{
  "data": "..."
}
```

Request:

```
{
  "email": "email",
  "password": "password",
  "name": "name"
}
```

Request Header:

```
{
  "Authorization": "Bearer token"
}
```

### Detail User

Endpoint: `GET` `/api/user/:id`

Response:

```
{
  "data": {
    "email": "email",
    "name": "name",
    "photo": "photo"
  }
}
```

Request Header:

```
{
  "Authorization": "Bearer token"
}
```

### Change Photo Profile

Endpoint: `PATCH` `/api/user/profile/:id`

Response:

```
{
  "data": "..."
}
```

Request:

```
{
  "photo": "..." // File Image
}
```

Request Header:

```
{
  "Authorization": "Bearer token"
}
```
