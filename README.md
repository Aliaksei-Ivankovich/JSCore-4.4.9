# JSCore-4.4.9

//---Register a new user---//

    //Request: 
        method: POST
        endpoint: https://blog.kata.academy/api/users
        body: {
                "user": {
                  "username": "newUser",
                  "email": "newUserMail@gmail.com",
                  "password": "newUserPassword"
                  }
                }

     //Response: 
        {
            "user": {
                "username": "newuser",
                "email": "newusermail@gmail.com",
                "token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzOGM4Yjc2MjA3NTk0MWIwMGU0NmU5ZCIsInVzZXJuYW1lIjoibmV
                          3dXNlciIsImV4cCI6MTY3NTMzOTEyNiwiaWF0IjoxNjcwMTU1MTI2fQ.
                          MUqh-bngCyMh2e2lNWsZ9Cumimp_mNUlikCbP2caHKk"
            }
        }
        
    
//---Login for existing user---//

    //Request: 
        method: POST
        endpoint: https://blog.kata.academy/api/users/login
        body: {
                "user": {
                  "email": "newusermail@gmail.com",
                  "password": "newUserPassword"
                }
              }   
              
     //Response: 
        {
          "user": {
              "username": "newuser",
              "email": "newusermail@gmail.com",
              "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzOGM4Yjc2MjA3NTk0MWIwMGU0NmU5ZCIsInVzZXJuYW1lIjoibmV3dXNlciIsImV4cCI6MTY3NTMz
                        OTY1NCwiaWF0IjoxNjcwMTU1NjU0fQ.hJAUXGCZgzZgazvLOn-7EXxhA-3EWyCdRrh5GV2MVP4"
          }
        }
        
        
//---Gets the currently logged-in user---//

    //Request: 
        method: GET
        endpoint: https://blog.kata.academy/api/user
        Authorization: Bearer Token
        
    //Response: 
        {
          "user": {
              "username": "newuser",
              "email": "newusermail@gmail.com",
              "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzOGM4Yjc2MjA3NTk0MWIwMGU0NmU5ZCIsInVzZXJuYW1lIjoibmV3dXNlciIsImV4cCI6MTY3NTMzOTc0
                        OSwiaWF0IjoxNjcwMTU1NzQ5fQ.4JQ_9X9pji9B04JObMIJkIKOFEc-ZrLkKqsyoC9jxeM"
          }
        }
    
    
    
    
    
    
