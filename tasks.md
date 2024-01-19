### Tasks

### MongoDB: (tasks):
_id
taskName
taskTimeLow
taskTimeHigh
taskCustomer
taskLabel
taskVertical
taskPersons (array)
taskSprints (array)
createdBy
isArchived
workflowStatus
createdAt
updatedAt

### MySQL: (tasks):
task_id
task_name
task_low
task_high
task_workflow_status
task_description
sprint_id
project_id
customer_id
label_id
task_type_id
task_vertical_id
customer_project_id
is_external

## Mapping (tasks <-> tasks):
| MongoDB | MySQL |
|---------|-------|
| _id | task_id |
| taskName | task_name |
| taskLow | task_low |
| taskHigh | task_high |
| taskCustomer | customer_id |
| taskLabel | label_id |
| taskVertical | task_vertical_id |
| taskPersons (array) | NULL (task persons inside task_persons table) |
| taskSprints (array) | sprint_id (NOTICE: taskSprints is array) |
| createdBy | NULL |
| isArchived | NULL |
| workflowStatus | task_workflow_status |
| createdAt | NULL |
| updatedAt | NULL |

### Missing properties (MySQL):
project_id
customer_project_id
is_external