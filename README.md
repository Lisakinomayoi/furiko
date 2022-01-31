# README
## users_table
| Column                | Type   | Options                   |
| --------------------- | ------ | ------------------------- |   
| user_name             | string | null: false               |
| password              | string | null: false               |
| password_confirmation | string | null: false               |
| first_name            | string | null: false               |
| last_name             | string | null: false               |
| email                 | string | null: false, unique: true |
| date_of_birth         | date   | null: false               |

### Association
- has_many itmems
- has_many orders

## items_table
| Column                 | Type | Options |
| ---------------------- | ---- | ------- |
| name                   | string 
| info                   | text 
| category_id            | integer
| sales_status_id        | integer
| shopping_fee_status_id | integer
| state_id               | integer
| scheduled_delivery_id  | integer
| price                  | integer
| user                   | reference

## oreders_table
| Column | Type | Options |
| ------ | ---- | ------- |

## sending_information table
| Column | Type | Options |
| ------ | ---- | ------- |