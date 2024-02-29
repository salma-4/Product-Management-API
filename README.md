# Product Management API

This project implements a RESTful API for managing product details and products. It provides endpoints to perform CRUD operations on product details and retrieve product information.

### Prerequisites

- Java 8+
- Maven

## Features

1. **Insert Product**
   - Endpoint: `/api/product` (POST)
   - Endpoint: `/api/products`
   - Request Body: ProductDetails JSON object
   - Response: ProductDetails JSON object
   - Example Request Body:
    ```json
    {
    "name": "",
    "expirationDate": "2078-12-02",
    "manufacturer": "",
    "price": 10.5,
    "available": true
    }
     
   
2. **Update productDetails**:
   - Method: PUT
   - Endpoint: `/api/products`
   - Request Body: ProductDetails JSON object
   - Response: ProductDetails JSON object
   - Example Request Body:
    ```json
    {
    "id":
    "name": "",
    "expirationDate": "2078-12-02",
    "manufacturer": "",
    "price": 10.5,
    "available": true
    }
     

3. **Delete Product **: 
   - Method: DELETE
   - Endpoint: `/api/products?id=`
   - Path Variable: ID of the product to delete

4. **Get Product Details by ID**:
   - Method: GET
   - Endpoint: `/api/products/productDetailsById?id=`
   - Path Variable: ID of the product to retrieve
   - Response: ProductDetails JSON object

5. **Get Product Details by Name**:
   - Method: GET
   - Endpoint: `/api/products/productDetailsByName?searchKey=`
   - Query Parameter: Name of the product to retrieve
   - Response: ProductDetails JSON object

6. **Get All Products**:
   - Method: GET
   - Endpoint: `/api/products`
   - Response: List of Product JSON objects

7. **Get Product by ID**: 
   - Method: GET
   - Endpoint: `/api/products/productById?id=`
   - Path Variable: ID of the product to retrieve
   - Response: Product JSON object


## Documentation

The APIs are documented using Swagger. You can access the Swagger UI by navigating to `/swagger-ui.html` after starting the application.
![swagger](https://github.com/salma-4/Product-Management-API/assets/116264673/77557eae-dcc7-49c3-b075-d781ae459886)

## Postman Collection

A Postman collection containing requests for each EndPoint , import this collection into Postman to test the APIs.
![post](https://github.com/salma-4/Product-Management-API/assets/116264673/56439488-9d80-4e1a-8b5d-f6d6af4451e4)


## Testing

Test cases are written using RestTemplate to ensure the functionality of the API.

![1](https://github.com/salma-4/Product-Management-API/assets/116264673/670e83b2-194c-4238-bc47-b29710aa2d63)
![test](https://github.com/salma-4/Product-Management-API/assets/116264673/831ff62f-058c-49fb-a54a-fd92d6cbce29)


### Interacting with the API

You can interact with the API using any REST client or HTTP testing tool. The API uses JSON for request and response data(Jakson).

``` jakson dependencies
    <dependency>
      <groupId>com.fasterxml.jackson.core</groupId>
      <artifactId>jackson-databind</artifactId>
      <version>2.16.1</version>
    </dependency>
    
    
    <dependency>
      <groupId>com.fasterxml.jackson.core</groupId>
      <artifactId>jackson-core</artifactId>
      <version>2.16.1</version>
    </dependency>
