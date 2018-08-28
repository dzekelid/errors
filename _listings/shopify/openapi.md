swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4602125518/risks/8609858574.json:
    delete:
      summary: Delete an erroneous risk entry
      description: Delete an erroneous risk entry.
      operationId: deleteAdminOrders4602125518Risks8609858574.json
      x-api-path-slug: adminorders4602125518risks8609858574-json-delete
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
      - Commerce
      - Erroneous
      - Risk
      - Entry