# Restful API Testing using Postman
[Processes](#process)  -  [Test Case](#test-cases)  -  [Go to Bottom](#---)
# <h3> Tools </h3>
* API: [Restful-Booker](https://restful-booker.herokuapp.com/)
* Postman - Testing


[Video Sample of the test](https://drive.google.com/file/d/1itBFPP6wAwLZqs2mzbHjiPy1LIcaTTOs/view?usp=sharing)


# <h3> Introduction </h3>

The Restful-booker is an API that you can use to learn more about API Testing or try out API testing tools against. The API comes pre-loaded with 10 records for you to work with and resets itself every 10 minutes back to that default state. Restful-booker also comes with detailed API documentation to help get you started with your API testing straight away.

For this pupose of the portfolio the API is a great tool for demonstraiting real world scenorios specifically for businesses involing booking or record keeping.

# <h3>API Documentation</h3>
The documentation can be read here: https://restful-booker.herokuapp.com/apidoc/index.html

# <h3>Process</h3>

My approach on this is to first understand what the product requirments are in order properly set test scenarios and then build test cases based on the created test scenarios.

# <h3>Scenario</h3>

In this scenario the company is a well known hiring agency from a big city and is building an API for their appointments setting tool which they will be using in their company system to manage their appointments on future hiring processes such as interviews for their clients. The API will serve as a pioneer for the company to allow their development team to develope a web app for the public and other companies to use.

# <h3>Requirements</h3>

- Test the API if all access points are working.
- API can CREATE, READ, UPDATE, DELETE (CRUD) data & records.
- Data is correctly handled in the CRUD Processes.
- API is stable.

# <h3>Test Cases</h3>

**1 - Ping Check**

The request is a simple health check endpoint to confirm whether the API is up and running. Testing to see if a response of code status: 201 indicates the API is connected and running.

![image](https://github.com/ESMercado/Software-QA-Portfolio/assets/170240544/fe74eb94-da57-4af0-8c3c-fa270beed5b0)

**2 - Create Booking**

Setting a request to create a booking into the database through the API Post /booking

JSON body:
```
{
    "firstname" : "Elmer",
    "lastname" : "Mercado",
    "totalprice" : {{$randomPrice}},
    "depositpaid" : true,
    "bookingdates" : {
        "checkin" : "2024-01-01",
        "checkout" : "2024-01-07"
    },
    "additionalneeds" : "Dinner"
}
```

The request response must return a status code 200. After that the I set a global variable as the bookingId value to keep track the test incase an error occures.

![image](https://github.com/ESMercado/Software-QA-Portfolio/assets/170240544/0976c11b-1449-410b-a826-8a8d7f30abae)

**3 - GET all booking

Test if API can collect all created bookings in the database. Using the link ``` https://restful-booker.herokuapp.com ```

![image](https://github.com/ESMercado/Software-QA-Portfolio/assets/170240544/013c5d40-56ef-4d43-96db-071fafb39e44)

**4 - GET 1 unique booking using ID

Test if API can filter 1 booking. Using the bookingId variable in the previous step to use as a filter to 

#
[Go to Top](#restful-api-testing-using-postman)

# ---
