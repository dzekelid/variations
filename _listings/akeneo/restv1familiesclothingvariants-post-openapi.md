---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API family variant (2.x only)
  description: Assuming that the given code is the code of an existing family
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/families/clothing/variants/clothing_colorsize:
    get:
      summary: family variant (2.x only)
      description: Assuming that the given codes are respectively the code of an existing
        family and an existing family variant
      operationId: RestV1FamiliesClothingVariantsClothingColorsizeGet
      x-api-path-slug: restv1familiesclothingvariantsclothing-colorsize-get
      responses:
        200:
          description: OK
      tags:
      - Family
      - Variant
      - (2
      - X
      - Only)
    patch:
      summary: family variant (2.x only)
      description: Assuming that the given codes are respectively the code of an existing
        family and an existing family variant
      operationId: RestV1FamiliesClothingVariantsClothingColorsizePatch
      x-api-path-slug: restv1familiesclothingvariantsclothing-colorsize-patch
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
      - Family
      - Variant
      - (2
      - X
      - Only)
  /rest/v1/families/clothing/variants:
    post:
      summary: family variant (2.x only)
      description: Assuming that the given code is the code of an existing family
      operationId: RestV1FamiliesClothingVariantsPost
      x-api-path-slug: restv1familiesclothingvariants-post
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
      - Family
      - Variant
      - (2
      - X
      - Only)
    get:
      summary: family variants (2.x only)
      description: Family variants (2.x only).
      operationId: RestV1FamiliesClothingVariantsGet
      x-api-path-slug: restv1familiesclothingvariants-get
      responses:
        200:
          description: OK
      tags:
      - Family
      - Variants
      - (2
      - X
      - Only)
    patch:
      summary: family variants (2.x only)
      description: Assuming that the given code is the code of an existing family
      operationId: RestV1FamiliesClothingVariantsPatch
      x-api-path-slug: restv1familiesclothingvariants-patch
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
      - Family
      - Variants
      - (2
      - X
      - Only)
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