## Logout Endpoint

#### Description
This endpoint processes a logout request for the currently authenticated user.

#### URL

`/auth/logout/`

#### Method

`POST`

#### Request Data

Send the session token of the currently authenticated user.

```json
{
  "value": "8d366f21-494b-400d-a0cb-4970687fc79a"
}
```

#### Responses

**Success Response:**

Status Code: `200`

```json
{
  "message": "success"
}
```


**Failure Response:**

Status Code: `400`

```json
{
    "message": "failure"
}
```