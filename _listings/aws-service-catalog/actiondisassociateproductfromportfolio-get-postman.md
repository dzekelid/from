{
  "info": {
    "name": "AWS Service Catalog API Disassociate Product From Portfolio",
    "_postman_id": "3d3669f1-ebfa-4f6c-8988-07cdd7a13615",
    "description": "Disassociates the specified product from the specified portfolio.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Portfolios",
      "item": [
        {
          "id": "62fc6a30-3e7f-4395-a3c6-1e66ad62c491",
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
              "id": "064afbbc-f92e-428c-89d7-8e57bdc486ce"
            }
          ]
        },
        {
          "id": "3a03a1bd-b49b-433b-966a-a28e9d7d0b94",
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
              "id": "dbb96f73-a6fa-4343-8b4d-d84dbfbdf915"
            }
          ]
        },
        {
          "id": "6c016af2-a041-4f9a-b63f-d7f9eb6092c8",
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
              "id": "3bb2d1d6-4d6a-456e-9afc-275d3b76f863"
            }
          ]
        },
        {
          "id": "cfa6dd03-bbff-4749-abd8-c36604a96401",
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
              "id": "80549571-51a1-47ca-a1ff-8dfceef71841"
            }
          ]
        },
        {
          "id": "369e0193-574a-4032-83e2-ab1697b0b1f1",
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
              "id": "6aa55de4-e317-4440-ab73-81ed81a41176"
            }
          ]
        },
        {
          "id": "5f5721e5-cd16-4d12-83db-fbd5c36c301d",
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
              "id": "f319f40c-a63f-4826-b004-8d037383f3b3"
            }
          ]
        },
        {
          "id": "138ce911-c437-4d33-9657-6af48e5f7e45",
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
              "id": "f1a6b5cf-389f-4fbe-be31-31242d4b1aac"
            }
          ]
        },
        {
          "id": "4a814ad4-ada2-4669-b439-d33fe57e2dda",
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
              "id": "37a8d9e5-002f-4e46-a09c-fdd7c55b1216"
            }
          ]
        },
        {
          "id": "68dc9e18-3456-4927-9021-aedbae84aedf",
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
              "id": "eff145fc-8cff-49b1-ae75-a076f30b77ed"
            }
          ]
        },
        {
          "id": "140a9541-8156-4256-862e-2e38378d6da7",
          "name": "disassociateProductFromPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateProductFromPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&ProductId=ProductId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified product from the specified portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ed2e73a-58c4-46a5-a686-08ba64031d1e"
            }
          ]
        }
      ]
    },
    {
      "name": "Constraints",
      "item": [
        {
          "id": "605c025a-db96-4909-8d2d-a63385fbc994",
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
              "id": "18e73d11-540f-4393-938e-603495bf4200"
            }
          ]
        },
        {
          "id": "1648467c-854b-4b8e-9ff0-5d6a44b8f72b",
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
              "id": "2c87913d-6d11-4ec7-9307-f4522eeeb269"
            }
          ]
        },
        {
          "id": "5e353ce0-56a2-4be2-8f1f-4276ec35554b",
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
              "id": "059d8a5f-972e-42d5-90fb-7540b78eb5ca"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "f0bb787f-da98-4dc1-9eff-1b0341524b78",
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
              "id": "9c2d3205-83f3-4d65-924c-e83ee27c18d0"
            }
          ]
        },
        {
          "id": "0e5b5325-3047-4275-9335-5164a5f770dd",
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
              "id": "a6412367-05f8-4c1c-9185-e4df28695239"
            }
          ]
        },
        {
          "id": "9ae2ea41-4ee5-4ea2-a5e1-ddd0ac14ff1c",
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
              "id": "9c370d4f-5b23-4af0-ae4b-30a1a6c6d601"
            }
          ]
        },
        {
          "id": "d4f11a51-f861-4674-86d9-b639c75acb20",
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
              "id": "5f4b4e0a-d86c-46bd-ba14-60a940c9d472"
            }
          ]
        },
        {
          "id": "648b898e-f38a-4774-9f1b-aa3ac5ee7f4e",
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
              "id": "ba4a518d-abb3-412c-93ba-cb283d551c07"
            }
          ]
        }
      ]
    },
    {
      "name": "Provisioning Artifacts",
      "item": [
        {
          "id": "84f9a437-fd1f-484f-9d49-64eba2d735d4",
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
              "id": "aa25fd54-e165-43b5-ba94-99ee0d8aa04b"
            }
          ]
        },
        {
          "id": "5134b967-98e9-4c85-bde7-5275c78ce8b3",
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
              "id": "73e8f480-c0da-4783-a99f-a1136ec93482"
            }
          ]
        },
        {
          "id": "f08797d0-6b1b-43bd-9173-4498e53aa324",
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
              "id": "27159862-abe4-40ab-8b55-6aaf8e38bbe9"
            }
          ]
        }
      ]
    },
    {
      "name": "Provisioning Parameters",
      "item": [
        {
          "id": "16b59741-9879-4e80-bdc8-9c985915c74b",
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
              "id": "2a8e8dc3-ffa6-4bb3-ab34-c512566045a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "8978d787-9343-49df-be4e-cdf0cba4f2c9",
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
              "id": "fdb06291-45ff-488b-add4-8344102feec4"
            }
          ]
        }
      ]
    }
  ]
}