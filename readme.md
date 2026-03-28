# Postman API Practice Project

This project demonstrates hands-on **API testing using Postman** with RESTful methods and test validations.
It was created as a practice project to strengthen **QA Automation / SDET API testing skills**.

## Project Overview

The collection covers end-to-end **CRUD operations** using the sample REST API from **JSONPlaceholder**.

### APIs Covered

* **GET Users** → Retrieve all users
* **GET Single User** → Retrieve a specific user by ID
* **POST Create User** → Create a new user profile
* **PUT Update User** → Update existing user details
* **DELETE User** → Delete a user
* **GET Posts by User** → Fetch posts using query parameters

---

## Tools & Technologies

* **Postman**
* **REST API Testing**
* **JSON**
* **Environment Variables**
* **Collection Runner**
* **GitHub**

---

## Base URL

```text
https://jsonplaceholder.typicode.com
```

---

## Key Features Implemented

* CRUD API validation
* Request and response body validation
* Status code assertions
* Query parameter testing
* Environment variable usage (`{{baseUrl}}`)
* Collection Runner execution
* Post-response test scripts

---

## Sample Test Validation

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response is not empty", function () {
    let jsonData = pm.response.json();
    pm.expect(jsonData.length).to.be.above(0);
});
```

---

## Purpose

This project demonstrates practical API testing workflow similar to real-world QA automation activities such as:

* validating REST endpoints
* verifying status codes
* checking response payload
* executing regression flows
* reusable environment configurations

---

## Author

**Shiva Kumar**
QA Automation Engineer | SDET
Skills: Selenium | Postman | API Testing | SQL | Playwright
