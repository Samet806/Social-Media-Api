-------------------------------Auth endpoint-----------------------------
Login - GET - /api/auth/login
Example request body:

{
    email: 'example@example.com',
    password: 'some super secret password'
}
Example request endpoint

https://api.example.com/api/auth/login
Returns:

{
    "profilePicture": "1.jpeg",
    "coverPicture": "",
    "followers": [],
    "followings": [],
    "isAdmin": false,
    "desc": "Hey friends",
    "city": "New York",
    "from": "Madrid",
    "_id": "659aa6b2c7b2d32e80579125",
    "username": "samet",
    "email": "samet@gmail.com",
    "password": "$2b$10$QB6O4MV6UN.Aj6CwInanHuHMt/PLslAK0BfQwz45dXRLDfmukfNCe",
    "createdAt": "2024-01-07T13:27:14.446Z",
    "updatedAt": "2024-01-10T13:08:42.978Z",
    "__v": 0,
    "relationship": 1
}
----------------------------------------------------------------------------------------------------------------
Register - POST - /api/auth/register
Example request body:

{
    name: 'John Doe',
    email: 'example@example.com',
    password: 'some super secret password'
}
Example request endpoint

https://api.example.com/api/auth/register
Returns:

{
    "profilePicture": "",
    "coverPicture": "2.jpeg",
    "followers": [],
    "followings": [],
    "isAdmin": false,
    "desc": "Hey Friends..",
    "city": "Kütahya",
    "from": "Türkiye",
    "_id": "659fdeb35d956b32206874c5",
    "username": "sevim",
    "email": "sevim@gmail.com",
    "password": "$2b$10$vEXaazuklG7ejvea76znmuSE3xVqdD5k18rRWQ7RZqOBF94ufsDjS",
    "createdAt": "2024-01-11T12:27:31.140Z",
    "updatedAt": "2024-01-11T12:27:31.140Z",
    "__v": 0
}
-----------------------------------------------------------------------------------------------------------------
-------------------------------User-----------------------------
Get user - GET - /api/users/?userId=659aa6b2c7b2d32e80579125
Example request endpoint

https://api.example.com/api/users/659aa6b2c7b2d32e80579125
Returns:

{
    "profilePicture": "1.jpeg",
    "coverPicture": "",
    "followers": [],
    "followings": [],
    "isAdmin": false,
    "desc": "Hey friends",
    "city": "New York",
    "from": "Madrid",
    "_id": "659aa6b2c7b2d32e80579125",
    "username": "samet",
    "email": "samet@gmail.com",
    "createdAt": "2024-01-07T13:27:14.446Z",
    "__v": 0,
    "relationship": 1
}
-----------------------------------------------------------------------------------------------
Delete user - Delete - /api/users/659aa6b2c7b2d32e80579125
Example request endpoint

https://api.example.com/api/users/659aa6b2c7b2d32e80579125
Returns:

"You can delete only your account!"

