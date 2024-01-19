### Timeregistrations / time_registrations

### MongoDB: (timeregistrations):
_id
userId
taskId
sprintId
timeRegistered
description
currentTime
createdAt
updatedAt

### MySql: (time_registrations):
time_registration_id
time_registration_amount
time_registration_date
task_id
person_id
time_registration_type_id
time_registration_note

## Mapping (timeregistrations <-> time_registrations):
| MongoDB | MySQL |
|---------|-------|
| _id | time_registration_id |
| userId | person_id |
| taskId | task_id |
| sprintId | NULL (currently time_registration_date) |
| timeRegistered | time_registration_amount |
| description | time_registration_note |
| currentTime | NULL / time_registration_date |
| createdAt | NULL |
| updatedAt | NULL |

### Missing properties (MySQL):
time_registration_type_id