swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/products/{productID}/relationships/variations:
    put:
      summary: Update Product <=> Variations Relationships
      description: '`Product Variation`''s specified in the payload willbe related
        to the `Product` any relatiosnhips to `Product Variation`''s **NOT** specified
        in payload will be removed.'
      operationId: V2ProductsRelationshipsVariationsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsvariations-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
    post:
      summary: Create Product <=> Variations Relationships
      description: Here you can add and remove `Product Variation`'s to a product.
        `Product Variation`'s specified in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsVariationsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsvariations-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
    delete:
      summary: Delete Product <=> Variations Relationships
      description: Here you can add and remove `Product Variation`'s to a product.
        Only relationships to `Product Variation`'s specified in the payload will
        be removed.
      operationId: V2ProductsRelationshipsVariationsByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsvariations-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
  /v2/variations:
    get:
      summary: Get Product Variations List
      description: Get product variations list.
      operationId: V2VariationsGet
      x-api-path-slug: v2variations-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - List