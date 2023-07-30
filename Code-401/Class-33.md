[Back to Home](../README.md)

## Reading Class-33: Authentication & Production Server

1- **Purpose of JSON Web Tokens (JWTs)**:
JWTs are used for securely transmitting information between parties as a JSON object. They are commonly used for authentication and authorization in web applications. JWTs consist of three parts: header, payload, and signature. The header and payload are Base64 URL encoded, and the signature is used to verify data integrity.

2- **JWT Authentication with Django REST Framework**:
JWT authentication can be integrated with Django REST Framework using the `djangorestframework-simplejwt` library. Key components include TokenObtainPairView for issuing tokens, TokenRefreshView for refreshing access tokens, and TokenVerifyView for token validation.

3- **Why Django's runserver is not suitable for production**:
Django's built-in runserver is not optimized for production environments in terms of performance, security, and stability. It lacks essential features like load balancing and process management. Production-ready options include Gunicorn, uWSGI, nginx, and Apache, often used with a reverse proxy. Follow best practices for configuration and security in production.

*- Author: Almothana Almasri*