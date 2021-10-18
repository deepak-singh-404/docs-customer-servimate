===============================================================================================================
**BOOK SERVICE**
**URL** : `/dev/api/v1/bookService`
**Method** : `POST`
**Header** : `application/json`
**Auth required** : NO
**Permissions required** : None
## Request Body 

```json
{
    "customerId": "6131e2650bb1eb002f6ae8b7",
    "serviceDate": "2021-09-04",
    "address": {
        "name":"Deepak Singh",
        "address":"Tower A, 401, Supertech Ecociti",
        "phoneNumber":"+919415332242",
        "zipcode":201305,
        "city":"Noida",
        "state":"Uttar Pradesh"
    },
    "modeOfPayment": "cod",
    "isPaid": false,
    "timeSlot": "02:30 PM  -  03:00 PM",
    "finalPrice":1988,
    "cartAmount":2067,
    "coupon":{
        "name":"FEE11",
        "amount":29
    },
    "extraCharge":{
        "type":"hygenic",
        "amount":25

    }
}
```
## Success Response 
**Code** : `200`
**Response**

```json
{
    "statusCode": 201,
    "message": "Service Booked successfully",
    "success": true,
    "response": {
        "lastServiceAddress": {
            "name": "Deepak Singh",
            "address": "Tower A, 401, Supertech Ecociti",
            "phoneNumber": "+919415332242",
            "zipcode": 201305,
            "city": "Noida",
            "state": "Uttar Pradesh"
        },
        "serviceBooked": [
            {
                "coupon": {
                    "id": "613a6b47b8b0f41eec12bb88",
                    "name": "PRAMOD50",
                    "amount": 54
                },
                "extraCharge": {
                    "type": "hygenic",
                    "amount": 25
                },
                "services": [
                    {
                        "quantity": 1,
                        "createdAt": "2021-09-15T05:47:39.833Z",
                        "_id": "614188fb2c4ba1005b6130b1",
                        "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                        "serviceId": "613cddb02f6d8a004c98544d",
                        "serviceName": "Face & Neck Bleach (OXY)",
                        "actualPrice": 230,
                        "discountedPrice": 190
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
                        "createdAt": "2021-09-15T05:47:30.403Z",
                        "_id": "614188f2456da200213b0fde",
                        "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                        "serviceId": "613a1ad900c2e7005be3eaf0",
                        "serviceName": "All in one ",
                        "actualPrice": 1838,
                        "discountedPrice": 1378
                    }
                ],
                "isServiceProviderAssigned": false,
                "isJobDone": false,
                "isRequestedToCancelService": false,
                "rating": 0,
                "isCancelled": false,
                "isAdminCancelledService": false,
                "_id": "61418e3e29274c3ad4be50dd",
                "bookingId": "l8C_22iP4",
                "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
                "customerId": "6131e2650bb1eb002f6ae8b7",
                "customerName": "Deepak singh",
                "address": {
                    "name": "Deepak Singh",
                    "address": "Tower A, 401, Supertech Ecociti",
                    "phoneNumber": "+919415332242",
                    "zipcode": 201305,
                    "city": "Noida",
                    "state": "Uttar Pradesh"
                },
                "modeOfPayment": "cod",
                "isPaid": false,
                "timeSlot": "02:30 PM  -  03:00 PM",
                "serviceDate": "2021-09-04",
                "finalPrice": 1988,
                "cartAmount": 2067,
                "timeOfBooking": "2021-09-15T06:10:06.570Z",
                "createdAt": "2021-09-15T06:10:06.570Z",
                "__v": 0
            },
            {
                "services": [
                    {
                        "quantity": 6,
                        "createdAt": "2021-09-09T18:11:39.668Z",
                        "_id": "613a4e5ba12e5d002f43478f",
                        "serviceCategory": "610ba32500373d0032153036",
                        "serviceId": "613a43858196970045ec1c55",
                        "serviceName": "Demo 2 service",
                        "actualPrice": 48,
                        "discountedPrice": 45
                    },
                    {
                        "quantity": 3,
                        "createdAt": "2021-09-09T18:11:36.892Z",
                        "_id": "613a4e58621d8e004588c917",
                        "serviceCategory": "610ba32500373d0032153036",
                        "serviceId": "613a2f9db37745005b544565",
                        "serviceName": "DEEP",
                        "actualPrice": 30,
                        "discountedPrice": 25
                    }
                ],
                "isServiceProviderAssigned": true,
                "isJobDone": false,
                "isRequestedToCancelService": false,
                "rating": 0,
                "isCancelled": false,
                "isAdminCancelledService": false,
                "_id": "61417df820fb1f002fb11bba",
                "bookingId": "-0byO8Zpp",
                "serviceCategoryId": "610ba32500373d0032153036",
                "customerId": "6131e2650bb1eb002f6ae8b7",
                "customerName": "Deepak singh",
                "address": {
                    "name": "Deepak singh",
                    "address": "Tower A, 401",
                    "phoneNumber": "9415332242",
                    "zipcode": "201305",
                    "city": "Gautam Buddha Nagar",
                    "state": "Uttar Pradesh"
                },
                "modeOfPayment": "cod",
                "isPaid": false,
                "timeSlot": "03:00 PM  -  03:30 PM",
                "serviceDate": "2021-09-19",
                "timeOfBooking": "2021-09-15T05:00:40.188Z",
                "createdAt": "2021-09-15T05:00:40.188Z",
                "__v": 0,
                "serviceProvider": {
                    "isPhoneVerified": false,
                    "isPasswordUpdated": false,
                    "_id": "613d2dfe6e2f030028a2a0c6",
                    "name": "Arvind Dixit",
                    "email": "arvinddixit@gmail.com",
                    "phoneNumber": 9793482670,
                    "password": "$2a$05$BRI.UitJ.7sdZIqCfRy3p.K6FUukkkyoYEbFgbho7ZmSLcZcJ4nO6",
                    "initialPassword": "arvind@servimate",
                    "imgUrl": "",
                    "cityName": "Jaipur",
                    "cityId": "60ec422a71c75d0015dac0f6",
                    "serviceCategoryId": "610e411c5ef67b004487c5d8",
                    "serviceCategoryName": "Make-Up",
                    "remark": "Good",
                    "certificates": [],
                    "createdAt": "2021-09-11T22:30:22.972Z",
                    "__v": 0
                },
                "serviceProviderId": "613d2dfe6e2f030028a2a0c6",
                "serviceProviderName": "Arvind Dixit"
            }
        ],
        "_id": "6131e2650bb1eb002f6ae8b7",
        "phoneNumber": "+919415332242"
    }
}

```
===============================================================================================================