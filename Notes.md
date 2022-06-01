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
