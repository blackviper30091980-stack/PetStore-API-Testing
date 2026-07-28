

FIELD /                                          DESCRIPTION

1.
Test Case ID:                                     TC_API_001

Module:                                            Pet

Method:                                            POST

Endpoint:                                          /pet

Preconditions:                                     PetID does not already exist in the system

Test Data:                                          Pet Name,PhotoURL,Pet status,Category,Tags,Pet ID

Steps:                                             1.Send a POST request to /pet with valid pet data
                                                   2.Observe the response

Expected Result:                                     Status code 200.
                                                   Response body contains: correct Pet ID, Pet name,Category,Photo URL,Statu
                                                   The returned data matches the request payload.


2.                   
Test Case ID:                                        TC_API_002

Module:                                                Pet

Method:                                                GET

Endpoint:                                              /pet/{petid}

Preconditions:                                         Pet with ID  already exist

Test Data:                                             Pet ID

Steps:                                                 1.Send GET request to /pet/{petID} with a valid petID
                                                      2.Observe response

Expected Result:                                       Status Code 200.
                                                      Response contains correct Pet ID


3.
Test Case ID:                                            TC_API_003   

Module:                                                   User 

Method:                                                   POST

Endpoint:                                                 /user

Preconditions:                                            User ID does not already exist in the system

Test Data                                                User ID,First Name,Last Name,email,password,phone,userStatus

Steps                                                    1.Send POST request to /user with valid user data
                                                         2.Observe the response

Expected Result:                                          Status code 200
                                                          Response body contains:user ID,First Name,Last Name,password,email,phone,userStatus.The returned data matches the request payload                       


4. 
Test Case ID:                                               TC_API_004

Module:                                                      User

Method:                                                      GET

Endpoint:                                                   /user/{username}

Preconditions:                                             User with username " " already exist

Test Data:                                                  Usename = " "

Steps:                                                      1.Send GET request to /user/{username} with a valid username
                                                           2.Observe the response

Expected result:                                            Status code 200
                                                            Response body contains:user ID,First Name,Last Name,password,phone,email, userStatus


5.
Test Case ID:                                               TC_API_005

Module:                                                     Store

Method:                                                      POST

Endpoint:                                                   /store/order

Preconditions:                                              Order ID does not exist in the system

Test Data:                                                  Order ID,pet ID,Quantity,shipDate,status,complete

Steps:                                                      1.Send POST request to /store/order with valid order data
                                                           2. Observe the response

Expected Result:                                            Status code 200
                                                           Response body contains: order ID,pet ID,Quantity,shipDate,status,complete. The returned data matches the request payload.


6.
Test Case ID:                                                TC_API_006

Module:                                                        Store

Method:                                                        GET

Endpoint:                                                     /store/order/{orderID}

Preconditions:                                                Order ID already exist in the system

Test Data:                                                    Order ID 

Steps:                                                         1.Send a GET request to /store/order/{orderID} with a valid 
                                                              order ID
                                                              2.Observe the response

Expected Result:                                              Status code 200
                                                             Response body contains: order ID,pet                                                                                         ID,Quantity,shipDate,status,complete
