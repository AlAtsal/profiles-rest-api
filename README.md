# Profiles REST API

Profiles REST API course code.

* To setup the vagrant server:
```bash
vagrant up
```

* To connect:
```bash
vagrant ssh
```
* Creating and activating/deactivating a virtual env in our server
```console
vagrant@ubuntu-bionic:/vagrant$ python -m venv ~/env
vagrant@ubuntu-bionic:/vagrant$ source ~/env/bin/activate
(env) vagrant@ubuntu-bionic:/vagrant$ deactivate

```

* To install the requirements from requirements.txt :
```console
(env) vagrant@ubuntu-bionic:/vagrant$ pip install -r requirements.txt
```

* Create the django project file (on the root folder):

```console
(env) vagrant@ubuntu-bionic:/vagrant$ django-admin.py startproject profiles_project .
```

* Create the profiles API app:

```console
(env) vagrant@ubuntu-bionic:/vagrant$ python manage.py startapp profile_api
```
* Start django development web server:
```console
(env) vagrant@ubuntu-bionic:/vagrant$  python manage.py runserver 0.0.0.0:8000
```
* And conect to http://127.0.0.1:8000/
