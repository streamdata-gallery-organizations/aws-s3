{
  "info": {
    "name": "AWS S3 PUT Bucket requestPayment",
    "_postman_id": "24c37704-87d8-4ca8-bf23-7e98aaf0171b",
    "description": "This implementation of the PUT operation uses therequestPayment subresource to set the request paymentconfiguration of a bucket",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "c8c47f79-5a36-4b31-a492-7843ccd7c015",
          "name": "put-bucket",
          "request": {
            "url": "{{default}}/",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-acl",
                "value": "{}",
                "description": "The canned ACL to apply to the bucket you are creating",
                "disabled": false
              },
              {
                "key": "x-amz-grant-full-control",
                "value": "{}",
                "description": "Allows grantee the READ, WRITE, READ_ACP, and WRITE_ACP permissions on thettttttttttttbucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read",
                "value": "{}",
                "description": "Allows grantee to list the objects in the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read-acp",
                "value": "{}",
                "description": "Allows grantee to read the bucket ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write",
                "value": "{}",
                "description": "Allows grantee to create, overwrite, and delete any object in the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write-acp",
                "value": "{}",
                "description": "Allows grantee to write the ACL for the applicable bucket",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This implementation of the PUT operation creates a new bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2925a5a-5db3-4484-b14f-9104abb1d857"
            }
          ]
        },
        {
          "id": "82c1bd19-e980-41da-959c-43b89ee23f1f",
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
              "id": "de51f2ef-a53f-4c14-acba-e2dbe2f4cb7b"
            }
          ]
        },
        {
          "id": "bfd4da0e-ae9c-442a-a5d5-dbe929697353",
          "name": "get-bucket-accelerate",
          "request": {
            "url": "{{default}}/?accelerate",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses the acceleratesubresource to return the Transfer Acceleration state of a bucket, which is eitherEnabled or Suspended"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1c906a2-4cfe-48c8-be15-7eacee8e8a0b"
            }
          ]
        },
        {
          "id": "716f48fe-53f1-4dfa-80e8-b8f039bf4db6",
          "name": "put-bucket-accelerate",
          "request": {
            "url": "{{default}}/?accelerate",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation uses the acceleratesubresource to set the Transfer Acceleration state of an existing bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "041a1178-025d-4d69-8a0d-47db2d70d907"
            }
          ]
        },
        {
          "id": "4ef5d79a-c662-4ea8-94f1-bf45a50ba4c2",
          "name": "get-bucket-acl",
          "request": {
            "url": "{{default}}/?acl",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses the aclsubresource to return the access control list (ACL) of a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5697ad84-7bc6-4745-a1c4-897ad757e254"
            }
          ]
        },
        {
          "id": "07b3d6a7-a5be-4641-86a3-0df0ccb4dd99",
          "name": "put-bucket-acl",
          "request": {
            "url": "{{default}}/?acl",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-acl",
                "value": "{}",
                "description": "Sets the ACL of the bucket using the specified canned ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-full-control",
                "value": "{}",
                "description": "Allows the specified grantee(s) the READ, WRITE, READ_ACP, and WRITE_ACPtttttttttpermissions on the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read",
                "value": "{}",
                "description": "Allows the specified grantee(s) to list the objects in the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read-acp",
                "value": "{}",
                "description": "Allows the specified grantee(s) to read the bucket ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write",
                "value": "{}",
                "description": "Allows the specified grantee(s) to create, overwrite, and delete any object in thetttttttttbucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write-acp",
                "value": "{}",
                "description": "Allows the specified grantee(s) to write the ACL for the applicabletttttttttbucket",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This implementation of the PUT operation uses the aclsubresource to set the permissions on an existing bucket using access control lists(ACL)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd8ed542-3ed7-4680-8441-5e55443fa9ca"
            }
          ]
        },
        {
          "id": "b7175117-8a0e-487c-b340-287ac586daa7",
          "name": "get-bucket-analytics-configuration",
          "request": {
            "url": "{{default}}/?analytics&amp;id=analytics-configuration-ID",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns an analytics configuration (identified bythe analytics configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b05f226-2324-4c49-b014-30c9cd5eefc6"
            }
          ]
        },
        {
          "id": "8eab77ad-d746-4e5a-a0bb-e1ae32f18ea4",
          "name": "delete-bucket-analyticsconfiguration",
          "request": {
            "url": "{{default}}/?analytics&amp;id=analytics-configuration-ID?id=%7B%7D",
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
            "description": "This implementation of the DELETE operation deletes an analytics configuration(identified by the analytics configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22b01f9d-4460-4f1a-b090-182d448df04c"
            }
          ]
        },
        {
          "id": "98d7a4df-e704-44de-8f13-1f71cffbe106",
          "name": "put-bucket-analytics-configuration",
          "request": {
            "url": "{{default}}/?analytics&amp;id=configuration-ID",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation adds an analytics configuration(identified by the analytics ID) to the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fb85743-9ec8-4f8e-a898-b6c4cb60b4a0"
            }
          ]
        },
        {
          "id": "ac7ba14e-1268-48a3-8fce-8aac6668e1e8",
          "name": "get-bucket-cors",
          "request": {
            "url": "{{default}}/?cors",
            "method": "GET",
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
            "description": "Returns the cors configuration information set for thebucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "267ce468-59ab-44e0-91d3-b540737a09d2"
            }
          ]
        },
        {
          "id": "501da634-889d-4c16-9eaf-3c12bc6b3d62",
          "name": "delete-bucket-cors",
          "request": {
            "url": "{{default}}/?cors",
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
            "description": "Deletes the cors configuration information set for the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b402906-1f24-4e09-8f3c-2b3ca0224850"
            }
          ]
        },
        {
          "id": "b8be2951-6105-416a-8607-9b7ed436528f",
          "name": "put-bucket-inventory-configuration",
          "request": {
            "url": "{{default}}/?inventory&amp;id=configuration-ID",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation adds an inventory configuration(identified by the inventory ID) to the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1e64cee-e58b-4946-8c0c-5fa263984f9e"
            }
          ]
        },
        {
          "id": "5f9b4d3c-dbb1-483b-a69e-e589d909fe0d",
          "name": "get-bucket-inventory-configuration",
          "request": {
            "url": "{{default}}/?inventory&amp;id=inventory-configuration-ID",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns an inventory configuration (identified bythe inventory configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "309eb86a-ad2a-4fe6-a684-55216d044cf7"
            }
          ]
        },
        {
          "id": "08696672-51bd-442e-bb41-67e8a8786952",
          "name": "delete-bucket-inventoryconfiguration",
          "request": {
            "url": "{{default}}/?inventory&amp;id=inventory-configuration-ID?id=%7B%7D",
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
            "description": "This implementation of the DELETE operation deletes an inventory configuration(identified by the inventory configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce1a4edd-c794-40f8-b960-2316e63f81ad"
            }
          ]
        },
        {
          "id": "c0250bfa-7d3f-43de-8271-e9dea1fd213c",
          "name": "get-bucket-lifecycle",
          "request": {
            "url": "{{default}}/?lifecycle",
            "method": "GET",
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
            "description": "NoteBucket lifecycle configuration now supports specifying lifecycle rule usingobject key name prefix, one or more object tags, or combination of both"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d799bc73-a953-407b-915f-931a9063dc17"
            }
          ]
        },
        {
          "id": "2dfeaeba-cedd-497d-86a4-7f067b4dab69",
          "name": "put-bucket-lifecycle",
          "request": {
            "url": "{{default}}/?lifecycle",
            "method": "PUT",
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
            "description": "Creates a new lifecycle configuration for the bucket or replaces an existing lifecycle configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d08814bf-06c4-4734-a5c1-87c88c2f1c69"
            }
          ]
        },
        {
          "id": "4ddee46f-308c-4998-a134-84c0aaf86746",
          "name": "delete-bucket-lifecycle",
          "request": {
            "url": "{{default}}/?lifecycle",
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
            "description": "Deletes the lifecycle configuration from the specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1d8862a-0149-4cfa-87c1-e957e804e5d3"
            }
          ]
        },
        {
          "id": "575ee958-70ef-4f3f-acb9-a716fa368a7e",
          "name": "get-bucket-list-objects-version-2",
          "request": {
            "url": "{{default}}/?list-type=2?continuation-token=%7B%7D&delimiter=%7B%7D&encoding-type=%7B%7D&fetch-owner=%7B%7D&list-type=%7B%7D&max-keys=%7B%7D&prefix=%7B%7D&start-after=%7B%7D",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns some or all (up to 1,000) ofthe objects in a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49fbda12-5193-46f9-9e1f-165da6127f4e"
            }
          ]
        },
        {
          "id": "1f4a9db0-3b09-4383-9dd4-a82d030cf845",
          "name": "get-bucket-location",
          "request": {
            "url": "{{default}}/?location",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses thelocation subresource to return a bucket's region"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d634ef2-98ba-4e4e-a3ea-283ff6dc914c"
            }
          ]
        },
        {
          "id": "2400f996-4fab-4c96-bc54-cbd2ebdd7f3c",
          "name": "get-bucket-logging",
          "request": {
            "url": "{{default}}/?logging",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses thelogging subresource to return the logging status of a bucketand the permissions users have to view and modify that status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6c79cb5-deaa-4f5d-bfde-ff44871c8a6d"
            }
          ]
        },
        {
          "id": "9aa77363-dc8f-4d7b-8740-8bfd193bf039",
          "name": "put-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics&amp;id=Id",
            "method": "PUT",
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
            "description": "Sets or updates a metrics configuration for the CloudWatch request metrics (specified by themetrics configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9788e918-c0f2-4322-9428-79aba88f18fb"
            }
          ]
        },
        {
          "id": "f30aa887-dd75-4d08-aef4-83e4c7b65f6f",
          "name": "delete-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics&amp;id=Id",
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
            "description": "Deletes a metrics configuration for the CloudWatch request metrics (specified by the metricsconfiguration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f871a12-69bd-48d9-a97f-c5d4630e0346"
            }
          ]
        },
        {
          "id": "721aa453-908b-4793-b822-12f3c50a2e7e",
          "name": "get-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics&amp;id=id",
            "method": "GET",
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
            "description": "Gets a metrics configuration for the CloudWatch request metrics (specified by the metricsconfiguration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f58ca5aa-65a1-436f-9739-90ad6c5e6002"
            }
          ]
        },
        {
          "id": "3e44c633-6dd6-4edd-9828-4f36e0264446",
          "name": "get-bucket-notification",
          "request": {
            "url": "{{default}}/?notification",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses thenotification subresource to return the notificationconfiguration of a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b01896e-142e-4657-97f0-5b585ce263fa"
            }
          ]
        },
        {
          "id": "4e2d81d2-0394-409b-8fd2-0223a105ed6e",
          "name": "put-bucket-notification",
          "request": {
            "url": "{{default}}/?notification",
            "method": "PUT",
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
            "description": "The Amazon S3 notification feature enables you to receive notifications when certain eventshappen in your bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbd0a2ef-1c21-477e-9fc4-a23109453517"
            }
          ]
        },
        {
          "id": "113822a2-b651-4b74-ae68-931788c96d25",
          "name": "get-bucket-policy",
          "request": {
            "url": "{{default}}/?policy",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses the policysubresource to return the policy of a specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9582cb77-6e4b-44a4-bb54-e31898ae763e"
            }
          ]
        },
        {
          "id": "92b60314-d2ed-4820-b3d4-f72a974cc419",
          "name": "put-bucket-policy",
          "request": {
            "url": "{{default}}/?policy",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation uses the policysubresource to add to or replace a policy on a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e153df78-03c1-4175-9d2e-cc6c108256e8"
            }
          ]
        },
        {
          "id": "9a0482da-889e-4448-9f23-99fde673f87b",
          "name": "delete-bucket-policy",
          "request": {
            "url": "{{default}}/?policy",
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
            "description": "This implementation of the DELETE operation uses the policy subresource to delete the policy on a specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cf69dc9-6bf4-4d81-b955-5b008ced5cab"
            }
          ]
        },
        {
          "id": "94b4d511-d9a7-4505-ad42-7614a801c238",
          "name": "get-bucket-replication",
          "request": {
            "url": "{{default}}/?replication?AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo; API Reference &raquo; Operations on Buckets &raquo; GET Bucket replication=%7B%7D",
            "method": "GET",
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
            "description": "Returns the replication configuration information set on the      bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb3a436e-4aca-4f99-935a-7412f7dd04b5"
            }
          ]
        },
        {
          "id": "2c89919f-cf2c-48b3-bea1-38bffff9f0e2",
          "name": "put-bucket-replication",
          "request": {
            "url": "{{default}}/?replication?AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo; API Reference &raquo; Operations on Buckets &raquo; PUT Bucket replication=%7B%7D",
            "method": "PUT",
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
            "description": "In a versioning-enabled bucket, this operation creates a new replication configuration (or      replaces an existing one, if present)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cba2ba9e-72f8-42de-8a9e-95f11fb3eaf7"
            }
          ]
        },
        {
          "id": "0f3b07b3-d2c2-4ddb-992e-857a5d239e63",
          "name": "delete-bucket-replication",
          "request": {
            "url": "{{default}}/?replication",
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
            "description": "Deletes the replication subresource associated with the specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01c1a7f3-86ae-41f1-aca4-5f073a97d31d"
            }
          ]
        },
        {
          "id": "a9af30f6-2c09-475c-b230-365d991f3221",
          "name": "get-bucket-tagging",
          "request": {
            "url": "{{default}}/?tagging",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses the taggingsubresource to return the tag set associated with the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "293ce90f-d299-40a5-bd8f-9831da6b7466"
            }
          ]
        },
        {
          "id": "4e01dc7a-d5ef-4e9a-bd24-03c4ad62833e",
          "name": "put-bucket-tagging",
          "request": {
            "url": "{{default}}/?tagging",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation uses the taggingsubresource to add a set of tags to an existing bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4908d98e-145e-40b3-8e2a-45a8835eede7"
            }
          ]
        },
        {
          "id": "86331d72-4d04-459f-95f1-61a636d0c595",
          "name": "delete-bucket-tagging",
          "request": {
            "url": "{{default}}/?tagging",
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
            "description": "This implementation of the DELETE operation uses the taggingsubresource to remove a tag set from the specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7977ea0d-dac2-4766-80a2-893b9028ef1b"
            }
          ]
        },
        {
          "id": "f6cba477-46e4-4db8-b282-26125a40b419",
          "name": "get-bucket-versioning",
          "request": {
            "url": "{{default}}/?versioning",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses theversioning subresource to return the versioning state of abucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f53d2d7c-cd1c-439b-8496-f5bb69a053d0"
            }
          ]
        },
        {
          "id": "10f39f90-ed2a-46f9-b3b5-fb860e98090d",
          "name": "put-bucket-versioning",
          "request": {
            "url": "{{default}}/?versioning",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-mfa",
                "value": "{}",
                "description": "The value is the concatenation of the authenticationtttttttttdevices serial number, a space, and the value displayed on yourtttttttttauthentication device",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This implementation of the PUT operation uses theversioning subresource to set the versioning state of anexisting bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa42a05b-db6f-49fe-9940-70df2e061822"
            }
          ]
        },
        {
          "id": "c518c448-0c26-4860-8a14-b423e5b70405",
          "name": "get-bucket-object-versions",
          "request": {
            "url": "{{default}}/?versions?delimiter=%7B%7D&encoding-type=%7B%7D&key-marker=%7B%7D&max-keys=%7B%7D&prefix=%7B%7D&version-id-marker=%7B%7D",
            "method": "GET",
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
            "description": "You can use the versions subresource to list metadata about all ofthe versions of objects in a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db531c8b-ddcc-4c82-884b-c37ac7c892b5"
            }
          ]
        },
        {
          "id": "d8ca9a38-aa0f-4f6a-838e-16c687ecf5ed",
          "name": "get-bucket-website",
          "request": {
            "url": "{{default}}/?website",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns the website configurationassociated with a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d41555ae-f950-4d6f-9108-452f98574521"
            }
          ]
        },
        {
          "id": "659be1cd-13e9-48bf-98d6-04aa294008f6",
          "name": "put-bucket-website",
          "request": {
            "url": "{{default}}/?website",
            "method": "PUT",
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
            "description": "Sets the configuration of the website that is specified in thewebsite subresource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6632282d-2ba8-4a07-a19f-bf0d9ab46518"
            }
          ]
        },
        {
          "id": "0b047d82-aef8-41fc-ad65-8bbb6e03235e",
          "name": "delete-bucket-website",
          "request": {
            "url": "{{default}}/?website",
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
            "description": "This operation removes the website configuration for a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b24ed4e-62bd-4d43-981c-11d3b3626c85"
            }
          ]
        },
        {
          "id": "29f3929d-02fe-40be-9601-64cd4af46d80",
          "name": "get-bucket-requestpayment",
          "request": {
            "url": "{{default}}/?requestPayment",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses therequestPayment subresource to return the request paymentconfiguration of a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8357941-1742-43e2-8674-37cf5f60b09e"
            }
          ]
        },
        {
          "id": "b2cd06bb-a28f-499e-a98a-dec7cde14a28",
          "name": "put-bucket-requestpayment",
          "request": {
            "url": "{{default}}/?requestPayment",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation uses therequestPayment subresource to set the request paymentconfiguration of a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfdf74ed-fd7f-442a-8248-f260105b168f"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "d744efdf-dda5-4e29-8d1d-f9d209538d6d",
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
              "id": "2cfbe2ed-9440-4dc3-9502-dda0becf7e3c"
            }
          ]
        },
        {
          "id": "d4d75b78-9961-4701-b9f3-12c6c9f34657",
          "name": "put-object--copy",
          "request": {
            "url": "{{default}}/destinationObject",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation creates a copy of an object that is      already stored in Amazon S3"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43152756-83b7-4df7-8bae-2550da0f3b26"
            }
          ]
        },
        {
          "id": "ef74e6c5-d902-4cb7-abff-c2e803251752",
          "name": "get-object",
          "request": {
            "url": "{{default}}/ObjectName?response-cache-control=%7B%7D&response-content-disposition=%7B%7D&response-content-encoding=%7B%7D&response-content-language=%7B%7D&response-content-type=%7B%7D&response-expires=%7B%7D",
            "method": "GET",
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
            "description": "This implementation of the GET operation retrieves objects from Amazon S3"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63f46e9b-e97a-4f3d-a568-52d1619076cb"
            }
          ]
        },
        {
          "id": "38e81d93-6d0a-4b9f-be07-9471a9240b22",
          "name": "put-object",
          "request": {
            "url": "{{default}}/ObjectName",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation adds an object to a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "815deaca-5be5-4e9d-81d5-38b1951482ee"
            }
          ]
        },
        {
          "id": "bc7ffc7f-522e-44f0-8b54-d191c80a93f3",
          "name": "delete-object",
          "request": {
            "url": "{{default}}/ObjectName",
            "method": "DELETE",
            "header": [
              {
                "key": "x-amz-mfa",
                "value": "{}",
                "description": "The value is the concatenation of the authenticationtttttttttdevices serial number, a space, and the value displayed on yourtttttttttauthentication device",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The DELETE operation removes the null version (if there is one) of anobject and inserts a delete marker, which becomes the current version of the object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f97eec92-3533-49ff-82d3-1ce57f4d05c7"
            }
          ]
        },
        {
          "id": "876fb45b-e92d-44bc-b411-e3f2ed38b476",
          "name": "get-object-acl",
          "request": {
            "url": "{{default}}/ObjectName?acl",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses the aclsubresource to return the access control list (ACL) of an object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fec2e1f-8e8a-4160-878c-85e92ec34932"
            }
          ]
        },
        {
          "id": "23f6178a-4a2c-4f51-bff3-531317c44ebc",
          "name": "put-object-acl",
          "request": {
            "url": "{{default}}/ObjectName?acl",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-acl",
                "value": "{}",
                "description": "Sets the ACL of the object using the specified canned ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-full-control",
                "value": "{}",
                "description": "Allows the specified grantee the READ, WRITE, READ_ACP, andtttttttttWRITE_ACP permissions on the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read",
                "value": "{}",
                "description": "Allows the specified grantee to list the objects in thetttttttttbucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read-acp",
                "value": "{}",
                "description": "Allows the specified grantee to read the buckettttttttttACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write",
                "value": "{}",
                "description": "Not applicable when granting access permissions on objects",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write-acp",
                "value": "{}",
                "description": "Allows the specified grantee to write the ACL for thetttttttttapplicable bucket",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This implementation of the PUT operation uses the aclsubresource to set the access control list (ACL) permissions for an object that alreadyexists in a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2bdbdc1-9888-4a64-925c-a1dd05db5c06"
            }
          ]
        },
        {
          "id": "bab72e7b-7778-4e38-bfc2-2e8cfad41e51",
          "name": "post-object-restore",
          "request": {
            "url": "{{default}}/ObjectName?restore&amp;versionId=VersionID",
            "method": "POST",
            "header": [
              {
                "key": "Content-MD5",
                "value": "{}",
                "description": "The base64-encoded 128-bit MD5 digest of the data",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Restores a temporary copy of an archived object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9260d28-bbda-4fe8-aee9-7871162f1ccd"
            }
          ]
        },
        {
          "id": "bb1c646e-3169-4339-a9d9-657983befbd6",
          "name": "get-object-tagging",
          "request": {
            "url": "{{default}}/ObjectName?tagging",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns the tags associated with anobject"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf204830-91cd-49a1-8fc7-4465d3745f98"
            }
          ]
        },
        {
          "id": "9d02172e-6fbf-4788-8efe-c37d1c22e4fd",
          "name": "put-object-tagging",
          "request": {
            "url": "{{default}}/ObjectName?tagging",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation uses the taggingsubresource to add a set of tags to an existing object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66eae5eb-4588-41bb-8923-21000a61dcab"
            }
          ]
        },
        {
          "id": "384c271d-f5bf-4fe5-b7d7-e26f8de4abc1",
          "name": "get-object-torrent",
          "request": {
            "url": "{{default}}/ObjectName?torrent",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses thetorrent subresource to return torrent files from a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "960511f6-43a9-40e3-80af-11e98e48ad4b"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "57d05fe4-41aa-425e-a3bf-a428a88537c0",
          "name": "list-bucket-analytics-configurations",
          "request": {
            "url": "{{default}}/?analytics?ContinuationToken=%7B%7D",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns a list of analyticsconfigurations for the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "651b999f-8ef3-493a-ab57-da40fbc6084e"
            }
          ]
        },
        {
          "id": "a86967a0-210c-4de2-9864-f0ef41044bb6",
          "name": "list-bucket-inventory-configurations",
          "request": {
            "url": "{{default}}/?inventory?ContinuationToken=%7B%7D",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns a list of inventoryconfigurations for the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bad1c49c-cc67-4077-a4f7-4fbb6e770830"
            }
          ]
        },
        {
          "id": "da882aec-0750-46c2-9e23-f60d890470ff",
          "name": "list-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics?BucketName=%7B%7D&ContinuationToken=%7B%7D",
            "method": "GET",
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
            "description": "Lists the metrics configurations for the CloudWatch request metrics of the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c1d49cd-cfe0-4a03-95bc-7a0f2c84fce5"
            }
          ]
        },
        {
          "id": "a66369cd-5fb1-4d9e-b55a-d3bb36d5fd8b",
          "name": "list-multipart-uploads",
          "request": {
            "url": "{{default}}/?uploads?delimiter=%7B%7D&encoding-type=%7B%7D&key-marker=%7B%7D&max-uploads=%7B%7D&prefix=%7B%7D&upload-id-&#8203;marker=%7B%7D",
            "method": "GET",
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
            "description": "This operation lists in-progress multipart uploads"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a8f8ec9-56ef-46b8-8977-c431e5733ba4"
            }
          ]
        },
        {
          "id": "0837f41a-62d3-47ec-9a62-0da86c12c88a",
          "name": "list-parts",
          "request": {
            "url": "{{default}}/ObjectName?uploadId=UploadId?encoding-type=%7B%7D&max-parts=%7B%7D&part-number&#8203;-marker=%7B%7D&uploadId=%7B%7D",
            "method": "GET",
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
            "description": "This operation lists the parts that have been uploaded for a specific multipart upload"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4367274-7640-4f7f-90e4-966d1e94200a"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "5b2d1ba4-878a-4eab-8acd-fcb1379d1f68",
          "name": "delete-multiple-objects",
          "request": {
            "url": "{{default}}/?delete",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "Length of the body according to RFC 2616",
                "disabled": false
              },
              {
                "key": "Content-MD5",
                "value": "{}",
                "description": "The base64-encoded 128-bit MD5 digest of the data",
                "disabled": false
              },
              {
                "key": "x-amz-mfa",
                "value": "{}",
                "description": "The value is the concatenation of the authentication devices serial number, a space,tttttttttand the value that is displayed on your authenticationtttttttttdevice",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The Multi-Object Delete operation enables you to delete multiple objects from a bucketusing a single HTTP request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23162bae-2b5d-45e7-8c43-f310529d72be"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "7620a5c7-0ec5-41e4-aa55-3eb92aef0b46",
          "name": "upload-part",
          "request": {
            "url": "{{default}}/ObjectName?partNumber=PartNumber&amp;uploadId=UploadId?AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo; API Reference &raquo; Operations on Objects &raquo; Upload Part - Copy=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The size of the part, in bytes",
                "disabled": false
              },
              {
                "key": "Content-MD5",
                "value": "{}",
                "description": "The base64-encoded 128-bit MD5 digest of the part data",
                "disabled": false
              },
              {
                "key": "Expect",
                "value": "{}",
                "description": "When your application uses 100-continue, it does not send the request body until ittttttttttreceives an acknowledgment",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source",
                "value": "{}",
                "description": "The name of the source bucket and the source object key name separated by a                  slash (/)",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-algorithm",
                "value": "{}",
                "description": "Specifies algorithm to use when decrypting the source object",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-key",
                "value": "{}",
                "description": "Specifies the customer provided base-64 encoded encryption key for Amazon                      S3 to use to decrypt the source object",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-&#8203;server-side&#8203;-encryption&#8203;-customer-key-MD5",
                "value": "{}",
                "description": "Specifies the base64-encoded 128-bit MD5 digest of the encryption key                      according to RFC 1321",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-match",
                "value": "{}",
                "description": "Perform a copy if the source object entity tag (ETag) matches the specified                  value",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-modified-since",
                "value": "{}",
                "description": "Perform a copy if the source object is modified after the time specified                  using this header",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-none-match",
                "value": "{}",
                "description": "Perform a copy if the source object entity tag (ETag) is different than the                  value specified using this header",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-unmodified-since",
                "value": "{}",
                "description": "Perform a copy if the source object is not modified after the time                  specified using this header",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-range",
                "value": "{}",
                "description": "The range of bytes to copy from the source object",
                "disabled": false
              },
              {
                "key": "x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm",
                "value": "{}",
                "description": "Specifies the algorithm to use to when encrypting the object",
                "disabled": false
              },
              {
                "key": "x-amz-server-side&#8203;-encryption&#8203;-customer-key",
                "value": "{}",
                "description": "Specifies the customer-provided base64-encoded encryption key for Amazon S3 to use intttttttttttttencrypting data",
                "disabled": false
              },
              {
                "key": "x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5",
                "value": "{}",
                "description": "Specifies the base64-encoded 128-bit MD5 digest of the encryption key according to RFC 1321",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This operation uploads a part in a multipart upload"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "392a1338-73e9-48fa-aca1-91403891697e"
            }
          ]
        }
      ]
    },
    {
      "name": "Complete",
      "item": [
        {
          "id": "fba9db69-7865-4467-abb4-fef63c368e9b",
          "name": "complete-multipart-upload",
          "request": {
            "url": "{{default}}/ObjectName?uploadId=UploadId",
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
            "description": "This operation completes a multipart upload by assembling previously uploaded parts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c78ee99-6208-4298-820d-892d35aa8141"
            }
          ]
        }
      ]
    },
    {
      "name": "Abort",
      "item": [
        {
          "id": "e01d8577-9fe2-4827-84b8-b56b2d93b3a4",
          "name": "abort-multipart-upload",
          "request": {
            "url": "{{default}}/ObjectName?uploadId=UploadId",
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
            "description": "This operation aborts a multipart upload"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38d2c092-1ca6-439c-92b5-d3e0f037911c"
            }
          ]
        }
      ]
    },
    {
      "name": "Initiate",
      "item": [
        {
          "id": "79212004-6b7f-42f2-8a72-b626c9195