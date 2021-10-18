===============================================================================================================
**APPLY COUPON**
**URL** : `dev/api/v1/voucher`
**Method** : `POST`
**Header** : `application/json`
**Auth required** : NO
**Permissions required** : None
## Request Body 

```json
{
    "couponCode":"PRAMOD50",
    "customerId":"6131e2650bb1eb002f6ae8b7"
}
```
## Success Response 
**Code** : `200`
**Response**

```json
{
    "message": "Coupon successfully applied",
    "success": true,
    "response": {
        "couponApplicableServices": [
            {
                "quantity": 1,
                "createdAt": "2021-09-15T05:47:30.403Z",
                "_id": "614188f2456da200213b0fde",
                "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                "serviceId": "613a1ad900c2e7005be3eaf0",
                "serviceName": "All in one ",
                "actualPrice": 1838,
                "discountedPrice": 1378
            },
            {
                "quantity": 1,
                "createdAt": "2021-09-15T05:47:34.807Z",
                "_id": "614188f6df4a490028b3e73a",
                "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                "serviceId": "613cdc1f896e500021025183",
                "serviceName": "Honey Wax (Full Arms, Underarms & Legs) + Threading",
                "actualPrice": 850,
                "discountedPrice": 499
            },
            {
                "quantity": 1,
                "createdAt": "2021-09-15T05:47:39.833Z",
                "_id": "614188fb2c4ba1005b6130b1",
                "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                "serviceId": "613cddb02f6d8a004c98544d",
                "serviceName": "Face & Neck Bleach (OXY)",
                "actualPrice": 230,
                "discountedPrice": 190
            }
        ],
        "totalAmount": 2067,
        "discountAfterCoupon": 2013,
        "discount": 54,
        "couponType": "rupee"
    },
    "statusCode": 200
}
```
===============================================================================================================