# gunda-api

## API Documentation

This is a lightweight web service, (REST interface), which provides an easy way to access **`gunda-api`** data.
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
- URL : [/get_assassins](http://baseapiurlgoeshere.com/get_assassins)
- MockURL : [get_assassins](http://theapache64.com/mock_api/get_json/gunda-api/get_assassins?is_skip_auth=true&is_skip_param=true)



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
    }, ... ]
  }
}
```


#### 2 . /get_pricing

- Method : **GET**
- URL : [/get_pricing](http://baseapiurlgoeshere.com/get_pricing)
- MockURL : [get_pricing](http://theapache64.com/mock_api/get_json/gunda-api/get_pricing?is_skip_auth=true&is_skip_param=true)



**Response Body**
```json
{
  "error" : false,
  "message" : "OK",
  "data" : {
    "pricing" : [ {
      "price_usd" : "2000",
      "price_inr" : "137940",
      "name" : "Left Hand Cut",
      "id" : "1"
    },... ]
  }
}
```



