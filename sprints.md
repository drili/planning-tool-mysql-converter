### Sprints

### MongoDB: (sprints):
_id
sprintName
sprintMonth
sprintYear

### MySQL (sprints):
sprint_id
sprint_name
sprint_year

## Mapping (sprints <-> sprints):
| MongoDB | MySQL |
|---------|-------|
| _id | sprint_id |
| sprintName | sprint_name |
| sprintMonth | (NULL) |
| sprintYear | sprint_year |