# Security Rules

## Naming Conventions

- Rules Granting permissions by Role Group Membership
  - `QC_<Resource>_<Actions>|<Control>`

e.g. **QC_ReloadTasks_Read|Developers**

| Segment  | Values                            |
| -------- | --------------------------------- |
| Resource | Tasks                             |
| Access   | Read                              |
| Control     | Developer (User Group Assignment) |


- Rules Granting permissions by Custom Property Assignments
  - `QC_<Resource>_<Actions>|<CustomProperty>`
  - `QC_<Resource>_<Type>_<Actions>|<CustomProperty>`

e.g. `QC_Apps_Resource_Read|GWA`

| Segment        | Value                                   |
| -------------- | --------------------------------------- |
| Resource       | Apps                                  |
| Access         | Read                                    |
| Control | GWA (Custom Property: GroupsWithAccess) |

e.g. `QC_AppObjects_Sheets_Publish|RWP`

| Segment        | Value                                   |
| -------------- | --------------------------------------- |
| Resource       | AppObjects                              |
| Type           | Sheets                                  |
| Access         | Publish                                 |
| Control | RWP (Custom Property: RolesWithPublish) |
