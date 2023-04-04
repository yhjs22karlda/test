## Endpoints
- ### GET /api/bean
  - get all pruducts

- ### POST /api/bean/order
  make an order
  - request:
  ```
  {
    "userId": "BJ8hbxOmt3vIamfu",
    "order": [
      {
        "name": String,
        "price": Number
      }
    ]
  }
  ```
  response:
  ```
  {
      "eta": Number,
      "orderNr": String
  }
  ```
/api/bean/order/status/826277a9-c8b3-45a8-b402-1ff338250881
- get order status
Response: {
    "success": false,
    "msg": "Ordernumret finns inte"
}

/api/user/signup
- create user
request: 
{
  "username": "orvar",
  "password": "abc12d3"
}

response:
{
    "success": true
}

/api/user/login
- log in
request:
{
  "username": "orvar",
  "password": "abc12d3"
}

response:
{
    "success": true,
    "msg": "Inloggning lyckades BJ8hbxOmt3vIamfu"
}

/api/user/history/BJ8hbxOmt3vIamfu
- get user history
response:
{
    "success": true,
    "userId": "BJ8hbxOmt3vIamfu",
    "history": [
        {
            "orderNr": "711e9a24-083c-4a0c-a2a2-980ac37a556d",
            "totalPrice": 84,
            "orderDate": "2023-04-04 14:12:59",
            "orderDelivered": true
        },
        {
            "orderNr": "987c90bb-3c72-42b1-a20d-f863915e3f85",
            "totalPrice": 84,
            "orderDate": "2023-04-04 13:42:44",
            "orderDelivered": true
        },
        {
            "orderNr": "c7a1a610-3db9-4581-8feb-cce67ae2030b",
            "totalPrice": 84,
            "orderDate": "2023-04-04 13:42:45",
            "orderDelivered": true
        }
    ]
} 
