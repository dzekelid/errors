{
  "info": {
    "name": "Runscope Get Buckets Errors",
    "_postman_id": "b75593ce-5ee0-436f-aa9a-bdda776e3ce9",
    "description": "Retrieve a list of error messages in a bucket",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "4e15c1fc-f936-441a-8f8c-9fe0e94678d2",
          "name": "buckets.bucketKey.errors.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey/errors"
              ],
              "query": [
                {
                  "key": "before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "bucketKey",
                  "value": "bucketKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of error messages in a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d0f1953-1a22-45de-8d5f-983f65408978"
            }
          ]
        }
      ]
    }
  ]
}