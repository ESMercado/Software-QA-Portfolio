# Restful API Testing using Postman

**Tools**
* API: [Restful-Booker](https://restful-booker.herokuapp.com/)
* Postman - Testing
* Newman - Reporting
#

**Introduction**

The Restful-booker is an API that you can use to learn more about API Testing or try out API testing tools against. The API comes pre-loaded with 10 records for you to work with and resets itself every 10 minutes back to that default state. Restful-booker also comes with detailed API documentation to help get you started with your API testing straight away.

For this pupose of the portfolio the API is a great tool for demonstraiting real world scenorios specifically for businesses involing booking or record keeping.
#

**API Documentation**
The documentation can be read here: https://restful-booker.herokuapp.com/apidoc/index.html
#

**Process**

My approach on this is to first understand what the product requirments are in order properly set test scenarios and then build test cases based on the created test scenarios.

**Scenario**

In this scenario the company is a well known hiring agency from a big city and is building an API for their appointments setting tool which they will be using in their company system to manage their appointments on future hiring processes such as interviews for their clients. The API will serve as a pioneer for the company to allow their development team to develope a web app for the public and other companies to use.
#

**Requirements**

- Test the API if all access points are working.
- API can CREATE, READ, UPDATE, DELETE (CRUD) data & records.
- Data is correctly handled in the CRUD Processes.
- API is stable.

**Test Cases**

| Requests                        | Tests                             |
|---------------------------------|-----------------------------------|
| **POST**                        | **Status code is 200**            |
| auth                            | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| Comments                       | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **POST**                        | **Status code is 200**            |
| create booking                  | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
|                                 | **Booking record retreaved**      |
|                                 | pm.test('Booking record retreaved', () => {<br> if (resp) {<br> pm.globals.set('bookingId', resp.bookingid);<br> pm.globals.set('fName', 'Elmer');<br> pm.globals.set('lName', 'Mercado');<br>}<br>}); |
| **GET**                         | **Status code is 201**            |
| health check                    | pm.test('Status code is 201', () => {<br> pm.response.to.have.status(201);<br>}); |
| **GET**                         | **Status code is 200**            |
| get all booking                 | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **GET**                         | **Status code is 200**            |
| show 1 booking                  | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **GET**                         | **Status code is 200**            |
| filter by first name            | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **GET**                         | **Status code is 200**            |
| filter by last name             | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **GET**                         | **Status code is 200**            |
| filter by book in date          | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **GET**                         | **Status code is 200**            |
| filter by book out date         | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **GET**                         | **Status code is 200**            |
| filter by book in & out date    | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **PUT**                         | **Status code is 200**            |
| update booking                  | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **PATCH**                       | **Status code is 200**            |
| partial update name booking     | pm.test('Status code is 200', () => {<br> pm.response.to.have.status(200);<br>}); |
| **DEL**                         | **Status code is 201**            |
| partial update name booking Copy| pm.test('Status code is 201', () => {<br> pm.response.to.have.status(201);<br>}); |

