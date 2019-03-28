# gunda_api

## API Documentation

This is a lightweight web service, (REST interface), which provides an easy way to access **`gunda_api`** data.
The API works through simple commands, so there should not be a problem coding some nice applications.
This API contains total **2** route(s)


## API Endpoints

All the API endpoints return the same data structure as below

|Returned Key|Description|Example|
|------------|-----------|-------|
|error|The returned status for the API call, can be either 'true' or 'false'|true|
|message|Either the error message or the successful message|OK|
|data|If 'error' is returned as 'false' the API query results will be inside 'data'|data|


**Success Response Format**

```json
{
    "error": false,
    "message": "SUCCESS_MESSAGE",
    "data": {}
}
```

**Error Response Format**

```json
{
    "error": true,
    "message": "ERROR_MESSAGE"
}
```

## Routes



#### 1 . /get_assassins

- Method : **GET**
- URL : [/get_assassins](http://localhost:8080/mock_api/get_json/gunda_api/get_assassins)
- MockURL : [get_assassins](http://theapache64.com/mock_api/get_json/gunda_api/get_assassins?is_skip_auth=true&is_skip_param=true)



**Response Body**
```json
{
  "error" : false,
  "message" : "OK",
  "data" : {
    "assassins" : [ {
      "image_url" : "https://image-archive.hitmanforum.com/hitmanforum/original/2X/d/d093f2431aa45e6e45d43da9c585e8515fcfc999.jpg",
      "name" : "Hitman",
      "mobile" : "1234567890",
      "specialization" : "Quick Killing",
      "id" : "1"
    }, {
      "image_url" : "https://cdn.flickeringmyth.com/wp-content/uploads/2018/04/John-Wick-2-600x336.jpg",
      "name" : "John Wick",
      "mobile" : "6346456434",
      "specialization" : "Quick Killing",
      "id" : "2"
    }, {
      "image_url" : "",
      "name" : "Thammanam Shaji S",
      "mobile" : "34534534345",
      "specialization" : "Left Hand Cut",
      "id" : "3"
    }, {
      "image_url" : "",
      "name" : "Nizarka",
      "mobile" : "53543453453",
      "specialization" : "Slow Killing",
      "id" : "4"
    } ]
  }
}
```


#### 2 . /get_pricing

- Method : **GET**
- URL : [/get_pricing](http://localhost:8080/mock_api/get_json/gunda_api/get_pricing)
- MockURL : [get_pricing](http://theapache64.com/mock_api/get_json/gunda_api/get_pricing?is_skip_auth=true&is_skip_param=true)



**Response Body**
```json
{
  "error" : false,
  "message" : "OK",
  "data" : {
    "pricing" : [ {
      "price_usd" : "2000",
      "price_inr" : "138021",
      "name" : "Left Hand Cut",
      "id" : "1"
    }, {
      "price_usd" : "2000",
      "price_inr" : "138021",
      "name" : "Right Hand Cut",
      "id" : "2"
    }, {
      "price_usd" : "3500",
      "price_inr" : "241536.75",
      "name" : "Both Hand Cut",
      "id" : "3"
    }, {
      "price_usd" : "3000",
      "price_inr" : "207031.5",
      "name" : "Left Leg Cut",
      "id" : "4"
    }, {
      "price_usd" : "3000",
      "price_inr" : "207031.5",
      "name" : "Right Leg Cut",
      "id" : "5"
    }, {
      "price_usd" : "5800",
      "price_inr" : "400260.9",
      "name" : "Both Legh Cut",
      "id" : "6"
    }, {
      "price_usd" : "10000",
      "price_inr" : "690105",
      "name" : "Head Cut",
      "id" : "7"
    }, {
      "price_usd" : "6000",
      "price_inr" : "414063",
      "name" : "Kidnapping",
      "id" : "8"
    }, {
      "price_usd" : "9000",
      "price_inr" : "621094.5",
      "name" : "Killing",
      "id" : "9"
    }, {
      "price_usd" : "10000",
      "price_inr" : "690105",
      "name" : "Quick Killing",
      "id" : "10"
    }, {
      "price_usd" : "20000",
      "price_inr" : "1380210",
      "name" : "Slow Killing",
      "id" : "11"
    }, {
      "price_usd" : "8000",
      "price_inr" : "552084",
      "name" : "Brain Injury",
      "id" : "12"
    } ]
  }
}
```



