{
  "info": {
    "name": "Blazemeter Get User Collections",
    "_postman_id": "ef3c1070-c3bf-4bd4-a608-ac08ad8cd34f",
    "description": "Get user collections.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "4a316407-98e5-4009-978d-6aab7f357d1f",
          "name": "retrieveCollections",
          "request": {
            "url": "http://a.blazemeter.com/api/v4/user/collections?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get user collections."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cf9a5e6-7c77-4733-b05b-7b2b1019d1e5"
            }
          ]
        }
      ]
    }
  ]
}