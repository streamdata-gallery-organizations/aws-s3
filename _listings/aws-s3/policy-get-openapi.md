---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 GET Bucket policy
  version: 1.0.0
  description: This implementation of the GET operation uses the policysubresource
    to return the policy of a specified bucket
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    delete:
      summary: DELETE Bucket
      description: This implementation of the DELETE operation deletes the bucket
        named inthe URI
      operationId: delete-bucket
      x-api-path-slug: delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
    head:
      summary: HEAD Bucket
      description: This operation is useful to determine if a bucket exists and you
        have permission to accessit
      operationId: head-bucket
      x-api-path-slug: head
      responses:
        200:
          description: OK
      tags:
      - Bucket
    post:
      summary: POST Object
      description: The POST operation adds an object to a specified bucket using HTML
        forms
      operationId: post-object
      x-api-path-slug: post
      responses:
        200:
          description: OK
      tags:
      - Object
    put:
      summary: PUT Bucket
      description: This implementation of the PUT operation creates a new bucket
      operationId: put-bucket
      x-api-path-slug: put
      parameters:
      - in: header
        name: x-amz-acl
        description: The canned ACL to apply to the bucket you are creating
      - in: header
        name: x-amz-grant-full-control
        description: Allows grantee the READ, WRITE, READ_ACP, and WRITE_ACP permissions
          on thettttttttttttbucket
      - in: header
        name: x-amz-grant-read
        description: Allows grantee to list the objects in the bucket
      - in: header
        name: x-amz-grant-read-acp
        description: Allows grantee to read the bucket ACL
      - in: header
        name: x-amz-grant-write
        description: Allows grantee to create, overwrite, and delete any object in
          the bucket
      - in: header
        name: x-amz-grant-write-acp
        description: Allows grantee to write the ACL for the applicable bucket
      responses:
        200:
          description: OK
      tags:
      - Bucket
  /?accelerate:
    get:
      summary: GET Bucket accelerate
      description: This implementation of the GET operation uses the acceleratesubresource
        to return the Transfer Acceleration state of a bucket, which is eitherEnabled
        or Suspended
      operationId: get-bucket-accelerate
      x-api-path-slug: accelerate-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Accelerate
    put:
      summary: PUT Bucket accelerate
      description: This implementation of the PUT operation uses the acceleratesubresource
        to set the Transfer Acceleration state of an existing bucket
      operationId: put-bucket-accelerate
      x-api-path-slug: accelerate-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Accelerate
  /?acl:
    get:
      summary: GET Bucket ACL
      description: This implementation of the GET operation uses the aclsubresource
        to return the access control list (ACL) of a bucket
      operationId: get-bucket-acl
      x-api-path-slug: acl-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - ACL
    put:
      summary: PUT Bucket ACL
      description: This implementation of the PUT operation uses the aclsubresource
        to set the permissions on an existing bucket using access control lists(ACL)
      operationId: put-bucket-acl
      x-api-path-slug: acl-put
      parameters:
      - in: header
        name: x-amz-acl
        description: Sets the ACL of the bucket using the specified canned ACL
      - in: header
        name: x-amz-grant-full-control
        description: Allows the specified grantee(s) the READ, WRITE, READ_ACP, and
          WRITE_ACPtttttttttpermissions on the bucket
      - in: header
        name: x-amz-grant-read
        description: Allows the specified grantee(s) to list the objects in the bucket
      - in: header
        name: x-amz-grant-read-acp
        description: Allows the specified grantee(s) to read the bucket ACL
      - in: header
        name: x-amz-grant-write
        description: Allows the specified grantee(s) to create, overwrite, and delete
          any object in thetttttttttbucket
      - in: header
        name: x-amz-grant-write-acp
        description: Allows the specified grantee(s) to write the ACL for the applicabletttttttttbucket
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - ACL
  /?analytics:
    get:
      summary: List Bucket Analytics Configurations
      description: This implementation of the GET operation returns a list of analyticsconfigurations
        for the bucket
      operationId: list-bucket-analytics-configurations
      x-api-path-slug: analytics-get
      parameters:
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue an analytics configuration
          listing that has beenttttttttttruncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Analytics
      - Configurations
  /?analytics&amp;id=analytics-configuration-ID:
    delete:
      summary: DELETE Bucket analyticsnttconfiguration
      description: This implementation of the DELETE operation deletes an analytics
        configuration(identified by the analytics configuration ID) from the bucket
      operationId: delete-bucket-analyticsconfiguration
      x-api-path-slug: analyticsampidanalyticsconfigurationid-delete
      parameters:
      - in: query
        name: id
        description: The ID that identifies the analytics configuration
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Analyticsnttconfiguration
    get:
      summary: GET Bucket analytics configuration
      description: This implementation of the GET operation returns an analytics configuration
        (identified bythe analytics configuration ID) from the bucket
      operationId: get-bucket-analytics-configuration
      x-api-path-slug: analyticsampidanalyticsconfigurationid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Analytics
      - Configuration
  /?analytics&amp;id=configuration-ID:
    put:
      summary: PUT Bucket analytics configuration
      description: This implementation of the PUT operation adds an analytics configuration(identified
        by the analytics ID) to the bucket
      operationId: put-bucket-analytics-configuration
      x-api-path-slug: analyticsampidconfigurationid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Analytics
      - Configuration
  /?cors:
    delete:
      summary: DELETE Bucket CORS
      description: Deletes the cors configuration information set for the bucket
      operationId: delete-bucket-cors
      x-api-path-slug: cors-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - CORS
    get:
      summary: GET Bucket CORS
      description: Returns the cors configuration information set for thebucket
      operationId: get-bucket-cors
      x-api-path-slug: cors-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - CORS
  /?delete:
    post:
      summary: Delete Multiple Objects
      description: The Multi-Object Delete operation enables you to delete multiple
        objects from a bucketusing a single HTTP request
      operationId: delete-multiple-objects
      x-api-path-slug: delete-post
      parameters:
      - in: header
        name: Content-Length
        description: Length of the body according to RFC 2616
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the data
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authentication devices
          serial number, a space,tttttttttand the value that is displayed on your
          authenticationtttttttttdevice
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Objects
  /?inventory:
    get:
      summary: List Bucket Inventory Configurations
      description: This implementation of the GET operation returns a list of inventoryconfigurations
        for the bucket
      operationId: list-bucket-inventory-configurations
      x-api-path-slug: inventory-get
      parameters:
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue an inventory configuration
          listing that has beenttttttttttruncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Inventory
      - Configurations
  /?inventory&amp;id=configuration-ID:
    put:
      summary: PUT Bucket inventory configuration
      description: This implementation of the PUT operation adds an inventory configuration(identified
        by the inventory ID) to the bucket
      operationId: put-bucket-inventory-configuration
      x-api-path-slug: inventoryampidconfigurationid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
  /?inventory&amp;id=inventory-configuration-ID:
    delete:
      summary: DELETE Bucket inventory configuration
      description: This implementation of the DELETE operation deletes an inventory
        configuration(identified by the inventory configuration ID) from the bucket
      operationId: delete-bucket-inventoryconfiguration
      x-api-path-slug: inventoryampidinventoryconfigurationid-delete
      parameters:
      - in: query
        name: id
        description: The ID that identifies the inventory configuration
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
    get:
      summary: GET Bucket inventory configuration
      description: This implementation of the GET operation returns an inventory configuration
        (identified bythe inventory configuration ID) from the bucket
      operationId: get-bucket-inventory-configuration
      x-api-path-slug: inventoryampidinventoryconfigurationid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
  /?lifecycle:
    delete:
      summary: DELETE Bucket lifecycle
      description: Deletes the lifecycle configuration from the specified bucket
      operationId: delete-bucket-lifecycle
      x-api-path-slug: lifecycle-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Lifecycle
    get:
      summary: GET Bucket lifecycle
      description: NoteBucket lifecycle configuration now supports specifying lifecycle
        rule usingobject key name prefix, one or more object tags, or combination
        of both
      operationId: get-bucket-lifecycle
      x-api-path-slug: lifecycle-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Lifecycle
    put:
      summary: PUT Bucket lifecycle
      description: Creates a new lifecycle configuration for the bucket or replaces
        an existing lifecycle configuration
      operationId: put-bucket-lifecycle
      x-api-path-slug: lifecycle-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Lifecycle
  /?list-type=2:
    get:
      summary: GET Bucket (List Objects) Version 2
      description: This implementation of the GET operation returns some or all (up
        to 1,000) ofthe objects in a bucket
      operationId: get-bucket-list-objects-version-2
      x-api-path-slug: listtype2-get
      parameters:
      - in: query
        name: continuation-token
        description: When the Amazon S3 response to this API call is truncated (that
          is, IsTruncated responsetttttttttelement value is true), the response also
          includes thettttttttttNextContinuationToken element, the value of whichtttttttttyou
          can use in the next request as thettttttttttcontinuation-token to list the
          next settttttttttof objects
      - in: query
        name: delimiter
        description: A delimiter is a character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: fetch-owner
        description: By default, the API does not return the Owner information in
          the response
      - in: query
        name: list-type
        description: Version 2 of the API requires this parameter and you must set
          its value to 2
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Limits the response to keys that begin with the specifiedtttttttttprefix
      - in: query
        name: start-after
        description: If you want the API to return key names after a specifictttttttttobject
          key in your key space, you can add this parameter
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - (List
      - Objects)
      - Version
      - "2"
  /?location:
    get:
      summary: GET Bucket location
      description: This implementation of the GET operation uses thelocation subresource
        to return a bucket's region
      operationId: get-bucket-location
      x-api-path-slug: location-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Location
  /?logging:
    get:
      summary: GET Bucket logging
      description: This implementation of the GET operation uses thelogging subresource
        to return the logging status of a bucketand the permissions users have to
        view and modify that status
      operationId: get-bucket-logging
      x-api-path-slug: logging-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Logging
  /?metrics:
    get:
      summary: List Bucket Metrics
      description: Lists the metrics configurations for the CloudWatch request metrics
        of the bucket
      operationId: list-bucket-metrics
      x-api-path-slug: metrics-get
      parameters:
      - in: query
        name: BucketName
        description: The name of the bucket containing the metrics configurationstttttttttto
          retrieve
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue a metrics configurationtttttttttlisting
          that has been truncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Metrics
  /?metrics&amp;id=Id:
    delete:
      summary: DELETE Bucket Metrics
      description: Deletes a metrics configuration for the CloudWatch request metrics
        (specified by the metricsconfiguration ID) from the bucket
      operationId: delete-bucket-metrics
      x-api-path-slug: metricsampidid-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
    put:
      summary: PUT Bucket Metrics
      description: Sets or updates a metrics configuration for the CloudWatch request
        metrics (specified by themetrics configuration ID) from the bucket
      operationId: put-bucket-metrics
      x-api-path-slug: metricsampidid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
  /?metrics&amp;id=id:
    get:
      summary: GET Bucket Metrics
      description: Gets a metrics configuration for the CloudWatch request metrics
        (specified by the metricsconfiguration ID) from the bucket
      operationId: get-bucket-metrics
      x-api-path-slug: metricsampidid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
  /?notification:
    get:
      summary: GET Bucket notification
      description: This implementation of the GET operation uses thenotification subresource
        to return the notificationconfiguration of a bucket
      operationId: get-bucket-notification
      x-api-path-slug: notification-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Notification
    put:
      summary: PUT Bucket notification
      description: The Amazon S3 notification feature enables you to receive notifications
        when certain eventshappen in your bucket
      operationId: put-bucket-notification
      x-api-path-slug: notification-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Notification
  /?policy:
    delete:
      summary: DELETE Bucket policy
      description: This implementation of the DELETE operation uses the policy subresource
        to delete the policy on a specified bucket
      operationId: delete-bucket-policy
      x-api-path-slug: policy-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Policy
    get:
      summary: GET Bucket policy
      description: This implementation of the GET operation uses the policysubresource
        to return the policy of a specified bucket
      operationId: get-bucket-policy
      x-api-path-slug: policy-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Policy
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---