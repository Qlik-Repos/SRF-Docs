# DeepLinks

The Custom Property **`DeepLinks`** can be applied to streams to allow users access to the Apps without having access to the Published Stream.

This allows for apps used by Mashups to be hidden when navigating the Qlik Sense Hub, while still allowing the users access to them if they have the appropriate authorisation and the Full URL for the App.

This Requires a [GroupsWithAccess](./GroupsWithAccess.md) property to be applied to the App

The Full app URL will then be accessible to any user who is a member of the group applied via `GroupsWithAccess` on the App.

