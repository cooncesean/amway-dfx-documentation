## Login Endpoint

#### Description
This endpoint processes a login request for an active user for a specified region.
#### URL

`/auth/login/{country}/`

#### URL Params

* `country`: The country code of the region that the Amway user belongs to.


#### Method

`POST`

#### Request Data

```json
{
  "username": "123456",
  "password": "abc123",
  "appId": "guidebook",
  "appSecret": "8pp-s3cr3t-k3y"
}
```
#### Responses

**Success Response:**

Status Code: `200`

```json
{
  "aboId": "123456",
  "message": "success",
  "token": {
    "value": "8d366f21-494b-400d-a0cb-4970687fc79a",
    "expiration": "2016-02-03 17:54:57",
    "tokenType": "bearer",
    "refreshToken": {
      "value": "f001382e-a150-4143-9336-81f75753f97b",
      "expiration": "2016-02-04 05:09:57"
    }
  }
}
```

**Failure Response:**

Status Code: `400`

```json
{
  "abo_id": "123456",
  "message": "failure"
}
```
