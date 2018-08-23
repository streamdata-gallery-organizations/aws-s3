{
  "info": {
    "name": "AWS S3 POST Object",
    "_postman_id": "7fd8b974-c068-4473-a658-52c2192441e4",
    "description": "The POST operation adds an object to a specified bucket using HTML forms",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Object",
      "item": [
        {
          "id": "34e21cad-ee23-4bdb-8600-cc3fc41ddd9f",
          "name": "post-object",
          "request": {
            "url": "{{default}}/",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The POST operation adds an object to a specified bucket using HTML forms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7058a62e-56f2-4fa3-bdb2-907944b6b986"
            }
          ]
        }
      ]
    },
    {
      "name": "Bucket",
      "item": [
        {
          "id": "e429bb69-259a-4066-a5ed-db1b391e92be",
          "name": "delete-bucket",
          "request": {
            "url": "{{default}}/",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This implementation of the DELETE operation deletes the bucket named inthe URI"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb733830-816c-4bed-8386-ded281d36e80"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}