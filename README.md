# Dj-Rest-Auth
[![<iMerica>](https://circleci.com/gh/iMerica/dj-rest-auth.svg?style=svg)](https://app.circleci.com/github/iMerica/dj-rest-auth/pipelines)


Drop-in API endpoints for authentication in Django Rest Framework.  

### Requirements
- Django 2 or 3.
- Python 3

### Setup

Install package

    pip install dj-rest-auth
    
Add `dj_rest_auth` app to INSTALLED_APPS in your django settings.py:

    INSTALLED_APPS = (
        ...,
        'rest_framework',
        'rest_framework.authtoken',
        ...,
        'dj_rest_auth'
    )
    
Add URL patterns


    urlpatterns = [
        url(r'^dj-rest-auth/', include('dj_rest_auth.urls'))
    ]

