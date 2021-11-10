# GroupsWithAccess
The GroupsWithAccess custom property is used to determine if the user is Authorised to access the resources the property has been applied to.

When defined the value of the custom property is compared to the users group membership. 

If the comparison results in **True**, the resource is available. 

It is suggested that if a resource should be available to all users then a specific group is established that includes all users. I.e. Qlik_Access.

the GroupsWithAccess custom property will need to be updated with all the groups that need to be assigned to resources within the environment.