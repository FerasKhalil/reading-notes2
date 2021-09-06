# Read: Class 33 Authentication & Production Server

### SON Web Tokens
- JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
- Scenarios where JSON web tokens are useful: 
	1. Authorization
	2. Information Exchange

- JSON Web Token structure:
	- Header
	- Payload
	- Signature

- Source from (https://jwt.io/introduction/)

### DRF JWT Authentication
-  The JWT is just an authorization token that should be included in all requests:
	- Command for that: 
	- $ curl http://127.0.0.1:8000/hello/ -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNTQzODI4NDMxLCJqdGkiOiI3ZjU5OTdiNzE1MGQ0NjU3OWRjMmI0OTE2NzA5N2U3YiIsInVzZXJfaWQiOjF9.Ju70kdcaHKn1Qaz8H42zrOYk0Jx9kIckTn9Xx7vhikY'


- Source from(https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)


### Django Runserver Is Not Your Production Server
- If you want to run Django in production, be sure to use a production-ready web server like Nginx, and let your app be handled by a WSGI application server like Gunicorn.
- If you plan on running on Heroku, a web server is provided implicitly. You don’t have to take care of it. You just need to specify a command to run your application server (again, Gunicorn is fine) in the Procfile.

- Source from (https://build.vsupalov.com/django-runserver-in-production/)