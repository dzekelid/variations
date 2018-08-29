swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/products/variants:
    get:
      summary: Retrieve variant with parameters
      description: Returns a `Variant` object list from the BigCommerce Catalog.
      operationId: V3CatalogProductsVariantsByStoreHashGet
      x-api-path-slug: store-hashv3catalogproductsvariants-get
      parameters:
      - in: query
        name: sku
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Variant
      - Parameters
  /{store_hash}/v3/catalog/products/{id}/variants/{id}:
    get:
      summary: Retrieve a single variant
      description: Get a `Variant` object.
      operationId: V3CatalogProductsVariantsIdByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidvariantsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Single
      - Variant
    put:
      summary: Update a variant
      description: Update a `Variant` object.
      operationId: V3CatalogProductsVariantsIdByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogproductsidvariantsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Variant
    delete:
      summary: Delete a variant
      description: Delete a `Variant`
      operationId: V3CatalogProductsVariantsIdByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidvariantsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Variant
  /{store_hash}/v3/catalog/products/{id}/variants/{id}/image:
    post:
      summary: Upload a variant image
      description: ""
      operationId: V3CatalogProductsVariantsIdImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidvariantsidimage-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: image_file
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Upload
      - Variant
      - Image
  /{store_hash}/v3/catalog/products/{id}/variants:
    post:
      summary: Create a variant
      description: ""
      operationId: V3CatalogProductsVariantsByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidvariants-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Variant
    get:
      summary: Retrieve a list of variants
      description: Returns a `Variant` object list from the BigCommerce Catalog.
      operationId: V3CatalogProductsVariantsByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidvariants-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - List
      - Of
      - Variants
  /{store-hash}/v3/catalog/products:
    post:
      summary: Create a new product with variants
      description: Sample request for creating a new product with variants through
        V3 Catalog API
      operationId: V3CatalogProductsByStoreHashPost
      x-api-path-slug: storehashv3catalogproducts-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Variants