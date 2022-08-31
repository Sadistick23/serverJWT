Server on node.js, express, MongoDB, bcrypt, JWT

{

  GET http://localhost:5000/auth/users

  Header:
      -Authorization
          -Bearer (JWT TOKEN on createt auth)
          
}

{

  POST http://localhost:5000/auth/registration
  
  Body: 
      -raw (JSON)
          -{
              "username": "admin",
              "password": "admin23"
           }
           
}

{

  post http://localhost:5000/auth/login
  
  Body:
      -raw (JSON)
          -{
               "username": "admin",
               "password": "admin23"
           }
           
  "He is createt JWT token. Past this token on GET /auth/users"
  
}
