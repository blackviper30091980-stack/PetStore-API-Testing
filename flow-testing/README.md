FIELD: DESCRIPTION

FLOW 1. PET LIFECYCLE

 Flow ID:  FT_001

 Module:  Pet

 Title:  create, verify, update and delete a pet

 Objective: verify the complete lifecycle of a pet by creating,retrieving,updating and deleting it through the Pet API endpoints

 Preconditions: petstore API is available; valid test data is available

 Test Data:  pet ID,pet name,tag,pet status,photoURL,category

 Steps: 

 Step 1.

 Method : POST

 Endpoint: /pet

 create a new pet

 Step 2.

 Method: GET

 Endpoint: /pet/{petid}

 find a created pet by ID

 Step 3.

 Method: PUT

 Endpoint: /pet

 update an existing pet,update a pet status

 Step 4.

 Method: DELETE

 Endpoint: /pet/{petid}

 delete an exisisting pet

 Step 5.

 Method: GET

 Endpoint: /pet/{petid}

 find  a deleted pet by ID

 Expected Result:
 
 - pet created ,status code 200;
  
 - GET returns the created pet,status code 200;
  
 - pet status is updated ,status code 200;
  
 - pet is deleted ,status code 200;
   
 - deleted pet is not found,status code 404



 FLOW 2.  ORDER LIFECYCLE

 Flow ID:  FT_002

 Module:  Store

 Title: create,retrieve and delete an order

 Objectives: verify the complete lifecycle of an order by creating,retrieving and deleting it through pet API endpoints 

 Preconditions: petstore API is available; valid test data is available

 Test Data: order ID,pet ID, shipDate,quantity,order status,complete

 Steps:

 Step 1.

 Method: POST

 Endpoint:/store/order

 place an order for a pet

 Step 2.

 Method: GET

 Endpoint: /store/order/{orderid}

 find purcharse order by ID

 Step 3.

 Method: DELETE

 Endpoint: /store/order{orderid}

 delete purcharse order by ID

 Step 4.

 Method: GET

 Endpoint: /store/order/{orderid}

 find a deleted purchase order by ID

 Expected Result:
 - an order for a pet is created,status code 200;
- a purcharse order is found  by ID,status code 200;
 - a purcharse order is deleted by ID,status code 200;
 - deleted purcharse order is not found ,satus code 404



FLOW 3. USER LIFECYCLE

Flow ID:  FT_003

Module:  User

Title: create,verify,update and delete a user

Objectives: verify the complete lifecycle of a user by creating,retrieving,updating and deleting it through pet API endpoints

Preconditions: petstore API is available; valid test data is available

Test Data: user ID,username,first name,last name,email,password,phone,userStatus

Steps:

Step 1.

Method: POST

Endpoint: /user

create user

Step 2.

Method: GET

Endpoint: /user/{username}

get user by username

Step 3.

Method: PUT

Endpoint:/user/{username}

update an existing user,update username

Step 4.

Method: GET

Endpoint: /user/{username}

get updated user by username

Step.5

Method: DELETE

Endpoint:/user/{username}

delete an existing user

Step 6.

Method: GET

Endpoint: /user/{username}

get a deleted user by username

Expected Result:

- user is created,status code 200;
  
- GET returns the created user,status code 200;
  
- username is updated,status code 200;

- GET returns the updated user;
  
- an existing user is deleted,status code,200;
  
- deleted user is not found,status code 404
  




 
