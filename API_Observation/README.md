1. Updating Username

PUT  /user/{username} does not return the complete user data in the response body.It contains only "code": 200, "type": "unknown", "message": "userid or username".

2.GETTING USER BY USERNAME

GET user by username and password request returns 200 status code.However, the response body does not include the complete user data.

3.CREATE USER

POST/user returnes status code 200 but the response body does not contain the created user object.

Many REST API returnes the created resource or its identifier.

4. USERSTATUS

Swagger schema defines userStatus as an integer,although many learning materials describe it as active/inactive.

5.GET PET RESPONSE

Get/pet/{petid} returnes status code 200ok,but the data in response body and the data in request body do not coincide.

6.POST PET RESPONSE

Update a pet in the store with form data through /pet/{petid} returnes only "code": 200,"type":"unknown","message":" petid".

7.DELETE AN EXISTING PET

After sending DELETE /pet/{petid} the API returnes 200ok.However, subsequent GET/pet/{petid} may still returne 200ok or returne the data that does not correspond to the deleted pet.

8.DELETE A STORE ORDER

After sending DELETE to store/order/{orderid} API returnes 200ok.The response body contains only "code":200,"type": "unknown","message":"orderid".


IMPORTANT: Swagger PetStore is a demonstration API designed for educational purposes.Some inconsistencies observed during testing are likely related to the limitations of the demo environment and should not be interpreted as defects of a production-ready system.

