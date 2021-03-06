swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/attributes/{attributeId}/names/{lang}:
    get:
      summary: List attribute names
      description: Lists the attribute names of an attribute.
      operationId: getRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Names
  /rest/items/attributes/{attributeId}/value_market_names:
    get:
      summary: Search attribute value market names
      description: Search attribute value market names.
      operationId: getRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lang
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
      responses:
        200:
          description: OK
      tags:
      - Search
      - Attribute
      - Value
      - Market
      - Names
  /rest/items/properties/{id}/names:
    get:
      summary: List the property names
      description: Lists the names of a property in all languages. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesNames
      x-api-path-slug: restitemspropertiesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Names
  /rest/items/property_groups/{id}/names:
    get:
      summary: List the property group names of a property group
      description: Lists the property group names of a property group in all languages.
        The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Group
      - Names
      - Of
      - Property
      - Group
  /rest/items/sales_prices/{id}/names:
    get:
      summary: List names of a sales price
      description: Lists the names of a sales price in all languages. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesNames
      x-api-path-slug: restitemssales-pricesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Sales
      - Price
  /rest/items/units/{id}/names:
    get:
      summary: List unit names
      description: Lists the unit names of a unit. The ID of the unit must be specified.
      operationId: getRestItemsUnitsNames
      x-api-path-slug: restitemsunitsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Unit
      - Names
  /rest/items/{id}/images/{imageId}/names:
    get:
      summary: List names of an image
      description: Lists all names of an image. The image ID must be specified.
      operationId: getRestItemsImagesImageNames
      x-api-path-slug: restitemsidimagesimageidnames-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Image
  /rest/orders/dates/types/{typeId}/names:
    get:
      summary: List names of an order date type
      description: Lists names in all languages available of an order date type. The
        ID of the date type must be specified.
      operationId: getRestOrdersDatesTypesTypeNames
      x-api-path-slug: restordersdatestypestypeidnames-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Order
      - Date
      - Type
  /rest/payment/properties/types/names/{lang?}:
    get:
      summary: List names of property types
      description: List names of property types.
      operationId: getRestPaymentPropertiesTypesNamesLang
      x-api-path-slug: restpaymentpropertiestypesnameslang-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: lang?
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Property
      - Types
  /rest/payments/methodNames:
    get:
      summary: List payment methods names
      description: Lists all payment method names.
      operationId: getRestPaymentsMethodnames
      x-api-path-slug: restpaymentsmethodnames-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payment
      - Methods
      - Names
  /rest/properties/groups/names:
    get:
      summary: List group names
      description: Lists group names.
      operationId: getRestPropertiesGroupsNames
      x-api-path-slug: restpropertiesgroupsnames-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Names
  /rest/properties/names:
    get:
      summary: List names
      description: Lists names.
      operationId: getRestPropertiesNames
      x-api-path-slug: restpropertiesnames-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Names