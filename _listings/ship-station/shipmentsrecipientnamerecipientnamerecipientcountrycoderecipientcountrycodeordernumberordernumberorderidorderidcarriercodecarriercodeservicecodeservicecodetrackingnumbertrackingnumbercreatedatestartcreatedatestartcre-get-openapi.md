---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station List Shipments with parameters
  description: |-
    Obtains a list of shipments that match the specified criteria.  Please note the following:

    - Only valid shipments with labels generated in ShipStation will be returned in the response. Orders that have been marked as shipped either through the UI or the API will not appear as they are considered external shipments.

    - To include every shipment's associated shipmentItems in the response, be sure to set the `includeShipmentItems` parameter to `true`.

    All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    shipments?recipientName={recipientName}
    &recipientCountryCode={recipientCountryCode}
    &orderNumber={orderNumber}
    &orderId={orderId}
    &carrierCode={carrierCode}
    &serviceCode={serviceCode}
    &trackingNumber={trackingNumber}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &shipDateStart={shipDateStart}
    &shipDateEnd={shipDateEnd}
    &voidDateStart={voidDateStart}
    &voidDateEnd={voidDateEnd}
    &includeShipmentItems={includeShipmentItems}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /fulfillments:
    get:
      summary: List Fulfillments w/o parameters
      description: ""
      operationId: fulfillments.get
      x-api-path-slug: fulfillments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Fulfillments
      - W
      - O
      - Parameters
  ? /fulfillments?fulfillmentId={fulfillmentId}&orderId={orderId}&orderNumber={orderNumber}&trackingNumber={trackingNumber}&recipientName={recipientName}&createDateStart={createDateStart}&createDateEnd={createDateEnd}&shipDateStart={shipDateStart}&shipDa
  : get:
      summary: List Fulfillments with parameters
      description: |-
        Obtains a list of fulfillments that match the specified criteria.  Please note the following:

        - Orders that have been marked as shipped either through the UI or the API will appear in the response as they are considered fulfillments.

        All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

        Url format with filters:

        ```
        fulfillments?fulfillmentId={fulfillmentId}
        &orderId={orderId}
        &orderNumber={orderNumber}
        &trackingNumber={trackingNumber}
        &recipientName={recipientName}
        &createDateStart={createDateStart}
        &createDateEnd={createDateEnd}
        &shipDateStart={shipDateStart}
        &shipDateEnd={shipDateEnd}
        &sortBy={sortBy}
        &sortDir={sortDir}
        &page={page}
        &pageSize={pageSize}
        ```
      operationId: fulfillments_fulfillmentId_fulfillmentId_orderId_orderId_orderNumber_orderNumber_trackingNumber_trac
      x-api-path-slug: fulfillmentsfulfillmentidfulfillmentidorderidorderidordernumberordernumbertrackingnumbertrackingnumberrecipientnamerecipientnamecreatedatestartcreatedatestartcreatedateendcreatedateendshipdatestartshipdatestartshipda-get
      parameters:
      - in: path
        name: createDateEnd
        description: Returns fulfillments created on or before the specified ``createDate``
      - in: path
        name: createDateStart
        description: Returns fulfillments created on or after the specified ``createDate``
      - in: path
        name: fulfillmentId
        description: Returns the fulfillment with the specified fulfillment ID
      - in: path
        name: orderId
        description: Returns fulfillments whose orders have the specified order ID
      - in: path
        name: orderNumber
        description: Returns fulfillments whose orders have the specified order number
      - in: path
        name: page
        description: page number
      - in: path
        name: pageSize
        description: page size
      - in: path
        name: recipientName
        description: Returns fulfillments shipped to the specified recipient name
      - in: path
        name: shipDateEnd
        description: Returns fulfillments with the ``shipDate`` on or before the specified
          date
      - in: path
        name: shipDateStart
        description: Returns fulfillments with the ``shipDate`` on or after the specified
          date
      - in: path
        name: sortBy
        description: Sort the responses by a set value
      - in: path
        name: sortDir
        description: Sets the direction of the sort order
      - in: path
        name: trackingNumber
        description: Returns fulfillments with the specified tracking number
      responses:
        200:
          description: OK
      tags:
      - List
      - Fulfillments
      - Parameters
  /orders:
    get:
      summary: List Orders w/o parameters
      description: ""
      operationId: orders.get
      x-api-path-slug: orders-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - W
      - O
      - Parameters
  ? /orders?customerName={customerName}&itemKeyword={itemKeyword}&createDateStart={createDateStart}&createDateEnd={createDateEnd}&modifyDateStart={modifyDateStart}&modifyDateEnd={modifyDateEnd}&orderDateStart={orderDateStart}&orderDateEnd={orderDateEnd}&
  : get:
      summary: List Orders with parameters
      description: |-
        Obtains a list of orders that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

        Url format with filters:

        ```
        /orders?customerName={customerName}
        &itemKeyword={itemKeyword}
        &createDateStart={createDateStart}
        &createDateEnd={createDateEnd}
        &modifyDateStart={modifyDateStart}
        &modifyDateEnd={modifyDateEnd}
        &orderDateStart={orderDateStart}
        &orderDateEnd={orderDateEnd}
        &orderNumber={orderNumber}
        &orderStatus={orderStatus}
        &paymentDateStart={paymentDateStart}
        &paymentDateEnd={paymentDateEnd}
        &storeId={storeId}
        &sortBy={sortBy}
        &sortDir={sortDir}
        &page={page}
        &pageSize={pageSize}
        ```
      operationId: orders_customerName_customerName_itemKeyword_itemKeyword_createDateStart_createDateStart_createDateE
      x-api-path-slug: orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get
      parameters:
      - in: path
        name: createDateEnd
        description: Returns orders that were created in ShipStation before the specified
          date
      - in: path
        name: createDateStart
        description: Returns orders that were created in ShipStation after the specified
          date
      - in: path
        name: customerName
        description: Returns orders that match the specified name
      - in: path
        name: itemKeyword
        description: Returns orders that contain items that match the specified keyword
      - in: path
        name: modifyDateEnd
        description: Returns orders that were modified before the specified date
      - in: path
        name: modifyDateStart
        description: Returns orders that were modified after the specified date
      - in: path
        name: orderDateEnd
        description: Returns orders less than or equal to the specified date
      - in: path
        name: orderDateStart
        description: Returns orders greater than the specified date
      - in: path
        name: orderNumber
        description: Filter by order number, performs a starts with search
      - in: path
        name: orderStatus
        description: Filter by order status
      - in: path
        name: page
        description: Page number
      - in: path
        name: pageSize
        description: Requested page size
      - in: path
        name: paymentDateEnd
        description: Returns orders that were paid before the specified date
      - in: path
        name: paymentDateStart
        description: Returns orders that were paid after the specified date
      - in: path
        name: sortBy
        description: Sort the responses by a set value
      - in: path
        name: sortDir
        description: Sets the direction of the sort order
      - in: path
        name: storeId
        description: Filters orders to a single store
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - Parameters
  /products:
    get:
      summary: List Products w/o parameters
      description: ""
      operationId: products.get
      x-api-path-slug: products-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Products
      - W
      - O
      - Parameters
  ? /products?sku={sku}&name={name}&productCategoryId={productCategoryId}&productTypeId={productTypeId}&tagId={tagId}&startDate={startDate}&endDate={endDate}&showInactive={showInactive}&sortBy={sortBy}&sortDir={sortDir}&page={page}&pageSize={pageSize}
  : get:
      summary: List Products with parameters
      description: |-
        Obtains a list of products that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

        Url format with filters:

        ```
        /products?sku={sku}
        &name={name}
        &productCategoryId={productCategoryId}
        &productTypeId={productTypeId}
        &tagId={tagId}
        &startDate={startDate}
        &endDate={endDate}
        &showInactive={showInactive}
        &sortBy={sortBy}
        &sortDir={sortDir}
        &page={page}
        &pageSize={pageSize}
        ```
      operationId: products_sku_sku_name_name_productCategoryId_productCategoryId_productTypeId_productTypeId_tagId_tag
      x-api-path-slug: productsskuskunamenameproductcategoryidproductcategoryidproducttypeidproducttypeidtagidtagidstartdatestartdateenddateenddateshowinactiveshowinactivesortbysortbysortdirsortdirpagepagepagesizepagesize-get
      parameters:
      - in: path
        name: endDate
        description: Returns products that were created before the specified date
      - in: path
        name: name
        description: Returns products that match the specified product name
      - in: path
        name: page
        description: Page number
      - in: path
        name: pageSize
        description: Requested page size
      - in: path
        name: productCategoryId
        description: Returns products that match the specified productCategoryId
      - in: path
        name: productTypeId
        description: Returns products that match the specified productTypeId
      - in: path
        name: showInactive
        description: Specifies whether the list should include inactive products
      - in: path
        name: sku
        description: Returns products that match the specified SKU
      - in: path
        name: sortBy
        description: Sorts the order of the response based off the specified value
      - in: path
        name: sortDir
        description: Sets the direction of the sort order
      - in: path
        name: startDate
        description: Returns products that were created after the specified date
      - in: path
        name: tagId
        description: Returns products that match the specified tagId
      responses:
        200:
          description: OK
      tags:
      - List
      - Products
      - Parameters
  /shipments:
    get:
      summary: List Shipments w/o parameters
      description: ""
      operationId: shipments.get
      x-api-path-slug: shipments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipments
      - W
      - O
      - Parameters
  ? /shipments?recipientName={recipientName}&recipientCountryCode={recipientCountryCode}&orderNumber={orderNumber}&orderId={orderId}&carrierCode={carrierCode}&serviceCode={serviceCode}&trackingNumber={trackingNumber}&createDateStart={createDateStart}&cre
  : get:
      summary: List Shipments with parameters
      description: |-
        Obtains a list of shipments that match the specified criteria.  Please note the following:

        - Only valid shipments with labels generated in ShipStation will be returned in the response. Orders that have been marked as shipped either through the UI or the API will not appear as they are considered external shipments.

        - To include every shipment's associated shipmentItems in the response, be sure to set the `includeShipmentItems` parameter to `true`.

        All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

        Url format with filters:

        ```
        shipments?recipientName={recipientName}
        &recipientCountryCode={recipientCountryCode}
        &orderNumber={orderNumber}
        &orderId={orderId}
        &carrierCode={carrierCode}
        &serviceCode={serviceCode}
        &trackingNumber={trackingNumber}
        &createDateStart={createDateStart}
        &createDateEnd={createDateEnd}
        &shipDateStart={shipDateStart}
        &shipDateEnd={shipDateEnd}
        &voidDateStart={voidDateStart}
        &voidDateEnd={voidDateEnd}
        &includeShipmentItems={includeShipmentItems}
        &sortBy={sortBy}
        &sortDir={sortDir}
        &page={page}
        &pageSize={pageSize}
        ```
      operationId: shipments_recipientName_recipientName_recipientCountryCode_recipientCountryCode_orderNumber_orderNum
      x-api-path-slug: shipmentsrecipientnamerecipientnamerecipientcountrycoderecipientcountrycodeordernumberordernumberorderidorderidcarriercodecarriercodeservicecodeservicecodetrackingnumbertrackingnumbercreatedatestartcreatedatestartcre-get
      parameters:
      - in: path
        name: carrierCode
        description: Returns shipments shipped with the specified carrier
      - in: path
        name: createDateEnd
        description: Returns shipments created on or before the specified ``createDate``
      - in: path
        name: createDateStart
        description: Returns shipments created on or after the specified ``createDate``
      - in: path
        name: includeShipmentItems
        description: 'Specifies whether to include shipment items with results Default
          value: false'
      - in: path
        name: orderId
        description: Returns shipments whose orders have the specified order ID
      - in: path
        name: orderNumber
        description: Returns shipments whose orders have the specified order number
      - in: path
        name: page
        description: page number
      - in: path
        name: pageSize
        description: page size
      - in: path
        name: recipientCountryCode
        description: Returns shipments shipped to the specified country code
      - in: path
        name: recipientName
        description: Returns shipments shipped to the specified recipient name
      - in: path
        name: serviceCode
        description: Returns shipments shipped with the specified shipping service
      - in: path
        name: shipDateEnd
        description: Returns shipments with the ``shipDate`` on or before the specified
          date
      - in: path
        name: shipDateStart
        description: Returns shipments with the ``shipDate`` on or after the specified
          date
      - in: path
        name: sortBy
        description: Sort the responses by a set value
      - in: path
        name: sortDir
        description: Sets the direction of the sort order
      - in: path
        name: trackingNumber
        description: Returns shipments with the specified tracking number
      - in: path
        name: voidDateEnd
        description: Returns shipments voided on or before the specified date
      - in: path
        name: voidDateStart
        description: Returns shipments voided on or after the specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipments
      - Parameters
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