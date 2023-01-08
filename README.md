# **[Django Admin Soft PRO](https://appseed.us/product/soft-ui-dashboard-pro/django/)**

**Django** starter styled with **[Django Admin Soft PRO](https://appseed.us/product/soft-ui-dashboard-pro/django/)**, a premium `Boostrap 5` design from [Creative-Tim](https://bit.ly/3fKQZaL)
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-soft-pro`

<br />

## Features: 

- **UI Kit**: Soft Dashboard BS5 PRO `v1.1.1` by Creative-Tim
- [Django Soft PRO](https://github.com/app-generator/django-soft-ui-dashboard-pro) - `sample project`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Soft UI Dashboard PRO](https://user-images.githubusercontent.com/51070104/211132481-9a81ef68-42d4-44b3-b7e5-b700a99ef9e0.png)

<br />

## Why `Django Admin Soft PRO`

- Modern [Bootstrap 5](https://www.admin-dashboards.com/bootstrap-5-templates/) Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

Designed for those who like bold elements and beautiful websites. Made of hundred of elements, designed blocks, and fully coded pages, **Soft UI Dashboard PRO** is ready to help you create stunning websites and web apps.

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install git+https://github.com/app-generator/priv-django-admin-soft-pro.git
```

<br />

> Add `admin_soft_pro` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_soft_pro.apps.AdminSoftProConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_soft_pro` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_soft_pro.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

## Screenshots

@Todo

<br />

---
**[Django Admin Soft PRO](https://appseed.us/product/soft-ui-dashboard-pro/django/)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
