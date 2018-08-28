---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Indices Real Time Search Indices By Name
  description: Search indices by name.
  version: 1.0.0
host: globalindicesrealtime.xignite.com
basePath: xglobalindicesrealtime.json/XigniteGlobalIndicesRealTime
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