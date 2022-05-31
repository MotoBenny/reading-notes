## [Django Rest Framework Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

Permissions checks run at the start of a given requests or view, no other code runs until the check finishes.

Permissions in DRF are always defined as a list of permission classes.
When the permission checks fail, either a "403 Forbidden" or a "401 Unauthorized" response will be returned

generic view does not automatically apply object level permissions to each instance in a queryset.

[API Reference](https://www.django-rest-framework.org/api-guide/permissions/#api-reference)
The Reference section of the documentation covers the different permission classes built into DRF.

A user can also create custom permission classes. 
To implement a custom permission, override `BasePermission` and implement either, or both, of the following methods:

-   `.has_permission(self, request, view)`
-   `.has_object_permission(self, request, view, obj)`

