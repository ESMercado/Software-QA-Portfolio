# Restful API Testing using Postman

**Tools**
* API: [Restful-Booker](https://restful-booker.herokuapp.com/)
* Postman - Testing
#

[Video Sample of the test](https://drive.google.com/file/d/1itBFPP6wAwLZqs2mzbHjiPy1LIcaTTOs/view?usp=sharing)


# 

<b id="introduction" > **Introduction** </b>

The Restful-booker is an API that you can use to learn more about API Testing or try out API testing tools against. The API comes pre-loaded with 10 records for you to work with and resets itself every 10 minutes back to that default state. Restful-booker also comes with detailed API documentation to help get you started with your API testing straight away.

For this pupose of the portfolio the API is a great tool for demonstraiting real world scenorios specifically for businesses involing booking or record keeping.
#

<b id="API_Documentation" > **API Documentation** <b>
The documentation can be read here: https://restful-booker.herokuapp.com/apidoc/index.html
#

<b id="Process" >**Process** </b>

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

The request is a simple health check endpoint to confirm whether the API is up and running. a response of code status: 201 indicated the API is connected and running.

![image](https://github.com/ESMercado/Software-QA-Portfolio/assets/170240544/fe74eb94-da57-4af0-8c3c-fa270beed5b0)

[Go to Top](#restful-api-testing-using-postman)
