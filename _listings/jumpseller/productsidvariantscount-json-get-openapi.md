---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Get Products Variants Count
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products/{id}/variants/{variant_id}.json:
    get:
      summary: Get Products Variants Variant
      description: ""
      operationId: getProductsVariantsVariant.json
      x-api-path-slug: productsidvariantsvariant-id-json-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: variant_id
        description: Id of the Product Variant
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Variants
      - Variant
      - Id
      - Json
    put:
      summary: Put Products Variants Variant
      description: ""
      operationId: putProductsVariantsVariant.json
      x-api-path-slug: productsidvariantsvariant-id-json-put
      parameters:
      - in: body
        name: body
        description: Product Variant parameters to change
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: path
        name: variant_id
        description: Id of the Product Variant
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Variants
      - Variant
      - Id
      - Json
  /products/{id}/variants.json:
    get:
      summary: Get Products Variants
      description: ""
      operationId: getProductsVariants.json
      x-api-path-slug: productsidvariants-json-get
      parameters:
      - in: path
        name: id
        description: ID of the Product
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Variants
      - Json
    post:
      summary: Post Products Variants
      description: ""
      operationId: postProductsVariants.json
      x-api-path-slug: productsidvariants-json-post
      parameters:
      - in: body
        name: body
        description: Product Variant parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Variants
      - Json
  /products/{id}/variants/count.json:
    get:
      summary: Get Products Variants Count
      description: ""
      operationId: getProductsVariantsCount.json
      x-api-path-slug: productsidvariantscount-json-get
      parameters:
      - in: path
        name: id
        description: ID of the Product
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Variants
      - Count
      - Json
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