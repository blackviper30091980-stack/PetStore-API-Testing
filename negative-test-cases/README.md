FIELD / DESCRIPTION
1.

Test Case ID:  TC_API_oo1

Module:  Pet

Method:  PUT

Endpoint:  /pet

Preconditions: Pet ID already exist in the system

Test Data:   pet ID,category Id,name,photoURL,tag,status

Steps:  1.Send a PUT request to /pet without pet ID to update pet data

2.Observe the response

Expected Result: Status code 500.Response body contains the message:"something bad happened"


2.

Test Case ID:   TC_API_002

Module:   Pet

Method: GET

Endpoint: /pet/{petid}

Preconditions: Pet ID already exist in the system

Test Data: pet ID

Steps:  1. Send a GET request to /pet/{petid} with invalid pet ID

2. Observe the response

Expected Result: Status code 404,not found.Response body does not contains any data.


3.

Test Case ID:   TC_API_003

Module:  Store

Method:  POST

Endpoint:  /store/order

Preconditions: Store order does not exist it the system

Test Data: order ID,pet ID,quatity,shipDate,status,complete

Steps:  1.Send o post request to /store/order with invalid quantity value to create a store order

2. Observe the response

Expected Result: Status code 400,bad request.Response body contains the message:"bad input"


4.

Test Case ID:   TC_API_004

Module:  Store

Method: DELETE

Endpoint:  /store/order/{orderid}

Preconditions: Store order  exists in the system

Test Data: order ID

Steps:  1. Send a delete request to /store/order/{orderid} to delete the store orde with invalid value

2. Observe the response

Expected Result: Status code 404,not found.Response body does not contains any data.


5.

Test Case ID:   TC_API_005

 Module: User

 Method: POST

 Endpoint:  /user

 Preconditions: User does not exists in the system

 Test Data: user ID,username,first name,last name,email,password,userStatus,phone

 Steps: 1. Send a post request to /user to create a user in the system with invalid id value

 2. Observe the response

Expected Result: status code 400,bad request.Response does not contains any data.


6.

Test Case ID:  TC_API_006

Module: User

Method:  PUT

Endpoint: /user

Preconditions: User already exists in the system

Test Data: user ID,username,first name,last name, email,password,phone,userStatus

Steps:  1. Send a put request to /user to update userdata with invalid username value

2. Observe the response

Expected Result: Status code 405,method not allowed.Response body does not contains any data.



