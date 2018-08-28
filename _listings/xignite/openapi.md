swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetDelayedIndicesValue:
    get:
      summary: Get Delayed Indices Value
      description: Get delayed indices value.
      operationId: GetDelayedIndicesValue
      x-api-path-slug: getdelayedindicesvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Delayed
      - Indices
      - Value
  /ListIndicesByIndexGroup:
    get:
      summary: List Indices By Index Group
      description: List indices by index group.
      operationId: ListIndicesByIndexGroup
      x-api-path-slug: listindicesbyindexgroup-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Indices
      - Index
      - Group
  /SearchIndicesByName:
    get:
      summary: Search Indices By Name
      description: Search indices by name.
      operationId: SearchIndicesByName
      x-api-path-slug: searchindicesbyname-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Indices
      - Name
  /GetLastClosingIndicesValue:
    get:
      summary: Get Last Closing Indices Value
      description: Get last closing indices value.
      operationId: GetLastClosingIndicesValue
      x-api-path-slug: getlastclosingindicesvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Indices
      - Value
  /GetHistoricalIndicesValue:
    get:
      summary: Get Historical Indices Value
      description: Get historical indices value.
      operationId: GetHistoricalIndicesValue
      x-api-path-slug: gethistoricalindicesvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Indices
      - Value
  /GetRealTimeIndicesValue:
    get:
      summary: Get Real Time Indices Value
      description: Get real time indices value.
      operationId: GetRealTimeIndicesValue
      x-api-path-slug: getrealtimeindicesvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Indices
      - Value