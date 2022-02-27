---------Get All Users--------
(GET) > https://zomatologin.herokuapp.com/api/auth/users


--------Register--------
(POST) > https://zomatologin.herokuapp.com/api/auth/register
        {"name":"Bhushan","email":"bhushan@gmail.com","password":"12345678","role":"Admin"}

--------Login--------
(POST) > https://zomatologin.herokuapp.com/api/auth/login
(Body) => {"email": "bhushan@gmail.com","password": "12345678"}
(response) => {"auth": true,"token": "token"}


--------UserInfo--------
(GET) > https://zomatologin.herokuapp.com/api/auth/userinfo
(Header) => {'x-access-token':'token from login'}