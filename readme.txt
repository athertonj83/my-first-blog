******** TUTORIAL LINK **********
I used the following link to complete this tutorial for a blog:
https://tutorial.djangogirls.org




******** VIRTUAL ENVIRONMENT **********
In order to activate the virtual environment, go to djangojen dir in cmd and type:
myvenv\Scripts\activate


In order to deactivate, type:
deactivate







******** CHANGES MADE TO DJANGO SETUP **********
Following changes needed to be made to ensure css was recognised:
in settings.py, commented out:

STATIC_URL = '/static/' 
STATIC_ROOT = os.path.join(BASE_DIR, 'static') 


in settings.py, added in:

STATIC_ROOT = ''
STATIC_URL = '/static/'
STATICFILES_DIRS = ( os.path.join('static'), )