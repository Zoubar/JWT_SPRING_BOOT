//Registration 

POST http://localhost:8080/api/v1/auth/register
Content-Type: application/json

{
  "firstname": "Yassine",
  "lastname": "Zoubairi",
  "email":  "Yassine@mail.com",
  "password": "12345",
  "role":  "ADMIN" or "MANAGER"
}

//Login 

POST http://localhost:8080/api/v1/auth/authenticate
Content-Type: application/json

{
  "email":  "Yassine@mail.com",
  "password": "12345"
}

//Change password

PATCH http://localhost:8080/api/v1/users
Content-Type: application/json
Authorization: Bearer {{auth-token}}

{
  "currentPassword": "password",
  "newPassword": "newPassword",
  "confirmationPassword":  "newPassword"
}






