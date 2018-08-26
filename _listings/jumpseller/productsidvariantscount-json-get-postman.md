{
  "info": {
    "name": "Jumpseller Get Products Variants Count",
    "_postman_id": "c6dbfe52-9dbf-42ff-b1b6-693ba5e0cddf",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "a7911101-40a7-41a5-9779-aeab439fef52",
          "name": "getCountries.json",
          "request": {
            "url": "http://api.jumpseller.com/v1/countries.json?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all countries.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8ce2222-8079-4080-9700-8ee295165614"
            }
          ]
        },
        {
          "id": "8b6479dc-036d-4eaf-a342-771c45bafcb2",
          "name": "getCountriesCountryCode.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a single country information.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "768a7045-3dd6-46d6-b059-ccae2833ebd6"
            }
          ]
        },
        {
          "id": "e0a81ff4-56bf-4d97-bcef-17dac5fab97e",
          "name": "getCountriesCountryCodeRegions.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code/regions.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all regions from a single country.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4a8c580-3f23-42ed-b598-9e957e62cfca"
            }
          ]
        },
        {
          "id": "da9ae80f-0c9e-4ca1-b2c7-0e64bb4cd31b",
          "name": "getCountriesCountryCodeRegionsRegionCode.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code/regions/:region_code.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "region_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a single region information object.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "263d205a-9483-4c63-9ee2-5f2e741057c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "8e8b8ea3-b1c7-470b-95a5-f3ec31d4dc0d",
          "name": "getProductsCategoryCategoryCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/category/:category_id/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "category_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Category Category Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cf8e849-1d91-4d5e-b908-8a020e9fb7e2"
            }
          ]
        },
        {
          "id": "8d6bf207-8b2c-45ba-9fbc-f4b8f61f3b83",
          "name": "getProductsCount.json",
          "request": {
            "url": "http://api.jumpseller.com/v1/products/count.json?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e880142-8c21-4509-a79c-044916836672"
            }
          ]
        },
        {
          "id": "c85b8db7-da1e-4f3e-8b6a-8b9c3ee8ce1f",
          "name": "getProductsStatusStatusCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/status/:status/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Status Status Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2123877e-bc17-4de1-9b5d-5448b7285dd3"
            }
          ]
        },
        {
          "id": "700a8d8e-aa8f-493e-be76-32377d9b21ee",
          "name": "getProductsFieldsCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/fields/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Fields Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98e3b88a-1926-42cb-be59-8e834b962d4d"
            }
          ]
        },
        {
          "id": "ac8ff8ba-a884-40d1-83f8-7173ef2b01bd",
          "name": "getProductsImagesCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/images/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Images Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a8cb8a2-23e9-4e92-85dc-fbccb01549a8"
            }
          ]
        },
        {
          "id": "096e69f8-403d-4e94-bca5-bca78d13e5ec",
          "name": "getProductsOptionsCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/options/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Options Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6453c1e7-b276-4855-9b90-7739975f83b3"
            }
          ]
        },
        {
          "id": "084b00a2-fe66-4ac7-9213-5c01179a1aaf",
          "name": "getProductsOptionsOptionValuesCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/options/:option_id/values/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "option_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Options Option Values Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44d314ab-21c8-4e5b-be6b-ad217c18e124"
            }
          ]
        },
        {
          "id": "a76f9880-80e5-4ed2-afcd-6f1384c4bfe3",
          "name": "getProductsVariantsCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/variants/count.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Variants Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "587cfe10-101e-48c1-8122-4ff45c196f5f"
            }
          ]
        }
      ]
    }
  ]
}