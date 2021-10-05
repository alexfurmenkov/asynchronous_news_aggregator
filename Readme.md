##News Aggregator

The service provides a RESTful API for getting news from different news providers:
* NY times
* Washington Post

The app uses JWT authentication with RSA encryption. 


###Stack:
* Framework: AIOHttp
* ORM: Pewee Async


###Running the app
### Running the tests


###API Description

* `GET /news` returns news from all providers.
* `GET /news/ny-times` returns news from NY Times.
* `GET /news/w-post` returns news from Washington Post.

All endpoints accept optional query parameters: 
1. ISO string `start_date`: YYYY-MM-DD 
2. ISO string `end_date`: YYYY-MM-DD

Examples: 

`GET /news?start_date=2021-02-10&end_date=2021-03-25`

`GET /news/w-post?start_date=2021-02-10&end_date=2021-03-25`