### **reqres API with Postman Newman**
This project demonstrates API testing using Postman, providing a collection of tests to validate various endpoints of the API.
### **Feature**
- Tests for GET, POST, PUT, DELETE requests
- Collection of tests covering different API endpoints
- Environment setup for easy switching between environments
- Pre-request scripts for data setup
- Test scripts for validations
## API Documentation
- https://documenter.getpostman.com/view/46763324/2sB3B7QaNT
### **Technoloy Used**
- Postman
- Newman
### **Prerequisite**
- Node.js
- Newman
- Newman html Report Library
### **Installation**
1. Postman: If you haven't already, [download and install Postman.](https://www.postman.com/downloads/)
2. Clone the repository:
 ```console 
  git clone https://github.com/aminulislamtutul/Rest_reqres_API_with_Newman_Report.git
```
3. Import the Postman collection:
    - Open Postman.
    - Click on the Import button.
    - Select the file from the repository.
4. Import the Postman environment:
    - In Postman, click on the gear icon in the top right corner.
    - Select **Import** and choose the file.
5. Newman and Report Installation Process:
    - Newman Install Command:
     ```console 
      npm install -g newman
    ```
    - Newman Html Report Install Command:
     ```console 
      npm install -g newman-reporter-htmlextra
    ```
### **Usage**
1. Select Environment:
    -   In Postman, select the appropriate environment (e.g., Development, Production) from the top-right dropdown.
2. Run Collection:
    -   Select the imported collection from the Collections sidebar.
    -   Click on the Runner button to open the collection runner.
    -   Select the desired environment.
    -   Click Start Test to run the collection.
3. View Results:
    -   Once the tests are complete, view the results in the Runner tab.
    -   Detailed test results can be viewed for each request.
    -   Detailed test results can be viewed for each request.
## Testing**

## Test Case Scenarios:
## Page_1
## _**1. Fetch a list of users with pagination**_
### Request URL: https://reqres.in/api/users?page=1
### Request Method: GET
 **Response Body:**:
```console
 {
    "id": 1,
    "email": "george.bluth@reqres.in",
    "first_name": "George",
    "last_name": "Bluth",
    "avatar": "https://reqres.in/img/faces/1-image.jpg"
 }
```
## _**2. Fetch a single user by ID**_
### Request URL: https://reqres.in/api/users/1
### Request Method: GET
 **Response Body:**:
```console
 {
    "id": 1,
    "email": "george.bluth@reqres.in",
    "first_name": "George",
    "last_name": "Bluth",
    "avatar": "https://reqres.in/img/faces/1-image.jpg"
 }
```
## _**3. Create a new user**_
### Request URL: https://reqres.in/api/users
### Request Method: POST
 **Request Body:** 
 ```Console
{
  "name": "Aminul",
  "job": "SQA Engineer"
}
```
**Response Body:**
```Console
{
    "name": "Aminul",
    "job": "SQA Engineer",
    "id": "716",
    "createdAt": "2025-07-30T16:50:58.230Z"
}
```
## _**4. Update an existing user**_
### Request URL: https://reqres.in/api/users/1
### Request Method: PUT
**Request Body:** 
```Console
{
  "name": "Najmus",
  "job": "MARN Stack Developer"
}
```
**Response Body:**
```Console
{
    "name": "Najmus",
    "job": "MARN Stack Developer",
    "updatedAt": "2025-07-30T16:53:07.841Z"
}
```
## _**5. Delete a user**_
### Request URL: https://reqres.in/api/users
### Request Method: DELETE
### Response Body: None 

## Page_2
## _**1. Fetch a list of users with pagination**_
### Request URL: https://reqres.in/api/users?page=2
### Request Method: GET
 **Response Body:**:
```console
 {
    "id": 7,
    "email": "michael.lawson@reqres.in",
    "first_name": "Michael",
    "last_name": "Lawson",
    "avatar": "https://reqres.in/img/faces/7-image.jpg"
}
```
## _**2. Fetch a single user by ID**_
### Request URL: https://reqres.in/api/users/7
### Request Method: GET
 **Response Body:**:
```console
 {
    "id": 7,
    "email": "michael.lawson@reqres.in",
    "first_name": "Michael",
    "last_name": "Lawson",
    "avatar": "https://reqres.in/img/faces/7-image.jpg"
}
```
## _**3. Create a new user**_
### Request URL: https://reqres.in/api/users
### Request Method: POST
 **Request Body:** 
 ```Console
{
  "name": "Aminul",
  "job": "SQA Engineer"
}
```
**Response Body:**
```Console
{
    "name": "Aminul",
    "job": "SQA Engineer",
    "id": "820",
    "createdAt": "2025-07-30T16:50:58.230Z"
}
```
## _**4. Update an existing user**_
### Request URL: https://reqres.in/api/users/7
### Request Method: PUT
**Request Body:** 
```Console
{
  "name": "Najmus",
  "job": "MARN Stack Developer"
}
```
**Response Body:**
```Console
{
    "name": "Najmus",
    "job": "MARN Stack Developer",
    "updatedAt": "2025-07-30T16:53:07.841Z"
}
```
## _**5. Delete a user**_
### Request URL: https://reqres.in/api/users
### Request Method: DELETE
### Response Body: None 
## Run Command:  
- Run Command for Console:
```console
newman run reqres_API_Collections.postman_collection.json -e reqres_API_Environments.postman_environment.json
```
- Run Command for Report: 
```console
newman run reqres_API_Collections.postman_collection.json -e reqres_API_Environments.postman_environment.json -r cli,htmlextra
```
## Newman Report Summary:

<img width="662" height="415" alt="Screenshot 2025-07-30 014029" src="https://github.com/user-attachments/assets/f44da2d3-0120-472f-8861-13d54e83a357" />
<img width="662" height="269" alt="Screenshot 2025-07-30 014104" src="https://github.com/user-attachments/assets/7fc3bf3b-1264-433a-bcea-1ee5bcfc6cd1" />
<img width="662" height="206" alt="Screenshot 2025-07-30 014123" src="https://github.com/user-attachments/assets/94117f4f-f0f5-4f7f-ab34-247eb29ad009" />
<img width="662" height="205" alt="Screenshot 2025-07-30 014139" src="https://github.com/user-attachments/assets/51e04e3a-003f-4ed4-9873-eaea7bb6292b" />






