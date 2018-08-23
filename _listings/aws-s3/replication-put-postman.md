{
  "info": {
    "name": "AWS S3 PUT Bucket replication",
    "_postman_id": "df5243d0-b829-494f-9c2a-dc4705ea2e56",
    "description": "In a versioning-enabled bucket, this operation creates a new replication configuration (or      replaces an existing one, if present)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "a5ec9672-641a-492b-964d-a3ec4c433c13",
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
              "id": "559e15b2-6afd-4bbd-9167-0437f8e2ee9b"
            }
          ]
        },
        {
          "id": "fbe584bd-2c16-4648-a0dd-de8a4c004f07",
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
              "id": "b502b1cc-bac9-48e9-bca4-9fb53b8d625e"
            }
          ]
        },
        {
          "id": "18dc7cd8-8e20-4898-9ba0-6e5adf9340e3",
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
              "id": "e4808377-13b9-468a-997a-6c2928a7a28d"
            }
          ]
        },
        {
          "id": "782db552-20dc-4e49-a6ec-5b5b42259e89",
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
              "id": "3231a428-a7d2-43f4-9ac2-c678f7c65cd3"
            }
          ]
        },
        {
          "id": "bc64dd85-9ac1-4e65-90f0-9b5263b29373",
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
              "id": "bed436ff-f131-409b-930f-32f9b38dd6a8"
            }
          ]
        },
        {
          "id": "bb53eb3f-c830-4479-b629-f30316a804a4",
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
              "id": "4e055cf0-1fc1-46f2-8f5f-9ccbebacb843"
            }
          ]
        },
        {
          "id": "5f2bf189-7486-4db1-8d3c-900311edddf9",
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
              "id": "bf20c98b-d7ae-49ce-a53e-858da966ba4d"
            }
          ]
        },
        {
          "id": "33eccdb4-8f29-475d-aba4-57042eaa4bd1",
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
              "id": "56a358be-db5e-4cc9-baa4-016cddeb181f"
            }
          ]
        },
        {
          "id": "edd82dbf-9eb6-402c-88fc-812275b260f5",
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
              "id": "d2c28b22-0218-48cf-ab6a-cd0bf952f906"
            }
          ]
        },
        {
          "id": "80bd32ca-98b1-4e4e-9da1-a0a93febba7f",
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
              "id": "7589476b-592d-4600-ad7f-06c6cb0465d5"
            }
          ]
        },
        {
          "id": "9c769c2b-068d-4045-b1fb-57db188f8b3b",
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
              "id": "71c8576e-4ad0-4a61-a57b-08291af8efb0"
            }
          ]
        },
        {
          "id": "14d133f8-3e6f-4d73-92e3-1991c4e539d5",
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
              "id": "40a039e9-1ed6-4933-9afc-1001f4a95519"
            }
          ]
        },
        {
          "id": "1dafb73d-417a-4231-b79e-770590de4cb4",
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
              "id": "7a544a2d-c9dd-41b8-b97b-15836caf7d13"
            }
          ]
        },
        {
          "id": "d319298e-de60-42f3-af1a-aa12968664fa",
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
              "id": "9e032a0c-512f-4fee-8910-94aea4bdc99b"
            }
          ]
        },
        {
          "id": "3bfed777-ecc1-41e5-814b-6722482d60be",
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
              "id": "0e94387f-8b2a-491a-84ad-763e11ec4883"
            }
          ]
        },
        {
          "id": "78b9df57-13e3-4381-a621-995e57f71ca0",
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
              "id": "353bca3b-4f45-43bd-87ea-89068ec0fb9b"
            }
          ]
        },
        {
          "id": "d553f971-b274-47e8-a443-de2af7c03740",
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
              "id": "e0216a8b-568a-4c6d-ae13-3684eb3d4074"
            }
          ]
        },
        {
          "id": "f8e76665-412f-4772-b4bb-8d9655911591",
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
              "id": "aa08ccdc-2ec9-4701-9e99-db90a939645f"
            }
          ]
        },
        {
          "id": "3808c943-0264-45c9-bfe0-a99c6d5a4d55",
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
              "id": "563db4e8-f5e0-4083-8119-67abc9affd91"
            }
          ]
        },
        {
          "id": "bf655669-05a6-4eff-aa99-044a6dfcc8d4",
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
              "id": "3d187ab5-72a0-4c05-8c2d-aa9f6afc25c8"
            }
          ]
        },
        {
          "id": "3d261a5f-6138-45c1-9633-e07c0728b6f5",
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
              "id": "ef5d8033-44ef-4148-97aa-b9ea9c806d45"
            }
          ]
        },
        {
          "id": "91320345-e12b-4735-a7f6-f900ca380792",
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
              "id": "9f2534eb-e24b-4488-8fc5-48ea2d37a9e1"
            }
          ]
        },
        {
          "id": "8435f3a1-849d-4fd3-bc99-c119b49a2b8c",
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
              "id": "27fa5f3a-c600-4f7b-a298-b39d3fe74a44"
            }
          ]
        },
        {
          "id": "10509fba-e211-4876-a0c7-111f9a54fcfa",
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
              "id": "3d1f6f26-728f-433f-a519-14a451e5bc6e"
            }
          ]
        },
        {
          "id": "a04a5cc9-e173-4930-93e3-54376557ab6e",
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
              "id": "d62879a1-fb73-4edc-90ae-d10d270ae4aa"
            }
          ]
        },
        {
          "id": "50922d84-b461-4e8a-85cb-9bd50f0e1bdb",
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
              "id": "63b32607-ea6d-410b-be44-806ff4dcdfec"
            }
          ]
        },
        {
          "id": "471c784a-0d15-449d-81e7-88316bcdfaa1",
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
              "id": "3b2847be-bb07-4a25-9747-eb11eb705fb2"
            }
          ]
        },
        {
          "id": "57ac62fa-1d71-43ac-9cf6-b7d70df75a41",
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
              "id": "55d2ef59-3f98-4cb0-a2b4-9e51f9a994b2"
            }
          ]
        },
        {
          "id": "b629b6af-0134-4389-bdce-41a2fef4ca61",
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
              "id": "b1546cf8-0d7c-49f2-b46b-602e00c2c563"
            }
          ]
        },
        {
          "id": "c0b87477-465a-4eeb-a2f7-ac208ed65e65",
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
              "id": "25430c8c-f301-47e8-925a-7e11687c6b6a"
            }
          ]
        },
        {
          "id": "d4938272-71c2-4bfb-9ef3-28091caab9c0",
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
              "id": "a00b6e4e-42a8-4265-93c0-b956551c6e82"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "58134c87-1585-464c-adc8-678d6a8c8643",
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
              "id": "86e33b8f-b670-4c80-a715-97dabd606649"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "a41a94bc-ac67-421e-9acb-ba639aef7f9f",
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
              "id": "310db8f6-75e8-4343-ae81-5a9bcf5dbb1d"
            }
          ]
        },
        {
          "id": "67fc23a5-5449-4bae-b87a-405d504b33fe",
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
              "id": "57177ecb-6ecd-4ee2-86cd-01c97fecda59"
            }
          ]
        },
        {
          "id": "fb9340ee-6f1e-4543-900b-a8906eceb21f",
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
              "id": "1ecd05b1-717b-41ea-b177-647a03aaaf8b"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "1a933c02-306f-4453-822c-c375ec2bb9ba",
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
              "id": "04a0e105-02e4-47b2-b79a-0404f464b563"
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