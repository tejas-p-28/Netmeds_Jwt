---------Get All Users--------
(GET) > https://netmedslogin.herokuapp.com/api/auth/users


--------Register--------
(POST) > https://netmedslogin.herokuapp.com/api/auth/register
        {"name":"Bhushan","email":"bhushan@gmail.com","password":"12345678","role":"Admin"}

--------Login--------
(POST) > https://netmedslogin.herokuapp.com/api/auth/login
(Body) => {"email": "bhushan@gmail.com","password": "12345678"}
(response) => {"auth": true,"token": "token"}


--------UserInfo--------
(GET) > https://netmedslogin.herokuapp.com/api/auth/userinfo
(Header) => {'x-access-token':'token from login'}