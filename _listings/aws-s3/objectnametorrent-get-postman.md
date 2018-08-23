{
  "info": {
    "name": "AWS S3 GET Object torrent",
    "_postman_id": "52bb66b5-4376-45f0-b4f8-f19fd193c39d",
    "description": "This implementation of the GET operation uses thetorrent subresource to return torrent files from a bucket",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "69a1ae0e-8c0e-4028-ab56-8ec05642bea1",
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
              "id": "dd007bf6-194f-4f81-aa05-91324c942c59"
            }
          ]
        },
        {
          "id": "98097132-8ec5-4dfd-813a-5bd368371ffb",
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
              "id": "434c2e36-15da-4884-819f-79c779ac4c2e"
            }
          ]
        },
        {
          "id": "1b4fba5f-8043-49df-85de-ec55e44e5247",
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
              "id": "11326c75-0fde-427a-851e-cc7ea7c7602c"
            }
          ]
        },
        {
          "id": "36b14c6a-9456-41c6-a5b8-a461cdbabbc8",
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
              "id": "64b1a064-301b-4e46-a6ab-b924a789a6c0"
            }
          ]
        },
        {
          "id": "f7e68a38-f39f-4ff8-907f-2c532a1ed20d",
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
              "id": "fa9fa7d5-cb56-49ac-80f8-49581630bdcf"
            }
          ]
        },
        {
          "id": "6fb46ac2-258d-448f-9f41-96d6457f1cf3",
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
              "id": "c0e4f42f-aee3-4092-be66-3487030dd482"
            }
          ]
        },
        {
          "id": "b26b9185-c5b2-46f7-baf0-ee78c24da2f2",
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
              "id": "39a38482-8e08-4176-88ce-e0c189a75684"
            }
          ]
        },
        {
          "id": "6252e4bf-3f3c-4b6c-8705-fd8b62b074ff",
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
              "id": "d8c84654-8ce8-43aa-9827-ebc46ceb841b"
            }
          ]
        },
        {
          "id": "7c4d17ab-51c2-44f5-bca3-c423a62ecce0",
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
              "id": "bb71680a-ed6f-4f66-a87b-6a6ee89ea860"
            }
          ]
        },
        {
          "id": "e9805f98-a519-40e0-976b-caf78ae71e95",
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
              "id": "4f2facfa-5177-4b23-983b-47ca520090d7"
            }
          ]
        },
        {
          "id": "b016b24e-eb84-430a-a276-89b2f9208a0d",
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
              "id": "39ad736e-d04d-475f-a1b5-b92e0000599a"
            }
          ]
        },
        {
          "id": "3b51e9e6-7450-4961-8aa9-0656c0154969",
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
              "id": "7c0f0dac-c784-4ca3-a381-0e01b90db7d9"
            }
          ]
        },
        {
          "id": "d4f3353e-6678-43f9-990b-edfabcef5056",
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
              "id": "f8ec9bbb-6ee2-4550-be89-7419049d62ae"
            }
          ]
        },
        {
          "id": "34434f7b-3eac-42fb-a4dd-24a14fd536a7",
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
              "id": "8fbeff3c-59ab-49c8-aee2-c5aab9e163c8"
            }
          ]
        },
        {
          "id": "8421a29d-fdcd-49cf-a00c-683e2fa7ea2e",
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
              "id": "c0e8ef27-a8b1-46d2-8828-52e5f4f40426"
            }
          ]
        },
        {
          "id": "b9ebe5b9-f673-44e2-a963-a7b815fd3f8b",
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
              "id": "aa7bb891-2e01-4d19-b104-d8bf47491791"
            }
          ]
        },
        {
          "id": "a15c1f73-e5e8-42bf-8c98-08b2c7af8e40",
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
              "id": "f1104f37-6ec8-4003-9199-2c0129059cc5"
            }
          ]
        },
        {
          "id": "7755d707-9e6b-4b82-b5e6-1908b713b6aa",
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
              "id": "916b7ead-4320-48e9-b94c-fc442aa0579d"
            }
          ]
        },
        {
          "id": "e4164be1-ad4c-4fa8-8114-2ffbe4a333e3",
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
              "id": "4b9fece9-e1ca-4f03-bd67-d5c3cc5b2043"
            }
          ]
        },
        {
          "id": "4be4abe6-3d6a-4119-b6c0-79d3d33c2afd",
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
              "id": "267c8055-798e-4ddf-9c8e-6b33fba2b578"
            }
          ]
        },
        {
          "id": "6f8b5ffb-e1b8-4299-8181-ff93c78b79f9",
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
              "id": "022fc29e-41e3-41a6-a925-f3cceb959032"
            }
          ]
        },
        {
          "id": "7f6f79ff-1197-47c9-9a1f-bd1245a8d8b9",
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
              "id": "a9fd66bd-43f2-4e66-95bd-8697fa2269d0"
            }
          ]
        },
        {
          "id": "71409a95-d4a1-4eff-a3d5-91ceadbcead3",
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
              "id": "f57aea6b-be9b-4cea-bab2-aae43904cd31"
            }
          ]
        },
        {
          "id": "aeb698cd-a3fa-4ba6-accf-220193172720",
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
              "id": "997f1901-cf15-429a-9de5-7ff40f273751"
            }
          ]
        },
        {
          "id": "4051fc79-3c74-4890-8f10-eaa3a3f0ae8f",
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
              "id": "0f8911af-9aa4-4d28-a99b-68bf234c8864"
            }
          ]
        },
        {
          "id": "04d6ced7-6770-4190-adfa-970ab96cff13",
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
              "id": "003e8764-7b70-4bf2-a94d-9f0999b36812"
            }
          ]
        },
        {
          "id": "913382cf-7cd5-4faa-b244-ab23765cbf59",
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
              "id": "756ff0d5-5bee-4080-9947-64c743addc77"
            }
          ]
        },
        {
          "id": "9fd3eda4-6a63-41b9-b99f-81de8a0e6b10",
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
              "id": "1da748ab-7936-4fa7-bc0c-2f65b32eebf0"
            }
          ]
        },
        {
          "id": "53b8d8dc-ba0d-424d-8f0c-5cd39cd0ee16",
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
              "id": "9e247c45-5b9a-400d-997f-b5bd234fffe4"
            }
          ]
        },
        {
          "id": "185fb00c-85a6-4cd5-a26a-a8b68098d740",
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
              "id": "6f73e39d-1f40-46f5-9e78-830ea9830816"
            }
          ]
        },
        {
          "id": "c515eada-5fbd-4533-aa9f-45e7dc5e676f",
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
              "id": "22f8e62e-e562-4f63-8110-e5ecae2b126a"
            }
          ]
        },
        {
          "id": "cd25bd4a-81e0-4561-a2bf-247fa167eeb8",
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
              "id": "04ff8041-2e39-4567-a5c6-0440d79e41f5"
            }
          ]
        },
        {
          "id": "2bed0f1d-b87f-4e13-959c-46de471a3e86",
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
              "id": "41d24279-2abc-456d-93ec-d03c9218bdff"
            }
          ]
        },
        {
          "id": "7c262eb8-8d7a-428c-8837-b8612648f63b",
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
              "id": "3972ec20-bb7e-4aaa-b199-38b19c5e2186"
            }
          ]
        },
        {
          "id": "8a1f41ca-1709-4aec-9184-1919ee18e9fb",
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
              "id": "c5bb1262-58ff-40ac-9b31-68cae24c3b36"
            }
          ]
        },
        {
          "id": "ac36da32-ccb0-44c9-b8ed-e4c7e1bb56f2",
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
              "id": "d2346086-05cc-4ac1-9e7f-3b6b8f36a270"
            }
          ]
        },
        {
          "id": "e6f7b0ba-ca7d-4572-8c77-4218bdebe9aa",
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
              "id": "5be4412e-3250-4885-9672-23ab33ed32d3"
            }
          ]
        },
        {
          "id": "e71131fd-dea6-4ec6-aa0d-4a529f7ede0d",
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
              "id": "eccd77b5-b1fc-40c3-ac97-7f10ae8c21f7"
            }
          ]
        },
        {
          "id": "cbe8d459-a38c-473e-84b8-502f5f7c7e4d",
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
              "id": "9f8dd782-3524-4762-af1b-396f533e2acd"
            }
          ]
        },
        {
          "id": "f490562a-1c7f-48d7-b3e5-b15bba913978",
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
              "id": "4433bd5d-e232-48c8-89aa-3864e1a2e2b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "03a42995-908d-4075-878f-0dc96083b7e4",
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
              "id": "95a3a569-4060-4d51-958d-ad3bacba8e88"
            }
          ]
        },
        {
          "id": "012a6646-850f-4f95-bc4c-310b5fb68d8e",
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
              "id": "2c09b922-f26e-4f15-b2be-5dafe39edfc0"
            }
          ]
        },
        {
          "id": "a9691b34-fb3f-4cd5-977d-1ed28b4be172",
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
              "id": "12865318-38c5-4355-8a71-a60fa221ac72"
            }
          ]
        },
        {
          "id": "3319067f-69f7-41c4-ad48-136ac50dd8d8",
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
              "id": "d992f76d-5095-48dc-bf5f-03235c6b1135"
            }
          ]
        },
        {
          "id": "1e4f7e26-531e-4409-9b5c-9e58727a2a7a",
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
              "id": "b5371e30-1dd4-45ce-8df9-2c1eb0fa2193"
            }
          ]
        },
        {
          "id": "0557f3bc-c573-4600-aa81-b66bcb1ac657",
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
              "id": "9986e661-6582-4b12-b5d6-b837c2f0f96f"
            }
          ]
        },
        {
          "id": "d9dbc152-87c7-4edc-9fa1-f77a87e8c526",
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
              "id": "b99ffbb4-4a14-4dfd-ab3f-9b4f594be101"
            }
          ]
        },
        {
          "id": "fbb3a5cc-3458-4122-b1f5-be14a156f3c8",
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
              "id": "2b946a76-b8da-4034-ae24-ab6fccb71d1a"
            }
          ]
        },
        {
          "id": "95a7d931-33a3-48b3-8fc4-dd22c1a79712",
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
              "id": "005f330c-44bd-45cc-832d-a4c3ca1a15ad"
            }
          ]
        },
        {
          "id": "08cb1962-1cb0-4e4e-b4f6-4148610364d1",
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
              "id": "96fea951-a816-47fe-becf-c18d2e775093"
            }
          ]
        },
        {
          "id": "53030557-6014-42a9-8755-931b4741fc6d",
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
              "id": "c5d27888-fa04-4898-bf92-672bf8a216c9"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "5e7094b6-8f5b-4b01-9515-28d1d4f8aed0",
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
              "id": "7ce6cab6-4d31-4f35-be4a-2d6e557aa0f9"
            }
          ]
        },
        {
          "id": "46256962-9a09-4ba8-9ff9-e5d7223a03a2",
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
              "id": "d231dca7-0279-4b15-a933-be695bb7de95"
            }
          ]
        },
        {
          "id": "f60e7bdb-1092-45fc-ae94-597cfa776caf",
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
              "id": "f8a9a5ea-ac96-4eab-9e4d-e1417cce2135"
            }
          ]
        },
        {
          "id": "0ef0444f-3d5e-4460-8b67-9fd895f2551d",
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
              "id": "561042e3-c06e-4607-96c8-d511d73c3a94"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "f8e935dd-0b9c-453c-a946-0707c62f699f",
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
              "id": "f6784400-95de-4681-ab4b-2f7175806890"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "0d43791c-21d6-4bb6-8d90-6ca39012aed0",
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
              "id": "2601ce10-f043-47e4-847b-93e889f9e59c"
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