# Account

    GET accounts/:account_id/plans
    
Returns a list of [Plans][] an Account has access to

## Parameters
None

## Example
**Request**

    https://api.zingle.me/v1/accounts/2d89b706-47f2-471d-8e1b-4a180b448838/plans

**Return**
``` json
{
    "status": {
        "text": "OK",
        "status_code": 200,
        "description": null,
        "sort_field": "display_name",
        "sort_direction": "asc",
        "page": 1,
        "page_size": 10,
        "total_pages": 1,
        "total_records": 3
    },
    "result": [
        {
          "id": "a0ec6d49-caa8-4bd2-ae15-acb529a2ca98",
          "code": "zingle_basic",
          "monthly_or_unit_price": 55,
          "term_months": 1,
          "setup_price": 0,
          "display_name": "Zingle Basic",
          "is_printer_plan": false
        },
        {
          "id": "828f6bb7-bda8-4c00-829b-3a9c372b0324",
          "code": "zingle_pro",
          "monthly_or_unit_price": 99,
          "term_months": 1,
          "setup_price": 0,
          "display_name": "Zingle Pro",
          "is_printer_plan": false
        }    
    ]
}
```

[Plans]: /plans/README.md