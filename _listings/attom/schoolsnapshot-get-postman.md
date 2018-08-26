{
  "info": {
    "name": "Attom Data Solutions API Return all schools within a defined radius from a point.",
    "_postman_id": "2d253303-d51c-4434-b5dd-4dcad53bf96a",
    "description": "Search for all schools that are located within a given radius around a given latitude and longitude.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "b2f704b8-0f1a-4140-9baf-e6e526a9c55c",
          "name": "getPropertyIdList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/id?geoid=%7B%7D&maxBeds=%7B%7D&minBeds=%7B%7D&orderby=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of property IDs within a specific geography that have a specific number of beds. Use orderby to choose how you want your results sorted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0730d6f-7669-4693-803a-90fa87af938c"
            }
          ]
        },
        {
          "id": "f0a4f345-2170-4437-b388-ac4b9ea08135",
          "name": "propertyDetails",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detail?address=%7B%7D&id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get property details based on its Onboard property ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "713ca394-e565-46ac-b6b9-4841a56d969d"
            }
          ]
        },
        {
          "id": "496a7e73-0b94-4399-afd5-7ce19ce7cdbc",
          "name": "adressList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/address?address1=%7B%7D&address2=%7B%7D&orderby=%7B%7D&page=%7B%7D&pagesize=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of properties within a zip code. Use propertytype and order by to narrow down your results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc680a91-ab40-4c0b-bb39-fc75590236a5"
            }
          ]
        },
        {
          "id": "0518b31d-827e-4ca7-8324-801a1fac9d4b",
          "name": "propertySnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/snapshot?cityname=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&maxavmvalue=%7B%7D&maxLotSize1=%7B%7D&maxtaxamt=%7B%7D&minavmvalue=%7B%7D&minLotSize1=%7B%7D&mintaxamt=%7B%7D&orderby=%7B%7D&postalcode=%7B%7D&propertytype=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a list of property snapshots within a specific city that are within a desired size range and a specific property type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8d48024-2cda-431d-a58a-f06090cdf1b8"
            }
          ]
        },
        {
          "id": "bd9f02a7-8e59-4fb6-b969-6dc610e289b6",
          "name": "propertyBasicProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/basicprofile?attomid=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get basic property information and most recent transaction and taxes for a specific attom id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0c527de-39d5-4c85-a0ad-a345cb6d219b"
            }
          ]
        },
        {
          "id": "e00d5381-422f-4c33-9a0b-c9d1c3a1d645",
          "name": "propertyExpandedProfile",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/expandedprofile?address1=%7B%7D&address2=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Get a detailed property information and most recent transaction and taxes for a specific address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ffb1891-061b-49a9-817a-dd062342697f"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "d1860134-369b-4986-a2a4-9ebf2c020d1b",
          "name": "propertyDetailsWithSchools",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/detailwithschools?id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Search for a property to have the property details returned, along with the schools in the associated attendance zones."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74eee97d-fc01-43c8-98b5-51ee06b54dbf"
            }
          ]
        },
        {
          "id": "fa62c6a2-ca95-4659-bb47-2b43411d2387",
          "name": "propertySchoolSnapshot",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/school/snapshot?filetypetext=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&radius=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
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
            "description": "Search for all schools that are located within a given radius around a given latitude and longitude."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e61cfcf2-4436-4b3c-ae2c-532e2c6e0b40"
            }
          ]
        }
      ]
    }
  ]
}