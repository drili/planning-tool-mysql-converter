### Customers

### MongoDB: (customers):
_id
customerName
customerColor
isArchived

### MySQL (customers):
customer_id
customer_name
customer_cvr
customer_color
customer_hourly_rate
customer_enabled
is_active_campaigns

## Mapping (customers <-> customers):
| MongoDB | MySQL |
|---------|-------|
| _id | customer_id |
| customerName | customer_name |
| customerColor | customer_color |
| isArchived | customer_enabled |

### Missing properties (MySQL):
customer_cvr
customer_hourly_rate
is_active_campaigns