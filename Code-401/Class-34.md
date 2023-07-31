[Back to Home](../README.md)

## Reading Class-34: API Deployment

1. **Key Principles for Django Settings:**

- Use separate settings modules for different environments (base, development, production, etc.).
- Store environment-specific settings in separate files.
- Utilize environment variables for sensitive information.
- Avoid committing secrets to version control.
- Import and override settings from base settings in environment-specific files.
- Group related settings together.
- Use constants and default settings for clarity.
- Follow the 12-Factor App methodology.

2. **White Noise for Efficient Static File Serving:**

- White Noise helps serve static files efficiently in Django applications.
- Install White Noise with `pip install whitenoise`.
- Add `'whitenoise.middleware.WhiteNoiseMiddleware'` to the `MIDDLEWARE` setting.
- Ensure `STATIC_ROOT` is configured and run `python manage.py collectstatic`.
- If using a separate web server, configure it to bypass static files handling.

3. **Cross-Origin Resource Sharing (CORS) in Django:**

- CORS controls how web pages hosted on one domain access resources on another.
- Install `django-cors-headers` with `pip install django-cors-headers`.
- Add `'corsheaders.middleware.CorsMiddleware'` to the `MIDDLEWARE` setting.
- Configure CORS settings based on your project's requirements:
  - Use `CORS_ALLOW_ALL_ORIGINS = True` for any origin (not recommended for production).
  - Use `CORS_ALLOWED_ORIGINS` to specify specific origins.
- CORS ensures secure resource access in web applications.

*- Author: Almothana Almasri*