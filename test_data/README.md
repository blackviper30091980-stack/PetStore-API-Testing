1.INTRODUCTION

This document defines the valid and invalid test data used to verity the functionality and input validation of the Swagger PetStore API.
The test data is organized by API module:Pet, Store and User.

2. PET MODULE
   
Pet ID

valid data:positive integer,unique ID( for creating a new pet),existing ID (for retrieving, updating or deliting a pet), not null;

invalid data: negative integer,letters,special characters,empty value, null.

Name

valid data: Latin and Cyrilic capital and lowercase letters,diacritics,hyphen,apostrophes;

invalid data: figuresial symbols(exepting hyphen and apostrophes),null,empty value.

Status

valid data: available,pending,sold;

invalid data: any other value,numbers,null,empty value,special characters.

Category

valid data: existing pet category names(e.g.,Dogs,Cats,Birds,Fish),Latin letters,not null;

invalid data: non-pet category names,numbers,special characters,empty value,null.



Tag

valid data: valid tag name;

invalid data: empty value,null,invalid tag name.

Photo URL

valid data: valid HTTP URL,valid HTTPS URL;

invalid data: malformed URL,missing protocol,empty value,null.

3. STORE MODULE
   
Pet ID

valid data:positive integer,unique ID( for creating a new pet),existing ID (for retrieving, updating or deliting a pet), not null;

invalid data: negative integer,letters,special characters,empty value, null.

Order ID

valid data:positive integer,unique ID( for creating a new order),existing ID (for retrieving, updating or deliting a order), not null;

invalid data: negative integer,letters,special characters,empty value, null.

Ship Date

valid data: valid date and time in ISO 8601 format;

invalid data: invalid date format,invalid month or day,lettes,empty value,null.

Status

valid data: placed,approved,delivered;

invalid data: available,pending,sold,any other values,numbers,special characters,empty value,null.

Quantity

valid data: positive numbers(excepts 0,decimals,fractions);

invalid data: null,0,empty value,negative numbers.

4. USER MODULE
   
User ID

valid data:positive integer,unique ID( for creating a new user),existing ID (for retrieving, updating or deliting a user), not null;

invalid data: negative integer,letters,special characters,empty value, null.

User Name( first name,last name)

valid data: Latin and Cyrilic capital and lowercase letters,diacritics,hyphen,apostrophes;

invalid data: figuresial symbols(exepting hyphen and apostrophes),null,empty value.

User email

valid data: valid email address,Latin uppercase and lowercase letters,numbers,dot(.),hyphen(-),underscore(_),symbol(@),maximum length:254 characters;

invalid data:missing (@),missing domain,invalid domain,leading dot in the local part,spaces,tabs,new line,unsupported special characters,emoji,empty value,null.

User status

valid data: active,inactive;

invalid data: any other value than active or inactive,misspeled values(e.g.,active,inactive),numbers,special charactes,empty value,null.

Password

valid data: letters,numbers,special characters,combination of lettes,numbers and special charactes,not null;

invalid data: empty value ,null.

Phone Number

valid data: digits,international format,digits with spaces or hyphens(if accepted by the API),not null;

invalid data: letters,emoji,special characters(except +,cpaces or hyphens if supported),empty value,null.


Test data was prepared based on the Swagger PetStore specifications.Additional values were verified during API testing using Postman.

