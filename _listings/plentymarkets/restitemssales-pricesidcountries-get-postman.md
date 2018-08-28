{
  "info": {
    "name": "Plentymarkets List countries by sales price",
    "_postman_id": "e4fa0fd4-64d8-4205-8e10-b7c7d0b2c88c",
    "description": "Lists active countries for a sales price. The ID of the sales price must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "886db21b-263d-4c31-aaba-b233682d8790",
          "name": "getRestItemsSalesPricesCountries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/countries"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists active countries for a sales price. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfff0af3-7503-4292-bd00-3deaedbacd9d"
            }
          ]
        }
      ]
    }
  ]
}