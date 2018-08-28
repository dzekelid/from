{
  "info": {
    "name": "Amazon RDS API Remove Source Identifier From Subscription",
    "_postman_id": "07da835b-f67b-4d8d-87b4-00ae9d246e0a",
    "description": "Removes a source identifier from an existing RDS event notification subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "d16b6d42-da16-48bc-ac86-576a1367f53d",
          "name": "addroletodbcluster",
          "request": {
            "url": "http://example.com/api/?Action=AddRoleToDBCluster?DBClusterIdentifier=DBClusterIdentifier&RoleArn=RoleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates an Identity and Access Management (IAM) role from an Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fecd3519-b6b1-4efd-ace8-ad7f79be9f64"
            }
          ]
        },
        {
          "id": "6b634720-53ad-4140-b754-dfbc8a999c08",
          "name": "createdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBCluster?AvailabilityZones.AvailabilityZone.N=AvailabilityZones.AvailabilityZone.N&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&DatabaseName=DatabaseName&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&DBSubnetGroupName=DBSubnetGroupName&Engine=Engine&EngineVersion=EngineVersion&KmsKeyId=KmsKeyId&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&ReplicationSourceIdentifier=ReplicationSourceIdentifier&StorageEncrypted=StorageEncrypted&Tags.Tag.N=Tags.Tag.N&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43de2cf4-0c79-460a-bc4e-ac5b9cec38ff"
            }
          ]
        },
        {
          "id": "2065e5c4-1eec-4d14-a349-e9df1d8e8a58",
          "name": "deletedbcluster",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBCluster?DBClusterIdentifier=DBClusterIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBCluster action deletes a previously provisioned DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f36c7cc-18f2-4486-94fb-246d89604675"
            }
          ]
        },
        {
          "id": "01f49d13-996f-4b39-8f3a-f89b3a8c8e90",
          "name": "describedbclusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusters?DBClusterIdentifier=DBClusterIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned Aurora DB clusters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c016f9b-ab6a-4b2e-b09c-ed5f6812939a"
            }
          ]
        },
        {
          "id": "2d32e991-5b1f-466d-a44d-8afac6a8227d",
          "name": "failoverdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=FailoverDBCluster?DBClusterIdentifier=DBClusterIdentifier&TargetDBInstanceIdentifier=TargetDBInstanceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forces a failover for a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "102fd2a2-3b2b-4e33-8a3a-ec8bb00f62f9"
            }
          ]
        },
        {
          "id": "f989dadc-f01e-4f9f-b98e-1b699baac949",
          "name": "modifydbcluster",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBCluster?ApplyImmediately=ApplyImmediately&BackupRetentionPeriod=BackupRetentionPeriod&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&MasterUserPassword=MasterUserPassword&NewDBClusterIdentifier=NewDBClusterIdentifier&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a setting for an Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01a6d4c8-a676-4685-b24b-6d793beec917"
            }
          ]
        },
        {
          "id": "7cba1e02-198f-47d3-9b4c-b60e7d94e8c8",
          "name": "removerolefromdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=RemoveRoleFromDBCluster?DBClusterIdentifier=DBClusterIdentifier&RoleArn=RoleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates an Identity and Access Management (IAM) role from an Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b53fb2e-cafb-4dee-909d-98b0d7ac3ba2"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "9fff663c-e7a9-4746-bd0c-6da2699efec1",
          "name": "addsourceidentifiertosubscription",
          "request": {
            "url": "http://example.com/api/?Action=AddSourceIdentifierToSubscription?SourceIdentifier=SourceIdentifier&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a source identifier to an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f8622a2-e867-416d-b168-5f04ceaa7aea"
            }
          ]
        },
        {
          "id": "ec18c562-8d6a-4641-bd19-293fcc3bd762",
          "name": "removesourceidentifierfromsubscription",
          "request": {
            "url": "http://example.com/api/?Action=RemoveSourceIdentifierFromSubscription?SourceIdentifier=SourceIdentifier&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a source identifier from an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7968c235-cf7d-4744-adea-c1d781b894ee"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "66d9ed3c-6cfb-4eb7-a81f-a5ea95b80fd7",
          "name": "addtagstoresource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceName=ResourceName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds metadata tags to an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bd36e60-6676-4857-8191-9611cb0eebc3"
            }
          ]
        },
        {
          "id": "ae40650a-6252-4817-b6c6-8cd89b0dd35c",
          "name": "listtagsforresource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Filters.Filter.N=Filters.Filter.N&ResourceName=ResourceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags on an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb4814a7-ac74-4d38-8cc3-712bb37ded04"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "9c5285c5-038b-4916-a0ef-aff582a72558",
          "name": "applypendingmaintenanceaction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyPendingMaintenanceAction?ApplyAction=ApplyAction&OptInType=OptInType&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a pending maintenance action to a resource (for example, to a DB instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "760c2892-0e69-4f0e-84f1-4059b1aa92ac"
            }
          ]
        },
        {
          "id": "7c0f7342-5fb0-4af8-aae7-049716233226",
          "name": "describependingmaintenanceactions",
          "request": {
            "url": "http://example.com/api/?Action=DescribePendingMaintenanceActions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of resources (for example, DB instances) that have at least one pending maintenance action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c8d15cc-6fd8-4a1d-af88-88fbf840c28f"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "2bdd871f-7141-48e0-998b-12e5b40ba530",
          "name": "authorizedbsecuritygroupingress",
          "request": {
            "url": "http://example.com/api/?Action=AuthorizeDBSecurityGroupIngress?CIDRIP=CIDRIP&DBSecurityGroupName=DBSecurityGroupName&EC2SecurityGroupId=EC2SecurityGroupId&EC2SecurityGroupName=EC2SecurityGroupName&EC2SecurityGroupOwnerId=EC2SecurityGroupOwnerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables ingress to a DBSecurityGroup using one of two forms of authorization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "636a95e7-cc53-4f6d-8154-87b9008caf9d"
            }
          ]
        },
        {
          "id": "7587dd35-90dc-4259-b7f9-5b89f750fd5a",
          "name": "createdbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSecurityGroup?DBSecurityGroupDescription=DBSecurityGroupDescription&DBSecurityGroupName=DBSecurityGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c897bf00-f5de-4491-865b-03df1c88e28b"
            }
          ]
        },
        {
          "id": "48a27a83-00ab-4b02-a2a0-5a338ec450d8",
          "name": "deletedbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSecurityGroup?DBSecurityGroupName=DBSecurityGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae722fe2-5788-4a2b-9b9d-6ac0bf0ef0fa"
            }
          ]
        },
        {
          "id": "20ef6854-c8e0-4acf-8857-2bbd1104e9d0",
          "name": "describedbsecuritygroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSecurityGroups?DBSecurityGroupName=DBSecurityGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSecurityGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27feed59-e0a0-4d9e-85fa-c48d93366c90"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "31dda300-939a-43bd-8602-dcb1b1276cb7",
          "name": "copydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterParameterGroup?SourceDBClusterParameterGroupIdentifier=SourceDBClusterParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterParameterGroupDescription=TargetDBClusterParameterGroupDescription&TargetDBClusterParameterGroupIdentifier=TargetDBClusterParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03a3cd9a-222d-46b7-a58b-e06d0dbebad9"
            }
          ]
        },
        {
          "id": "2c748457-8c3a-4b8d-94b3-b5bf8768bd8b",
          "name": "createdbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&DBParameterGroupFamily=DBParameterGroupFamily&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7629d8f7-c12b-4cff-8e93-132958fceb6f"
            }
          ]
        },
        {
          "id": "807a358b-a91e-446e-b8a0-66f733b11115",
          "name": "deletedbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7967ab0d-1de3-4f15-afd7-7976eabd8764"
            }
          ]
        },
        {
          "id": "5a689f62-aaca-4ab0-a17c-92b22ddd3f4b",
          "name": "describedbclusterparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameterGroups?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBClusterParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae4b340d-0383-41e4-88ff-63dc278336f2"
            }
          ]
        },
        {
          "id": "45f425f1-87cc-4d16-b7c9-17483b23211a",
          "name": "modifydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2952ea05-b1a0-4db6-827d-3b5fe9b75a1e"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Snapshots",
      "item": [
        {
          "id": "d4b70f35-a2c3-48a3-a584-289e7b021029",
          "name": "copydbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterSnapshot?SourceDBClusterSnapshotIdentifier=SourceDBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterSnapshotIdentifier=TargetDBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cba23038-55cf-4c31-a35c-3b5483c6e932"
            }
          ]
        },
        {
          "id": "eaab3dc0-7733-42ef-9acc-0f2cfacc6bfc",
          "name": "createdbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterSnapshot?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b2cbbed-2220-4320-bdeb-0ad72aa10348"
            }
          ]
        },
        {
          "id": "a7400f8f-4504-4967-8b35-ae896886509a",
          "name": "deletedbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterSnapshot?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05540000-f9fc-45ad-ab24-c10173589d77"
            }
          ]
        },
        {
          "id": "26ced8e3-d526-46c1-a203-8e6667df35c6",
          "name": "describedbclustersnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshotAttributes?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB cluster snapshot attribute names and values for a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d56e8cf-bf64-4a70-968d-afd5f4a449aa"
            }
          ]
        },
        {
          "id": "a7910573-c44d-4a19-8947-0e3a3da1a4aa",
          "name": "describedbclustersnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshots?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB cluster snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "096793c8-ce03-47fe-822e-d405e84cd151"
            }
          ]
        },
        {
          "id": "02b01587-ddd7-4a73-abb8-809da56a1192",
          "name": "modifydbclustersnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterSnapshotAttribute?AttributeName=AttributeName&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b8277e2-b0be-4e74-974d-8fc9eebbcff0"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter Groups",
      "item": [
        {
          "id": "3fca0401-9177-4cc8-b9f5-c5a97235ad22",
          "name": "copydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBParameterGroup?SourceDBParameterGroupIdentifier=SourceDBParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBParameterGroupDescription=TargetDBParameterGroupDescription&TargetDBParameterGroupIdentifier=TargetDBParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "268a9671-b244-4397-bd0e-5303376b27b3"
            }
          ]
        },
        {
          "id": "bef30fc7-810e-4246-809c-4c4a33605303",
          "name": "createdbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBParameterGroup?DBParameterGroupFamily=DBParameterGroupFamily&DBParameterGroupName=DBParameterGroupName&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efac49c0-b12a-42be-ae28-6ec616c30c11"
            }
          ]
        },
        {
          "id": "d62eda0e-2235-4a1e-ac34-1c5529e334b7",
          "name": "deletedbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBParameterGroup?DBParameterGroupName=DBParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DBParameterGroup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9be0a35f-e3f5-4aa1-b95c-0657e9a7c0dd"
            }
          ]
        },
        {
          "id": "9f7de6b2-c496-4cc4-b5bd-8fee173effd7",
          "name": "describedbparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameterGroups?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ce7f001-3305-4d18-bf42-c72473dc12f7"
            }
          ]
        },
        {
          "id": "e33df019-3a20-45b8-9ad6-5019969e8e1d",
          "name": "modifydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBParameterGroup?DBParameterGroupName=DBParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48bc7a89-017d-4b68-a776-31a771648ed2"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "0f6c43a7-6645-423d-bace-345e6ec6dcaa",
          "name": "copydbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBSnapshot?CopyTags=CopyTags&KmsKeyId=KmsKeyId&PreSignedUrl=PreSignedUrl&SourceDBSnapshotIdentifier=SourceDBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBSnapshotIdentifier=TargetDBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64b8b2a6-fabb-4130-86eb-b867870af764"
            }
          ]
        },
        {
          "id": "9c22944c-c814-4624-83b2-70888734fd29",
          "name": "createdbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSnapshot?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f8018b8-1c65-46d9-ab74-16e111fb4787"
            }
          ]
        },
        {
          "id": "40c467ef-0187-4052-8895-a5e2db30a673",
          "name": "deletedbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSnapshot?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f728d07f-d6cb-4aea-8ed9-6c099407ba9d"
            }
          ]
        },
        {
          "id": "1aa8fb6d-4d7b-40ba-80c6-38363dc753d3",
          "name": "describedbsnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshotAttributes?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB snapshot attribute names and values for a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb8d3f12-7c4b-4a90-91dd-359cf4105974"
            }
          ]
        },
        {
          "id": "a9dc4f3d-b19d-4c8c-b09f-a80a79b9733e",
          "name": "describedbsnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshots?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73ab12ab-4adf-42b8-a206-73443afa8bcb"
            }
          ]
        },
        {
          "id": "10b9269d-c36c-477b-b502-c3c5a43f6478",
          "name": "modifydbsnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSnapshotAttribute?AttributeName=AttributeName&DBSnapshotIdentifier=DBSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66f05269-7be0-47e0-a752-a01570d90266"
            }
          ]
        }
      ]
    },
    {
      "name": "Option Groups",
      "item": [
        {
          "id": "37ee5bee-2a9f-4456-bfbe-12a0e6200eda",
          "name": "copyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyOptionGroup?SourceOptionGroupIdentifier=SourceOptionGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetOptionGroupDescription=TargetOptionGroupDescription&TargetOptionGroupIdentifier=TargetOptionGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccf2d91d-26d1-48f2-98d0-630adbca42a9"
            }
          ]
        },
        {
          "id": "35d88640-2847-4fc7-a6b0-c45d153416b8",
          "name": "createoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateOptionGroup?EngineName=EngineName&MajorEngineVersion=MajorEngineVersion&OptionGroupDescription=OptionGroupDescription&OptionGroupName=OptionGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96ab7001-e7e1-4d2e-97c8-4301d52584bb"
            }
          ]
        },
        {
          "id": "ab47bcb5-ed84-4249-a427-e910eb529d04",
          "name": "deleteoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteOptionGroup?OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c52cf32d-2547-4a4a-951d-2ee033452fb7"
            }
          ]
        },
        {
          "id": "181dfd24-9bf2-4457-b708-dfa6a05d4d6a",
          "name": "describeoptiongroupoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroupOptions?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes all available options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e8819d7-25de-4bd4-bc03-20e0a37d5fc8"
            }
          ]
        },
        {
          "id": "4aa7e2f3-f231-435b-80bf-741412929d74",
          "name": "describeoptiongroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroups?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords&OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available option groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8157b727-3a1d-487f-a355-cbdbb2daebe5"
            }
          ]
        },
        {
          "id": "02459b44-cdfb-45a6-a915-895ec546ef4a",
          "name": "modifyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyOptionGroup?ApplyImmediately=ApplyImmediately&OptionGroupName=OptionGroupName&OptionsToInclude.OptionConfiguration.N=OptionsToInclude.OptionConfiguration.N&OptionsToRemove.member.N=OptionsToRemove.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b43b4e4e-91b6-4fe9-b4df-60a6b4f43ba3"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "4c1e093e-b3f3-4ca4-8274-4923d7fa8875",
          "name": "createdbinstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstance?AllocatedStorage=AllocatedStorage&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&CopyTagsToSnapshot=CopyTagsToSnapshot&DBClusterIdentifier=DBClusterIdentifier&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBName=DBName&DBParameterGroupName=DBParameterGroupName&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&Engine=Engine&EngineVersion=EngineVersion&Iops=Iops&KmsKeyId=KmsKeyId&LicenseModel=LicenseModel&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageEncrypted=StorageEncrypted&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&Timezone=Timezone&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c6b7fdd-25e9-4201-819e-30cbcf23802d"
            }
          ]
        },
        {
          "id": "88ebc2cb-a45b-4c5e-af6d-6747939e61e4",
          "name": "createdbinstancereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstanceReadReplica?AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBSubnetGroupName=DBSubnetGroupName&Iops=Iops&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&OptionGroupName=OptionGroupName&Port=Port&PubliclyAccessible=PubliclyAccessible&SourceDBInstanceIdentifier=SourceDBInstanceIdentifier&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DB instance for a DB instance running MySQL, MariaDB, or PostgreSQL that acts as a Read Replica of a source DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60fe0df0-4b0f-4f3f-b974-970b561481c2"
            }
          ]
        },
        {
          "id": "c7b15c32-a19c-48aa-907c-a1f52e314fd5",
          "name": "deletedbinstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBInstance?DBInstanceIdentifier=DBInstanceIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBInstance action deletes a previously provisioned DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef6efb49-99fa-4fef-9299-9347ebdd7317"
            }
          ]
        },
        {
          "id": "c29292d8-95fb-4da5-8790-9ddbf95298c8",
          "name": "describedbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBInstances?DBInstanceIdentifier=DBInstanceIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned RDS instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c1e606d-50b4-4e9f-bd9e-f0412da6e51a"
            }
          ]
        },
        {
          "id": "53be79fd-91b6-4024-ab01-0c02876cebc5",
          "name": "describeorderabledbinstanceoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOrderableDBInstanceOptions?DBInstanceClass=DBInstanceClass&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&LicenseModel=LicenseModel&Marker=Marker&MaxRecords=MaxRecords&Vpc=Vpc",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of orderable DB instance options for the specified engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "387c377c-6dda-4c2f-81ed-a86ca24348f0"
            }
          ]
        },
        {
          "id": "a80fcd5e-faf9-4fa8-84e5-da1bfe2e942f",
          "name": "describereserveddbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstances?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstanceId=ReservedDBInstanceId&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about reserved DB instances for this account, or about a specified reserved DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddd6b7cf-7fcc-4456-8891-bcd729684616"
            }
          ]
        },
        {
          "id": "2970b27e-1075-46c0-9fd6-003e4065403f",
          "name": "describereserveddbinstancesofferings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstancesOfferings?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists available reserved DB instance offerings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6cbc8b7-7211-49f3-9213-8dea263e0e43"
            }
          ]
        },
        {
          "id": "003aa029-6bb3-414b-bbdc-1a1425db0a96",
          "name": "modifydbinstance",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBInstance?AllocatedStorage=AllocatedStorage&AllowMajorVersionUpgrade=AllowMajorVersionUpgrade&ApplyImmediately=ApplyImmediately&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&BackupRetentionPeriod=BackupRetentionPeriod&CACertificateIdentifier=CACertificateIdentifier&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBParameterGroupName=DBParameterGroupName&DBPortNumber=DBPortNumber&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&EngineVersion=EngineVersion&Iops=Iops&LicenseModel=LicenseModel&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&NewDBInstanceIdentifier=NewDBInstanceIdentifier&OptionGroupName=OptionGroupName&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageType=StorageType&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies settings for a DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bc49ac2-398c-4562-b5b7-ec18c23ddf2b"
            }
          ]
        },
        {
          "id": "b015f511-5061-427c-a91e-8089b708e2a3",
          "name": "purchasereserveddbinstancesoffering",
          "request": {
            "url": "http://example.com/api/?Action=PurchaseReservedDBInstancesOffering?DBInstanceCount=DBInstanceCount&ReservedDBInstanceId=ReservedDBInstanceId&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Purchases a reserved DB instance offering."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b63d1467-3a24-4283-9aa1-22a1aef86815"
            }
          ]
        },
        {
          "id": "b42c21d7-1f0f-4c65-b113-6cb6b4327a7a",
          "name": "rebootdbinstance",
          "request": {
            "url": "http://example.com/api/?Action=RebootDBInstance?DBInstanceIdentifier=DBInstanceIdentifier&ForceFailover=ForceFailover",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Rebooting a DB instance restarts the database engine service."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b9649f6-e424-468f-aea6-0cd111e4d8f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnet Groups",
      "item": [
        {
          "id": "c2dfee76-9700-4a1e-8425-4222e9f97e8b",
          "name": "createdbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c552af82-878a-4b80-88c8-01df66b46e7a"
            }
          ]
        },
        {
          "id": "f5432e7d-efdb-4156-a54b-a83c289a28cd",
          "name": "deletedbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSubnetGroup?DBSubnetGroupName=DBSubnetGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c76adce3-9f61-4f48-a579-c0e71eed7f17"
            }
          ]
        },
        {
          "id": "c1cf373c-e87e-4ef8-905d-92b08f3b714a",
          "name": "describedbsubnetgroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSubnetGroups?DBSubnetGroupName=DBSubnetGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSubnetGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa6606e8-1b84-41b3-9c9b-6f94a10739f4"
            }
          ]
        },
        {
          "id": "3b70faf5-0ad9-4898-90b7-7a7d56d5d994",
          "name": "modifydbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "611c15f2-6126-44c6-bc42-947cfd2d5f50"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "4c427393-9aa4-48d7-900f-199e96041b30",
          "name": "createeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceIds.SourceId.N=SourceIds.SourceId.N&SourceType=SourceType&SubscriptionName=SubscriptionName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae80807f-f587-453a-a41c-ae33607435b1"
            }
          ]
        },
        {
          "id": "a6177ed5-5176-409e-bb8c-7a9dff6a6233",
          "name": "deleteeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSubscription?SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d23d9b25-8eb0-4ab2-b7c9-2930734bec86"
            }
          ]
        },
        {
          "id": "e169fd64-04d7-4b26-a733-eb1f2ef35c33",
          "name": "describeeventsubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventSubscriptions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the subscription descriptions for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53b2598a-ace0-4ac8-afb2-44c9e77cf549"
            }
          ]
        },
        {
          "id": "357ff823-46c7-4c9b-ad03-e70079c8d46b",
          "name": "modifyeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=ModifyEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceType=SourceType&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2cdc6cf-d574-424a-819b-e9c236d06142"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "f41c9248-fd54-44e1-995f-126eb2452c3a",
          "name": "describeaccountattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountAttributes?AccountQuotas.AccountQuota.N=AccountQuotas.AccountQuota.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the attributes for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f171d655-daa8-4f3c-9994-578422903d3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "5894db68-46dd-4671-be85-39e22240bcfa",
          "name": "describecertificates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCertificates?CertificateIdentifier=CertificateIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the set of CA certificates provided by Amazon RDS for this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "724d66a5-f6da-4699-afdd-093d66a4145b"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameters",
      "item": [
        {
          "id": "e9e9ec2b-8f49-4c65-871d-9213e420ceea",
          "name": "describedbclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameters?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84cb6a57-66bf-4bfe-91bd-49a1760ab889"
            }
          ]
        }
      ]
    },
    {
      "name": "Engines",
      "item": [
        {
          "id": "2ceef3b7-31eb-47c6-b351-d1ed1c8486cd",
          "name": "describedbengineversions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBEngineVersions?DBParameterGroupFamily=DBParameterGroupFamily&DefaultOnly=DefaultOnly&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&ListSupportedCharacterSets=ListSupportedCharacterSets&ListSupportedTimezones=ListSupportedTimezones&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available DB engines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95ed0109-c85f-4f66-8263-5d8f3875cbdb"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog Files",
      "item": [
        {
          "id": "0a4e0069-8221-4228-bdba-66ad5b6c9688",
          "name": "describedblogfiles",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBLogFiles?DBInstanceIdentifier=DBInstanceIdentifier&FileLastWritten=FileLastWritten&FilenameContains=FilenameContains&FileSize=FileSize&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB log files for the DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acc5b2eb-5a05-4218-832d-775b0e5cc7da"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "25bd4fdd-42ae-44b2-bf07-82d6f68bbaa1",
          "name": "describedbparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameters?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "727b6589-0113-4738-8898-8fec6d926d77"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Cluster Parameters",
      "item": [
        {
          "id": "3c1446d5-1969-4d5c-a07e-41aa87b95129",
          "name": "describeenginedefaultclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultClusterParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the cluster database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d6bb19d-0d8f-4753-84bc-240e497ded57"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Parameters",
      "item": [
        {
          "id": "a3f2065b-d6fe-4aa4-bf75-f7c4827b1a78",
          "name": "describeenginedefaultparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the specified database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02bd57b1-4684-45ec-a2c6-dfaa253b2475"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Categories",
      "item": [
        {
          "id": "498d9a58-9e46-4bbe-b741-32fa27f74db9",
          "name": "describeeventcategories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventCategories?Filters.Filter.N=Filters.Filter.N&SourceType=SourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Displays a list of categories for all event source types, or, if specified, for a specified source type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "745faba7-5921-43c8-ae82-28de06700851"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "2df5e88b-e07a-444f-9088-8515832ae5d8",
          "name": "describeevents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEvents?Duration=Duration&EndTime=EndTime&EventCategories.EventCategory.N=EventCategories.EventCategory.N&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SourceIdentifier=SourceIdentifier&SourceType=SourceType&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns events related to DB instances, DB security groups, DB snapshots, and DB parameter groups for the past 14 days."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a7a3def-d6ac-4914-830e-f27336cd0573"
            }
          ]
        }
      ]
    },
    {
      "name": "Source Regions",
      "item": [
        {
          "id": "b4904518-9d1c-43ea-a879-1bd812af934f",
          "name": "describesourceregions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSourceRegions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&RegionName=RegionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the source AWS regions where the current AWS region can create a Read Replica \n            or copy a DB snapshot from."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "750af5e4-94a0-4738-90b0-2ebbd8035011"
            }
          ]
        }
      ]
    },
    {
      "name": "Log Files",
      "item": [
        {
          "id": "283345a1-ef2d-4ca1-9ca1-405ae9cc17d2",
          "name": "downloaddblogfileportion",
          "request": {
            "url": "http://example.com/api/?Action=DownloadDBLogFilePortion?DBInstanceIdentifier=DBInstanceIdentifier&LogFileName=LogFileName&Marker=Marker&NumberOfLines=NumberOfLines",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Downloads all or a portion of the specified log file, up to 1 MB in size."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a99286fb-911f-431e-8fba-0924319b3204"
            }
          ]
        }
      ]
    },
    {
      "name": "Replicas",
      "item": [
        {
          "id": "0431338e-4cc7-48df-bfa6-74e18002d351",
          "name": "promotereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=PromoteReadReplica?BackupRetentionPeriod=BackupRetentionPeriod&DBInstanceIdentifier=DBInstanceIdentifier&PreferredBackupWindow=PreferredBackupWindow",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Promotes a Read Replica DB instance to a standalone DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "978321e4-4757-4141-8e0b-fe3ed5d52c96"
            }
          ]
        },
        {
          "id": "3cc08a2d-6121-48d2-8f07-42c303391dc9",
          "name": "promotereadreplicadbcluster",
          "request": {
            "url": "http://example.com/api/?Action=PromoteReadReplicaDBC