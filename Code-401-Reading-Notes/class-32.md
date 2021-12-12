# class_32
## Django REST framework
### permission 
Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.
<br>
### How permissions are determined
If any permission check fails, an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.
<br>
### Object level permissions
Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.
<br>
Object level permissions are run by REST framework's generic views when .get_object() is called. As with view level permissions, an exceptions.PermissionDenied exception will be raised if the user is not allowed to act on the given object.
<br>
### Setting the permission policy
`REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}`

`'DEFAULT_PERMISSION_CLASSES': [
   'rest_framework.permissions.AllowAny',
]`

`from rest_framework.permissions import IsAuthenticated<br>
from rest_framework.response import Response<br>
from rest_framework.views import APIView`

`class ExampleView(APIView):
    permission_classes = [IsAuthenticated]

    def get(self, request, format=None):
        content = {
            'status': 'request was permitted'
        }
        return Response(content)`
    
  ### API Reference
  * **AllowAny** : The AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.
  * **IsAuthenticated** : The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise.
  * **IsAdminUser**:The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.
  * **IsAuthenticatedOrReadOnly**: The IsAuthenticatedOrReadOnly will allow authenticated users to perform any request.
