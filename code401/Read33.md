## [Json Web Tokens](https://jwt.io/introduction/)

A standard that defines a compact and self contained way to trasmit data between parties, as a JSON object. A digitally signed token

They can be encrypted or signed. 

#### When should you use one?
- Auth, When a user is logged in, each subsiquent request will include a JWT
- Information exchange, To securely trasmit data between parties 

### JWT structure
* Header
* Payload
* Signature

[a handy tool to disect and play with JWTs](https://jwt.io/#debugger-io)

A JWT is much less verbose than XML, much smaller, making it great for html and HTTP.
___
## [How to Use JWT Authentication with Django REST Framework](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

#### Installation & Setup

For this tutorial we are going to use the [`djangorestframework_simplejwt`](https://github.com/davesque/django-rest-framework-simplejwt) library, recommended by the DRF developers.

```bash
pip install djangorestframework_simplejwt
```

**settings.py**

```python
REST_FRAMEWORK = {
    'DEFAULT_AUTHENTICATION_CLASSES': [
        'rest_framework_simplejwt.authentication.JWTAuthentication',
    ],
}
```

**urls.py**

```python
from django.urls import path
from rest_framework_simplejwt import views as jwt_views

urlpatterns = [
    # Your URLs...
    path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
    path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
]
```

First you need to authenticate and obtain the token. via `/api/token/` as the endpoint, which only accepts POST requests.

`http post http://127.0.0.1:8000/api/token/ username=vitor password=123`
- This token is valid for 5 minutes

##### Refresh Token

To get a new **access token**, you should use the refresh token endpoint `/api/token/refresh/` posting the **refresh token**:

```python
http post http://127.0.0.1:8000/api/token/refresh/ refresh=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoicmVmcmVzaCIsImV4cCI6MTU0NTMwODIyMiwianRpIjoiNzAyOGFlNjc0ZTdjNDZlMDlmMzUwYjg3MjU1NGUxODQiLCJ1c2VyX2lkIjoxfQ.Md8AO3dDrQBvWYWeZsd_A1J39z6b6HEwWIUZ7ilOiPE
```

![HTTPie JWT Refresh Token](https://simpleisbetterthancomplex.com/media/2018/12/jwt-refresh-token.png)

The return is a new **access token** that you should use in the subsequent requests.

The **refresh token** is valid for the next 24 hours. When it finally expires too, the user will need to perform a full authentication again using their username and password to get a new set of **access token** + **refresh token**.

___

[Django Runserver Is Not Your Production Server](https://vsupalov.com/django-runserver-in-production/)

Our Runserver tool is purely for development and testing, It is a dev enviroment and has not been vetted for security or performance testing. 

A Production enviroment should only consist of reliable functioning code that is robustly tested. 

Similar to react a production enviroment should consist of multiple small focused components built to a specific purpose.

## How Does Django Fit In?

Your Django app does not actually _run_ as you would think a server would - waiting for requests and reacting to them. Your project provides a `uwsgi.py` file, which contains a function to be called by the application server. This function gets a Python object representing the incoming request.

This function calls your code, and produces a response object which is passed to the WSGI server. There the response is translated into a HTTP response and is passed back to the web server, which finally delivers it to the user.

## In Conclusion

If you want to run Django in production, be sure to use a production-ready web server like Nginx, and let your app be handled by a WSGI application server like [Gunicorn](https://vsupalov.com/what-is-gunicorn/).

If you plan on running on Heroku, a web server is provided implicitly. You don’t have to take care of it. You just need to specify a command to run your application server (again, Gunicorn is fine) in the Procfile.