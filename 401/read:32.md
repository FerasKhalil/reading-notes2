# Read: Class 32 Permissions & Postgresql

## DRF Permissions

- Permission checks are always run at the very start of the view, before any other code is allowed to proceed. 

- Permission checks will typically use the authentication information in the request.user and request.auth properties 
to determine if the incoming request should be permitted.

- Permissions are used to grant or deny access for different classes of users to different parts of the API.

- The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user.

	- This corresponds to the IsAuthenticated class in REST framework.

- A less strict style of permission is read only

	- This corresponds to the IsAuthenticatedOrReadOnly class in REST framework.

- 403: Forbidden

	- The request was successfully authenticated, but permission was denied.

	- The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers.

- 401: Unauthorized

	- The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. 

- REST framework permissions also support Object level permissioning.

	- Object level permissions:

		- used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

		- Object level permissions are run by REST framework's generic views when .get_object() is called.

i. IsAuthenticated: Permission class will deny permission to any unauthenticated user.
	- This permission is suitable if you want your API to only be accessible to registered users.

ii. IsAdminUser: Permission class will deny permission to any user, unless user.is_staff is True.
	- This permission is suitable if you want your API to only be accessible to a subset of trusted administrators.

iii. IsAuthenticatedOrReadOnly: will allow authenticated users to perform any request of the safe methods(GET, HEAD, OPTIONS).
	- This permission is suitable if you want to your API to allow read permissions to anonymous users, and only allow write permissions to authenticated users.

iiii. DjangoModelPermissions:  This permission must only be applied to views that have a .queryset property or get_queryset() method.
	- Authorization will only be granted if the user is authenticated and has the relevant model permissions assigned.
	- POST requests require the user to have the add permission on the model.
	- PUT and PATCH requests require the user to have the change permission on the model.
	- DELETE requests require the user to have the delete permission on the model.

iiiii. DjangoModelPermissionsOrAnonReadOnly
	- Similar to DjangoModelPermissions, but also allows unauthenticated users to have read-only access to the API.


- Source from (https://www.django-rest-framework.org/api-guide/permissions/)