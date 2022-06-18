# HoodFiller-Docker

This microservice is used to return minimum items to prepare the hood.

Steps to run 

1. docker pull mugunth78/hoodfiller:latest
2. docker run -p 9001:9001 mugunth78/hoodfiller:latest
3. After step2 hoodfiller service will up and running.then in postman use the below curl to 
   run
curl::
curl --location --request POST 'http://localhost:9001/hoodfiller/' \
--header 'Content-Type: application/json' \
--data-raw '{ 
  "hood_capacity": 41, 
  "present_weights": [2,5]
}'
