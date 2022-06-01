# send data in post method api
- make api

1. make form
2. get form value
3. test api
4. send data to api
5. test api result


# Install json server

 npm install -g json-server

# Start JSON Server

 json-server --watch db.json


# output:-
http://localhost:3000   - select users
http://localhost:3000/users

{
  "posts": [
    {
      "id": 1,
      "title": "json-server",
      "author": "typicode"
    }
  ],
  "users": [
    {
      "id": 1,
      "email": "vijay@gmail.com",
      "password": "vijay@1234"
    }
  ]
}



# postman open -->

1) GET :- get data

   step-1: past URL:- http://localhost:3000/users 

   step-2: SEND

     +

2) POST :- send data

   step-1: past URL:- http://localhost:3000/users

   step-2: click body, click raw, choose JSON, Then type:-
    {
      "id": 2,
      "email": "kumar@gmail.com",
      "password": "kumar@1234"
    }

    step-3: SEND
    
    +
    
3) PUT :- editing

   step-1: past url:- http://localhost:3000/users/2
   
   step-2: click body, click raw, choose JSON, Then type:-
    {
      "id": 2,
      "email": "kumar@gmail.com",
      "password": "kumar@123"
    }
    
   step-3: SEND
   
4) DELETE :- delete data (using id to delete the data)

   step-1: past url:- http://localhost:3000/users/2
   
   step-2: SEND
   
