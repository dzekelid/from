{
  "info": {
    "name": "AWS Service Catalog API Disassociate Principal From Portfolio",
    "_postman_id": "0d038bd1-58a2-47ae-9d1e-bebca0da46fe",
    "description": "Disassociates a previously associated principal ARN from a specified\n         portfolio.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Portfolios",
      "item": [
        {
          "id": "b9d92296-7ff8-461d-a5d0-f01979a32c14",
          "name": "acceptPortfolioShare",
          "request": {
            "url": "http://example.com/api/?Action=AcceptPortfolioShare?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts an offer to share a portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62b3b5fb-59f5-4692-be8a-2185cb4f9347"
            }
          ]
        },
        {
          "id": "0abf8be0-ac83-441f-bbcb-0023aca9df9f",
          "name": "associatePrincipalWithPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=AssociatePrincipalWithPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&PrincipalARN=PrincipalARN&PrincipalType=PrincipalType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified principal ARN with the specified portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9872bb9-8ae5-4062-8b97-23cb998c116d"
            }
          ]
        },
        {
          "id": "b5e54214-ec75-4fae-b0aa-445cea5e356e",
          "name": "associateProductWithPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=AssociateProductWithPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&ProductId=ProductId&SourcePortfolioId=SourcePortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates a product with a portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e73691d7-2028-423f-82c8-c43ff797b936"
            }
          ]
        },
        {
          "id": "c349369d-d5a3-4fa3-b49d-71cba77c5251",
          "name": "createPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=CreatePortfolio?AcceptLanguage=AcceptLanguage&Description=Description&DisplayName=DisplayName&IdempotencyToken=IdempotencyToken&ProviderName=ProviderName&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "110f8b59-40ae-479e-a76c-bc056a63e7c3"
            }
          ]
        },
        {
          "id": "57bfc8bd-efe1-4afd-be90-01aea072dc55",
          "name": "createPortfolioShare",
          "request": {
            "url": "http://example.com/api/?Action=CreatePortfolioShare?AcceptLanguage=AcceptLanguage&AccountId=AccountId&PortfolioId=PortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new portfolio share."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4c97c6d-4edf-4377-a4cb-d28234339848"
            }
          ]
        },
        {
          "id": "f3c585ac-9289-4f7a-9446-95193b9fafa9",
          "name": "deletePortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DeletePortfolio?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c041dbd-0497-432e-b428-451eb0dd69a5"
            }
          ]
        },
        {
          "id": "172ca9a5-3bf9-4641-a77e-6fdc27e3108b",
          "name": "deletePortfolioShare",
          "request": {
            "url": "http://example.com/api/?Action=DeletePortfolioShare?AcceptLanguage=AcceptLanguage&AccountId=AccountId&PortfolioId=PortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified portfolio share."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d25076a0-ab5a-4878-8f2c-581101747110"
            }
          ]
        },
        {
          "id": "16f469ef-6fce-43a8-9062-96d6abc54871",
          "name": "describePortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DescribePortfolio?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves detailed information and any tags associated with the specified\n         portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2800b56f-27b4-442e-8b73-8ed1b9aec9a8"
            }
          ]
        },
        {
          "id": "5692de4b-e1cf-4fc2-877a-359ac60db52e",
          "name": "disassociatePrincipalFromPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DisassociatePrincipalFromPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&PrincipalARN=PrincipalARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates a previously associated principal ARN from a specified\n         portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfffe739-d422-4278-b07f-c00f95bba612"
            }
          ]
        }
      ]
    },
    {
      "name": "Constraints",
      "item": [
        {
          "id": "00494d98-b4d4-4c7e-9be3-b6762c6c95f5",
          "name": "createConstraint",
          "request": {
            "url": "http://example.com/api/?Action=CreateConstraint?AcceptLanguage=AcceptLanguage&Description=Description&IdempotencyToken=IdempotencyToken&Parameters=Parameters&PortfolioId=PortfolioId&ProductId=ProductId&Type=Type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new constraint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "372459e9-962d-4e75-aa0c-2d43650ab7ca"
            }
          ]
        },
        {
          "id": "8953e8f1-0f15-4d52-b824-5eaadab53a7c",
          "name": "deleteConstraint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConstraint?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified constraint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90814e4a-a360-404c-aa0a-8ab1dbdfb6e3"
            }
          ]
        },
        {
          "id": "04720da3-501d-417c-b787-3e4c4d81945c",
          "name": "describeConstraint",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConstraint?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves detailed information for a specified constraint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed7634d7-df0f-4c57-8e1d-a518dbf51f01"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "e3ded155-bcbd-44d8-8d1f-c3139bfa0824",
          "name": "createProduct",
          "request": {
            "url": "http://example.com/api/?Action=CreateProduct?AcceptLanguage=AcceptLanguage&Description=Description&Distributor=Distributor&IdempotencyToken=IdempotencyToken&Name=Name&Owner=Owner&ProductType=ProductType&ProvisioningArtifactParameters=ProvisioningArtifactParameters&SupportDescription=SupportDescription&SupportEmail=SupportEmail&SupportUrl=SupportUrl&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e395a6b3-066c-44b8-8c04-571409367d1d"
            }
          ]
        },
        {
          "id": "dc47c276-b7e4-43a9-8322-dec4f3ce873e",
          "name": "deleteProduct",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProduct?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c38ea391-258f-4731-a675-904d646044eb"
            }
          ]
        },
        {
          "id": "f3d71c51-9df4-48ed-b33f-697147f6186d",
          "name": "describeProduct",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProduct?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c46342f7-5c3a-4679-aa2d-bc538e3bc6d6"
            }
          ]
        },
        {
          "id": "d835a672-3d91-416e-9d18-dd1fbfe675fb",
          "name": "describeProductAsAdmin",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProductAsAdmin?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a specified product, run with administrator\n         access."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56037edb-a30e-4186-a399-5b093833a493"
            }
          ]
        },
        {
          "id": "2eacb390-d309-465b-b2da-61de5c20b562",
          "name": "describeProductView",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProductView?AcceptLanguage=AcceptLanguage&Id=Id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf5151f4-f11f-4dbe-95d2-182817666166"
            }
          ]
        }
      ]
    },
    {
      "name": "Provisioning Artifacts",
      "item": [
        {
          "id": "e79fdabd-d65e-49b1-bebf-4790e947aa1c",
          "name": "createProvisioningArtifact",
          "request": {
            "url": "http://example.com/api/?Action=CreateProvisioningArtifact?AcceptLanguage=AcceptLanguage&IdempotencyToken=IdempotencyToken&Parameters=Parameters&ProductId=ProductId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new provisioning artifact for the specified product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac6362a4-670e-4c5a-a41f-b18f7113bdf1"
            }
          ]
        },
        {
          "id": "c627f61b-9b94-4e58-b9c4-551fc5cc01b1",
          "name": "deleteProvisioningArtifact",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProvisioningArtifact?AcceptLanguage=AcceptLanguage&ProductId=ProductId&ProvisioningArtifactId=ProvisioningArtifactId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified provisioning artifact."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e60f1c70-7894-4cf9-b14c-760b1ff8ecb7"
            }
          ]
        },
        {
          "id": "48583a52-270b-4682-865b-8c8626bb15c5",
          "name": "describeProvisioningArtifact",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProvisioningArtifact?AcceptLanguage=AcceptLanguage&ProductId=ProductId&ProvisioningArtifactId=ProvisioningArtifactId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves detailed information about the specified provisioning artifact."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8cfd751-026a-4761-aca7-e5ab0348ecc2"
            }
          ]
        }
      ]
    },
    {
      "name": "Provisioning Parameters",
      "item": [
        {
          "id": "f7778dbb-77a0-477d-ae87-a52b9e901eb5",
          "name": "describeProvisioningParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeProvisioningParameters?AcceptLanguage=AcceptLanguage&PathId=PathId&ProductId=ProductId&ProvisioningArtifactId=ProvisioningArtifactId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about parameters required to provision a specified product in a\n         specified manner."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf2e59b3-2003-4264-9867-765c69c75a2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "11a61569-45fe-44d8-af86-c74716e8e81c",
          "name": "describeRecord",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRecord?AcceptLanguage=AcceptLanguage&Id=Id&PageSize=PageSize&PageToken=PageToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a paginated list of the full details of a specific request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29b18281-432a-44ce-b61c-51e65cb42200"
            }
          ]
        }
      ]
    }
  ]
}