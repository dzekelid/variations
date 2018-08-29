---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Create a new product with multiple product variants
  description: Create a new product with multiple product variants.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/variants/34705478094.json:
    put:
      summary: Update an existing product variant
      description: Update an existing product variant.
      operationId: putAdminVariants34705478094.json
      x-api-path-slug: adminvariants34705478094-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Product
      - Variant
  /admin//variants/25831837123.json:
    get:
      summary: Get a product variant by id
      description: Get a product variant by id.
      operationId: getAdminVariants25831837123.json
      x-api-path-slug: adminvariants25831837123-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Variant
      - By
      - Id
  /admin/products/7990943555/variants.json:
    post:
      summary: Create a new product variant
      description: Create a new product variant.
      operationId: postAdminProducts7990943555Variants.json
      x-api-path-slug: adminproducts7990943555variants-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Variant
  /admin/products/7990943555/variants/34705478094.json:
    delete:
      summary: Delete a product variant
      description: Delete a product variant.
      operationId: deleteAdminProducts7990943555Variants34705478094.json
      x-api-path-slug: adminproducts7990943555variants34705478094-json-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Variant
  /admin/products/9579007950.json:
    put:
      summary: Update a product and one of its variants
      description: Update a product and one of its variants.
      operationId: putAdminProducts9579007950.json
      x-api-path-slug: adminproducts9579007950-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Its
      - Variants
  /admin/products.json:
    post:
      summary: Create a new product with multiple product variants
      description: Create a new product with multiple product variants.
      operationId: postAdminProducts.json
      x-api-path-slug: adminproducts-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Multiple
      - Product
      - Variants
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