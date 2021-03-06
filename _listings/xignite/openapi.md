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
  /GetAllCorporateActionsByExchange:
    get:
      summary: Get All Corporate Actions By Exchange
      description: Get all corporate actions for a date range in the specified exchange.
      operationId: postGetallcorporateactionsbyexchange
      x-api-path-slug: getallcorporateactionsbyexchange-get
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
      - Corporate
      - Actions
      - By
      - Exchange
  /GetCorporateActionHistory:
    get:
      summary: Get Corporate Action History
      description: Get the corporate action history for a stock for a date range.
      operationId: postGetcorporateactionhistory
      x-api-path-slug: getcorporateactionhistory-get
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
      - Corporate
      - Action
      - History
  /GetCorporateIntradayVWAP:
    get:
      summary: Get Corporate Intraday VWAP
      description: Returns a corporate intraday VWAP for a security based on the trades
        performed in a time range.
      operationId: GetCorporateIntradayVWAP
      x-api-path-slug: getcorporateintradayvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Intraday
      - VWAP
  /GetCorporateHistoricalVWAP:
    get:
      summary: Get Corporate Historical VWAP
      description: Returns a corporate intraday VWAP for a security based on the trades
        performed in a time range.
      operationId: GetCorporateHistoricalVWAP
      x-api-path-slug: getcorporatehistoricalvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Historical
      - VWAP