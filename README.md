# IBM Full Stack Certificate
## Application Development using Microservices and Serverless

### Week 2: Web API Essentials: RESTAPI and GraphQL

## Hands-on Lab: Creating a Hello World REST API with Python and Flask

1. Setup Flask server.py

2. Install Flask

$ python3 -m pip install flask

3. start server at port 5000

$ python3 server.py

4. ctrl + c to stop server

## Hands-on Lab: CRUD Operations with Python

1. git clone: 

$ [ ! -d 'jmgdo-microservices' ] && git clone <https://github.com/ibm-developer-skills-network/jmgdo-microservices.git>

$cd jmgdo-microservices/CRUD

$ ls

2. install packages:

$ python3 -m pip install flask flask_cors

3. Run and test the server with cURL

$ python3 products.py

* open another terminal

$ curl <http://localhost:5000/products>

$ curl -X POST -H "Content-Type: application/json" \
    -d '{"id": 145, "name": "Pen", "price": 2.5}' \
    <http://localhost:5000/products>

* Verify if the product is added by running the following command:

$ curl <http://localhost:5000/products/145>

## Hands-on lab: Creating a Swagger Documentation REST API

1. Getting your application started

$ git clone <https://github.com/ibm-developer-skills-network/jmgdo-microservices.git>

$ cd jmgdo-microservices/swagger_example

$ python3 -m pip install flask_cors

* start the application on port number 5000

$ python3 app.py

* copy the url on the address bar

* paste the URL where it says **<your application url \>** without the protocol (https://)

* copy the entire content of the file to https://editor.swagger.io/