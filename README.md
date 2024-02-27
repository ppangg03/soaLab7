READ ME
1)GET
http://localhost:8080/Lab6hibernate/rest/services/customers/
     show database


2) POST
http://localhost:8080/Lab6hibernate/rest/services/authenticate
Body -> input your data username and pwd
{
    "username": "xxx",
    "pwd": "xxx"
}
copy token ->>> "result": "XXXXXXXXXX",


3)GET
http://localhost:8080/Lab6hibernate/rest/services/customers/{username}

Headers
key "token" value "paste token"
key "Content-Type" value "application/json"

show
{
    "status": "200",
    "result": {
        "cusId": x,
        "name": "xxxxxxxxx",
        "username": "xxxxxx",
        "pwd": "xxxxxx",
        "userroles": "CLIENT",
        "phonenumbers": []
    },
    "msg": "ok"
}
