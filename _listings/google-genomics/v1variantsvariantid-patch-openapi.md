---
swagger: "2.0"
x-collection-name: Google Genomics
x-complete: 0
info:
  title: Google Genomics API Update Variant
  description: |-
    Updates a variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    This method supports patch semantics. Returns the modified variant without
    its calls.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: genomics.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/variants:
    post:
      summary: Create Variant
      description: |-
        Creates a new variant.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variants.create
      x-api-path-slug: v1variants-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants/search:
    post:
      summary: Get Variants
      description: |-
        Gets a list of variants matching the criteria.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchVariants](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L126).
      operationId: genomics.variants.search
      x-api-path-slug: v1variantssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants/{variantId}:
    delete:
      summary: Delete Variant
      description: |-
        Deletes a variant.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variants.delete
      x-api-path-slug: v1variantsvariantid-delete
      parameters:
      - in: path
        name: variantId
        description: The ID of the variant to be deleted
      responses:
        200:
          description: OK
      tags:
      - Variant
    get:
      summary: Get Variant
      description: |-
        Gets a variant by ID.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variants.get
      x-api-path-slug: v1variantsvariantid-get
      parameters:
      - in: path
        name: variantId
        description: The ID of the variant
      responses:
        200:
          description: OK
      tags:
      - Variant
    patch:
      summary: Update Variant
      description: |-
        Updates a variant.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        This method supports patch semantics. Returns the modified variant without
        its calls.
      operationId: genomics.variants.patch
      x-api-path-slug: v1variantsvariantid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      - in: path
        name: variantId
        description: The ID of the variant to be updated
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants:import:
    post:
      summary: Create Variant
      description: |-
        Creates variant data by asynchronously importing the provided information.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        The variants for import will be merged with any existing variant that
        matches its reference sequence, start, end, reference bases, and
        alternative bases. If no such variant exists, a new one will be created.

        When variants are merged, the call information from the new variant
        is added to the existing variant, and Variant info fields are merged
        as specified in
        infoMergeConfig.
        As a special case, for single-sample VCF files, QUAL and FILTER fields will
        be moved to the call level; these are sometimes interpreted in a
        call-specific context.
        Imported VCF headers are appended to the metadata already in a variant set.
      operationId: genomics.variants.import
      x-api-path-slug: v1variantsimport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants:merge:
    post:
      summary: Merge Variants
      description: |-
        Merges the given variants with existing variants.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Each variant will be
        merged with an existing variant that matches its reference sequence,
        start, end, reference bases, and alternative bases. If no such variant
        exists, a new one will be created.

        When variants are merged, the call information from the new variant
        is added to the existing variant. Variant info fields are merged as
        specified in the
        infoMergeConfig
        field of the MergeVariantsRequest.

        Please exercise caution when using this method!  It is easy to introduce
        mistakes in existing variants and difficult to back out of them.  For
        example,
        suppose you were trying to merge a new variant with an existing one and
        both
        variants contain calls that belong to callsets with the same callset ID.

            // Existing variant - irrelevant fields trimmed for clarity
            {
                "variantSetId": "10473108253681171589",
                "referenceName": "1",
                "start": "10582",
                "referenceBases": "G",
                "alternateBases": [
                    "A"
                ],
                "calls": [
                    {
                        "callSetId": "10473108253681171589-0",
                        "callSetName": "CALLSET0",
                        "genotype": [
                            0,
                            1
                        ],
                    }
                ]
            }

            // New variant with conflicting call information
            {
                "variantSetId": "10473108253681171589",
                "referenceName": "1",
                "start": "10582",
                "referenceBases": "G",
                "alternateBases": [
                    "A"
                ],
                "calls": [
                    {
                        "callSetId": "10473108253681171589-0",
                        "callSetName": "CALLSET0",
                        "genotype": [
                            1,
                            1
                        ],
                    }
                ]
            }

        The resulting merged variant would overwrite the existing calls with those
        from the new variant:

            {
                "variantSetId": "10473108253681171589",
                "referenceName": "1",
                "start": "10582",
                "referenceBases": "G",
                "alternateBases": [
                    "A"
                ],
                "calls": [
                    {
                        "callSetId": "10473108253681171589-0",
                        "callSetName": "CALLSET0",
                        "genotype": [
                            1,
                            1
                        ],
                    }
                ]
            }

        This may be the desired outcome, but it is up to the user to determine if
        if that is indeed the case.
      operationId: genomics.variants.merge
      x-api-path-slug: v1variantsmerge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variantsets:
    post:
      summary: Create Variant Set
      description: |-
        Creates a new variant set.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        The provided variant set must have a valid `datasetId` set - all other
        fields are optional. Note that the `id` field will be ignored, as this is
        assigned by the server.
      operationId: genomics.variantsets.create
      x-api-path-slug: v1variantsets-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant Set
  /v1/variantsets/search:
    post:
      summary: Get Variant Sets
      description: |-
        Returns a list of all variant sets matching search criteria.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchVariantSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L49).
      operationId: genomics.variantsets.search
      x-api-path-slug: v1variantsetssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant Set
  /v1/variantsets/{variantSetId}:
    delete:
      summary: Delete Variant Set
      description: |-
        Deletes a variant set including all variants, call sets, and calls within.
        This is not reversible.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.delete
      x-api-path-slug: v1variantsetsvariantsetid-delete
      parameters:
      - in: path
        name: variantSetId
        description: The ID of the variant set to be deleted
      responses:
        200:
          description: OK
      tags:
      - Variant Set
    get:
      summary: Get Variant Set
      description: |-
        Gets a variant set by ID.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.get
      x-api-path-slug: v1variantsetsvariantsetid-get
      parameters:
      - in: path
        name: variantSetId
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Variant Set
    patch:
      summary: Update Variant Set
      description: |-
        Updates a variant set using patch semantics.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.patch
      x-api-path-slug: v1variantsetsvariantsetid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      - in: path
        name: variantSetId
        description: The ID of the variant to be updated (must already exist)
      responses:
        200:
          description: OK
      tags:
      - Variant Set
  /v1/variantsets/{variantSetId}:export:
    post:
      summary: Export Variant Set
      description: |-
        Exports variant set data to an external destination.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.export
      x-api-path-slug: v1variantsetsvariantsetidexport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: variantSetId
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Variant Set
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