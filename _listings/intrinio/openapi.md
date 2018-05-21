---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 1
info:
  title: Intrinio
  description: through-our-intrinio-data-marketplace-we-offer-a-wide-selection-of-financial-data-feeds-sourced-by-our-own-proprietary-processes-as-well-as-from-many-data-vendors-the-primary-application-of-the-intrinio-api-is-for-use-in-thirdparty-applications-and-integrations-or-for-endusers-utilizing-the-excel-addin-and-google-sheets-addon-the-intrinio-api-uses-https-verbs-and-a-restful-endpoint-structure-which-makes-it-easy-to-request-data-from-intrinio-basic-authentication-is-administered-over-https-responses-are-delivered-in-json-format
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /indices:
    get:
      summary: Index Master
      description: 'Returns indices list and information for all indices covered by
        Intrinio. There are three distinct types of indices: Stock Market, SIC (Sector
        &amp; Industry), and Economic.  You can view the Stock Market Indices Master,
        SIC Indices Master, and the Economic Indices Master.'
      operationId: index-master
      x-api-path-slug: indices-get
      parameters:
      - in: query
        name: identifier
        description: ' the Intrinio symbol associated with the index: '
        type: string
      - in: query
        name: order
        description: ' returns the results in the given order: popularity | symbol'
        type: string
      - in: query
        name: page_number
        description: ' an integer greater than or equal to 1 for specifying the page
          number for the return values'
        type: string
      - in: query
        name: page_size
        description: ' an integer greater than 1 for specifying the number of results
          on each page'
        type: string
      - in: query
        name: query
        description: ' a string query search of index name or symbol with the returned
          results being the relevant securities in compacted list format'
        type: string
      - in: query
        name: type
        description: ' the type of indices specified: stock_market | economic | sic'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Indices
---