---
name: Google Genomics
x-slug: google-genomics
description: Google Genomics helps the life science community organize the world&rsquo;s
  genomic information and make it accessible and useful. Big genomic data is here
  today, with petabytes rapidly growing toward exabytes. Through our extensions to
  Google Cloud Platform, you can apply the same technologies that power Google Search
  and Maps to securely store, process, explore, and share large, complex datasets.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Variations
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/apis.md
specificationVersion: "0.14"
apis:
- name: Genomics - Create Variant
  x-api-slug: v1variants-post
  description: |-
    Creates a new variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variants-post-openapi.md
- name: Genomics - Get Variants
  x-api-slug: v1variantssearch-post
  description: |-
    Gets a list of variants matching the criteria.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    Implements
    [GlobalAllianceApi.searchVariants](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L126).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantssearch-post-openapi.md
- name: Genomics - Delete Variant
  x-api-slug: v1variantsvariantid-delete
  description: |-
    Deletes a variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-delete-openapi.md
- name: Genomics - Get Variant
  x-api-slug: v1variantsvariantid-get
  description: |-
    Gets a variant by ID.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-get-openapi.md
- name: Genomics - Update Variant
  x-api-slug: v1variantsvariantid-patch
  description: |-
    Updates a variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    This method supports patch semantics. Returns the modified variant without
    its calls.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-patch-openapi.md
- name: Genomics - Create Variant
  x-api-slug: v1variantsimport-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsimport-post-openapi.md
- name: Genomics - Merge Variants
  x-api-slug: v1variantsmerge-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsmerge-post-openapi.md
- name: Genomics - Create Variant Set
  x-api-slug: v1variantsets-post
  description: |-
    Creates a new variant set.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    The provided variant set must have a valid `datasetId` set - all other
    fields are optional. Note that the `id` field will be ignored, as this is
    assigned by the server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsets-post-openapi.md
- name: Genomics - Get Variant Sets
  x-api-slug: v1variantsetssearch-post
  description: |-
    Returns a list of all variant sets matching search criteria.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    Implements
    [GlobalAllianceApi.searchVariantSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L49).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetssearch-post-openapi.md
- name: Genomics - Delete Variant Set
  x-api-slug: v1variantsetsvariantsetid-delete
  description: |-
    Deletes a variant set including all variants, call sets, and calls within.
    This is not reversible.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-delete-openapi.md
- name: Genomics - Get Variant Set
  x-api-slug: v1variantsetsvariantsetid-get
  description: |-
    Gets a variant set by ID.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-get-openapi.md
- name: Genomics - Update Variant Set
  x-api-slug: v1variantsetsvariantsetid-patch
  description: |-
    Updates a variant set using patch semantics.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-patch-openapi.md
- name: Genomics - Export Variant Set
  x-api-slug: v1variantsetsvariantsetidexport-post
  description: |-
    Exports variant set data to an external destination.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetidexport-post-openapi.md
- name: Genomics - Create Variant
  x-api-slug: v1variants-post
  description: |-
    Creates a new variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variants-post-openapi.md
- name: Genomics - Get Variants
  x-api-slug: v1variantssearch-post
  description: |-
    Gets a list of variants matching the criteria.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    Implements
    [GlobalAllianceApi.searchVariants](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L126).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantssearch-post-openapi.md
- name: Genomics - Delete Variant
  x-api-slug: v1variantsvariantid-delete
  description: |-
    Deletes a variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-delete-openapi.md
- name: Genomics - Get Variant
  x-api-slug: v1variantsvariantid-get
  description: |-
    Gets a variant by ID.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-get-openapi.md
- name: Genomics - Update Variant
  x-api-slug: v1variantsvariantid-patch
  description: |-
    Updates a variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    This method supports patch semantics. Returns the modified variant without
    its calls.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-patch-openapi.md
- name: Genomics - Create Variant
  x-api-slug: v1variantsimport-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsimport-post-openapi.md
- name: Genomics - Merge Variants
  x-api-slug: v1variantsmerge-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsmerge-post-openapi.md
- name: Genomics - Create Variant Set
  x-api-slug: v1variantsets-post
  description: |-
    Creates a new variant set.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    The provided variant set must have a valid `datasetId` set - all other
    fields are optional. Note that the `id` field will be ignored, as this is
    assigned by the server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsets-post-openapi.md
- name: Genomics - Get Variant Sets
  x-api-slug: v1variantsetssearch-post
  description: |-
    Returns a list of all variant sets matching search criteria.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    Implements
    [GlobalAllianceApi.searchVariantSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L49).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetssearch-post-openapi.md
- name: Genomics - Delete Variant Set
  x-api-slug: v1variantsetsvariantsetid-delete
  description: |-
    Deletes a variant set including all variants, call sets, and calls within.
    This is not reversible.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-delete-openapi.md
- name: Genomics - Get Variant Set
  x-api-slug: v1variantsetsvariantsetid-get
  description: |-
    Gets a variant set by ID.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-get-openapi.md
- name: Genomics - Update Variant Set
  x-api-slug: v1variantsetsvariantsetid-patch
  description: |-
    Updates a variant set using patch semantics.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-patch-openapi.md
- name: Genomics - Export Variant Set
  x-api-slug: v1variantsetsvariantsetidexport-post
  description: |-
    Exports variant set data to an external destination.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetidexport-post-openapi.md
- name: Genomics - Merge Variants
  x-api-slug: v1variantsmerge-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsmerge-post-openapi.md
- name: Genomics - Create Variant
  x-api-slug: v1variantsimport-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsimport-post-openapi.md
- name: Genomics - Update Variant
  x-api-slug: v1variantsvariantid-patch
  description: |-
    Updates a variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    This method supports patch semantics. Returns the modified variant without
    its calls.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-patch-openapi.md
- name: Genomics - Get Variant
  x-api-slug: v1variantsvariantid-get
  description: |-
    Gets a variant by ID.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-get-openapi.md
- name: Genomics - Delete Variant
  x-api-slug: v1variantsvariantid-delete
  description: |-
    Deletes a variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsvariantid-delete-openapi.md
- name: Genomics - Get Variants
  x-api-slug: v1variantssearch-post
  description: |-
    Gets a list of variants matching the criteria.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    Implements
    [GlobalAllianceApi.searchVariants](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L126).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantssearch-post-openapi.md
- name: Genomics - Create Variant
  x-api-slug: v1variants-post
  description: |-
    Creates a new variant.

    For the definitions of variants and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variants-post-openapi.md
- name: Genomics - Export Variant Set
  x-api-slug: v1variantsetsvariantsetidexport-post
  description: |-
    Exports variant set data to an external destination.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetidexport-post-openapi.md
- name: Genomics - Update Variant Set
  x-api-slug: v1variantsetsvariantsetid-patch
  description: |-
    Updates a variant set using patch semantics.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-patch-openapi.md
- name: Genomics - Get Variant Set
  x-api-slug: v1variantsetsvariantsetid-get
  description: |-
    Gets a variant set by ID.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-get-openapi.md
- name: Genomics - Delete Variant Set
  x-api-slug: v1variantsetsvariantsetid-delete
  description: |-
    Deletes a variant set including all variants, call sets, and calls within.
    This is not reversible.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetsvariantsetid-delete-openapi.md
- name: Genomics - Get Variant Sets
  x-api-slug: v1variantsetssearch-post
  description: |-
    Returns a list of all variant sets matching search criteria.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    Implements
    [GlobalAllianceApi.searchVariantSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L49).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsetssearch-post-openapi.md
- name: Genomics - Create Variant Set
  x-api-slug: v1variantsets-post
  description: |-
    Creates a new variant set.

    For the definitions of variant sets and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    The provided variant set must have a valid `datasetId` set - all other
    fields are optional. Note that the `id` field will be ignored, as this is
    assigned by the server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/power-your-science.png
  humanURL: https://cloud.google.com/genomics/
  baseURL: ://genomics.googleapis.com//
  tags: Science, Genome, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/variations/master/_listings/google-genomics/v1variantsets-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.fusion.tables.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.genomics.stack.network
- type: x-documentation
  url: https://cloud.google.com/genomics/overview
- type: x-forum
  url: https://groups.google.com/forum/#!forum/google-genomics-discuss/join
- type: x-pricing
  url: https://cloud.google.com/genomics/pricing
- type: x-rate-limits
  url: https://cloud.google.com/genomics/quotas
- type: x-support
  url: https://cloud.google.com/genomics/support
- type: x-website
  url: https://cloud.google.com/genomics/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---