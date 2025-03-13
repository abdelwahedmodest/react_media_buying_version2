# Django Backend

This directory is intended to contain the Django backend code from the `abdelwahedmodest/media_buying_django_react` repository.

## Instructions for Moving Backend Code

1. Clone the original Django repository:
   ```bash
   git clone https://github.com/abdelwahedmodest/media_buying_django_react.git
   ```

2. Copy all Django backend files to this directory:
   ```bash
   cp -r media_buying_django_react/* /path/to/django_react/backend/
   ```

3. Make sure to exclude any unnecessary files like `.git`, `.gitignore`, etc.

4. Update the Django settings to work with the new project structure.

## Configuration

Make sure to update the Django settings to allow CORS from the frontend:

```python
# In settings.py

CORS_ALLOWED_ORIGINS = [
    "http://localhost:5173",  # Vite default development server
]

INSTALLED_APPS = [
    # ...
    'corsheaders',
    # ...
]

MIDDLEWARE = [
    # ...
    'corsheaders.middleware.CorsMiddleware',
    'django.middleware.common.CommonMiddleware',
    # ...
]
```

Make sure to install the required packages:

```bash
pip install django-cors-headers
```