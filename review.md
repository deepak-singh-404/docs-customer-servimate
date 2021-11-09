===============================================================================================================
**POST REVIEW**
**URL** : `/dev/api/v1/review`
**Method** : `POST`
**Header** : `application/json`
**Auth required** : NO
**Permissions required** : None
## Request Body 

```json
{
    "message": "Recent review",
    "rating": 5,
    "customerId": "61350d0f77a4e100282c06ed",
    "customerName": "Arvind Dixit",
    "bookingId": "61723e7e73cbf90050721718"
}
```
## Success Response 
**Code** : `200`
**Response**

```json
{
    "success": true,
    "statusCode": 200,
    "response": {
        "_id": "618a5ad7e63e5100663c02f6",
        "message": "Recent review",
        "rating": 5,
        "bookingId": "61723e7e73cbf90050721718",
        "customerId": "61350d0f77a4e100282c06ed",
        "customerName": "Arvind Dixit",
        "createdAt": "2021-11-09T11:26:15.059Z",
        "__v": 0
    }
}
```