---
swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 1
info:
  title: AWS Machine Learning API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDataSourceFromRDS:
    get:
      summary: Create Data Source From R D S
      description: Creates a DataSource object from an.
      operationId: createDataSourceFromRDS
      x-api-path-slug: actioncreatedatasourcefromrds-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: RDSData
        description: 'The data specification of an Amazon RDS DataSource:'
        type: string
      - in: query
        name: RoleARN
        description: The role that Amazon ML assumes on behalf of the user to create
          and activate a data          pipeline in the users account and copy data
          using the SelectSqlQuery query from Amazon RDS to Amazon S3
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=CreateDataSourceFromRedshift:
    get:
      summary: Create Data Source From Redshift
      description: Creates a DataSource from a database hosted on an Amazon Redshift
        cluster.
      operationId: createDataSourceFromRedshift
      x-api-path-slug: actioncreatedatasourcefromredshift-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: DataSpec
        description: 'The data specification of an Amazon Redshift DataSource:'
        type: string
      - in: query
        name: RoleARN
        description: A fully specified role Amazon Resource Name (ARN)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=CreateDataSourceFromS3:
    get:
      summary: Create Data Source From S3
      description: Creates a DataSource object.
      operationId: createDataSourceFromS3
      x-api-path-slug: actioncreatedatasourcefroms3-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied identifier that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: DataSpec
        description: 'The data specification of a DataSource:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
---