## Refresh Endpoint

#### Description
This endpoint retrieves profile data for the currently authenticated user.

#### URL

`/auth/profile/{country}/`

#### Method

`GET`

#### Request Data

None. This endpoint does not require any request data.

#### Responses

**Success Response:**

Status Code: `200`

```json
{
  "aboId": "123456",
  "aboClass": "direct_distributor",
  "currentAwardLevel": "founders_ruby",
  "highestAwardLevel": "founders_emerald",
  "currentBonusLevel": "15",
  "highestBonusLevel": "21",
  "partners": [
    {
      "partnerId": "1",
      "aboName": "John Doe",
      "firstName": "John",
      "lastName": "Doe",
      "email": "john.doe@washington.com",
      "mobileNumber": "+989905445"
    },
    {
      "partnerId": "2",
      "aboName": "Miranda Doe",
      "firstName": "Miranda",
      "lastName": "Doe",
      "email": "miranda.doe@washington.com",
      "mobileNumber": "+989975446"
    }
  ],
  "privacyFlag": true
}
```

**Failure Response:**

Status Code: `401`

Empty Response