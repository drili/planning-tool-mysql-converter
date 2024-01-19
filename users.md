### Users / Persons

### MongoDB: (users):
_id
username
email
password
isActivated
profileImage
userRole
userTitle
createdAt
updatedAt
activeYear

### MySQL (persons):
person_id
person_name
person_email
person_password
person_image
permission_role_id
person_enabled
person_is_external
person_phone_no
secret_key

## Mapping (users <-> persons):
| MongoDB | MySQL |
|---------|-------|
| _id | person_id |
| username | person_name |
| email | person_email |
| password | person_password |
| isActivated | person_enabled |
| profileImage | person_image |
| userRole | permission_role_id |
| userTitle | (NULL), default: employee |
| createdAt | (NULL) |
| updatedAt | (NULL) |
| activeYear |(NULL), default: 2024 |

### Missing properties (MySQL):
person_is_external
person_phone_no
secret_key