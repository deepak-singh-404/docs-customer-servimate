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
        "review": {
            "_id": "61921fac40a510005b12811c",
            "message": "Recent review",
            "rating": 5,
            "bookingId": "61723e7e73cbf90050721718",
            "customerId": "61350d0f77a4e100282c06ed",
            "customerName": "Arvind Dixit",
            "createdAt": "2021-11-15T08:51:56.135Z",
            "__v": 0
        },
        "booking": {
            "coupon": {
                "id": "61717edc5d4272002fd5211a",
                "name": "PM11",
                "amount": 20
            },
            "extraCharge": {
                "type": "hygenicFee",
                "amount": 25
            },
            "services": [
                {
                    "quantity": 1,
                    "createdAt": "2021-10-22T04:27:47.180Z",
                    "_id": "61723dc35b3343003a49b8c7",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613a1ad900c2e7005be3eaf0",
                    "serviceName": "All in one ",
                    "actualPrice": 1837,
                    "discountedPrice": 1378
                }
            ],
            "isServiceProviderAssigned": true,
            "isJobDone": false,
            "isRequestedToCancelService": false,
            "rating": 0,
            "isCancelled": false,
            "isAdminCancelledService": false,
            "isAdminApprovedCancellationRequest": false,
            "requestedServiceProviders": [],
            "systemOrManual": 1,
            "isFeedbackGivenByCustomer": true,
            "_id": "61723e7e73cbf90050721718",
            "bookingId": "Ft3mRs_3W",
            "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
            "customerId": "61717e7dd12cd80028408c33",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401",
                "phoneNumber": "9415332242",
                "zipcode": "201305",
                "city": "Gautam Buddha Nagar",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "02:30 PM  -  03:00 PM",
            "serviceDate": "2021-10-23",
            "finalPrice": 1383,
            "cartAmount": 1378,
            "timeOfBooking": "2021-10-22T04:30:54.743Z",
            "createdAt": "2021-10-22T04:30:54.743Z",
            "approvedAt": "2021-10-22T04:30:54.743Z",
            "__v": 1,
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
    }
}
```