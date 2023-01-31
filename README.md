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

![Soft UI Dashboard PRO - Premium Django Starter](https://user-images.githubusercontent.com/51070104/215729645-658632c1-1eec-4abc-baaa-f1d3deca29ad.png)

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

## How to Customize 

When a template file is loaded in the controller, `Django` scans all template directories starting from the ones defined by the user, and returns the first match or an error in case the template is not found. 
The  theme used to style this starter provides the following files: 

```bash
< LIBRARY_ROOT >                      # This exists in ENV: LIB/admin_soft_pro
   |
   |-- templates/                     # Root Templates Folder 
   |    |          
   |    |-- accounts/       
   |    |    |-- signin/basic.html    # Sign IN Page
   |    |    |-- signup/basic.html    # Sign UP Page
   |    |
   |    |-- includes/       
   |    |    |-- footer.html          # Footer component
   |    |    |-- sidebar.html         # Sidebar component
   |    |    |-- navigation.html      # Navigation Bar
   |    |    |-- scripts.html         # Scripts Component
   |    |
   |    |-- layouts/       
   |    |    |-- base.html            # Masterpage
   |    |    |-- base-fullscreen.html # Masterpage for Auth Pages
   |    |
   |    |-- pages/       
   |         |-- widgets.html         # Widgets page
   |         |-- messages.html        # Messaging APP Page
   |         |-- *.html               # All other pages
   |    
   |-- ************************************************************************
```

When the project requires customization, we need to copy the original file that needs an update (from the virtual environment) and place it in the template folder using the same path. 

For instance, if we want to customize the `footer.html` these are the steps:

- `Step 1`: create the `templates` DIRECTORY inside your app 
- `Step 2`: configure the project to use this new template directory
  - Edit `settings.py` TEMPLATES section 
- `Step 3`: copy the `footer.html` from the original location (inside your ENV) and save it to the `YOUR_APP/templates` DIR
  - Source PATH: `<YOUR_ENV>/LIB/admin_soft_pro/includes/footer.html`
  - Destination PATH: `YOUR_APP/templates/includes/footer.html`
- Edit the footer (Destination PATH)    

At this point, the default version of the `footer.html` shipped in the library is ignored by Django.

In a similar way, all other files and components can be customized easily.

<br />

## Screenshots

![Django Admin Soft PRO - Main dashboard page, dark-mode ready.](https://user-images.githubusercontent.com/51070104/211251678-0ff9390a-2035-4cb3-b07d-62fa23f908d3.jpg)

<br />

> [Django Admin Soft PRO](https://appseed.us/product/soft-ui-dashboard-pro/django/) - `Automotive Page`

![Django Admin Soft PRO - Automotive page, premium starter by AppSeed & Creative-Tim.](https://user-images.githubusercontent.com/51070104/211251777-1ea7e1d4-b451-48c5-ad3a-164c58b1700c.jpg)

<br />

> [Django Admin Soft PRO](https://appseed.us/product/soft-ui-dashboard-pro/django/) - `Calendar Page`

![Django Admin Soft PRO - Calendar page, premium starter by AppSeed & Creative-Tim](https://user-images.githubusercontent.com/51070104/211251881-748489f7-a6e8-487f-9bd5-c721cc678c88.jpg)

<br />

---
**[Django Admin Soft PRO](https://appseed.us/product/soft-ui-dashboard-pro/django/)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
