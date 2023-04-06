# Django y Docker

## Pasos/comandos

- 1 Para crear el proyecto ejecuto el comando
```
django-admin startproject primer_proyecto_django
```

- 2 Se puede levantar el server con
```
python manage.py runserver
```
y acceder a http://127.0.0.1:8000/
Pero con lo hecho hasta acá solo muestra la bienvenida.

- 3 Crear las aplicaciones/funcionalidades/estructuras predefinidas por el framework, estas están definidas en el archivo settings.py en INSTALLED_APPS, las cuales son admin, auth, contenttypes, sessions, messages y staticfiles.
Para crearlas ejecuto 
```
python manage.py migrate
```

- 4 Crear el usuario admin (nos va a pedir username, mail y password). Solo se puede hacer habíendo hecho el punto 3. Para crear el usuario admin ejecuto
```
python manage.py createsuperuser
```

- 5 Logueo (luego de hacer lo del punto 4), levanto el server con
```
python manage.py runserver
```
y accedo a http://127.0.0.1:8000/admin/login/
