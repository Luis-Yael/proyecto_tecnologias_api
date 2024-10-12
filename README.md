PIK - API
====================

## Requerimientos

* Python 3.5+
* Pip 3  

- - -

## Ambientación

1. Install Python 3.5+

2. Install Pip 3

3. Install virtualenv  
Se usa para crear ambientes virtuales y ejecutar la versión de Python requerida

4. Clonar el proyecto  

5. Activar el ambiente virtual  
$ source env/bin/activate
  Windows:
C:/path_to_the_folder/> env/Project_name/Scripts/activate.bat

6. Instalar las librerías requeridas por el proyecto  
$ pip3 install -r requirements.txt

7. Configurar conexión a base de datos (MySQL)  
/sistema_buap_api/my.cnf

8. Crear la base de datos y aplicar las migraciones  
$ python3 manage.py makemigrations sistema_buap_api  
$ python3 manage.py migrate  


9. Cargar todos los fixtures en el orden en que están numerados. Ejemplo:  
$ ./manage.py loaddata fixtures/1initial_data.json
$ ./manage.py loaddata fixtures/2authgroup.json
$ ./manage.py loaddata fixtures/3user.json
etc..

10. Crear un django administrator (IMPORTANTE)  
$ python3 manage.py createsuperuser --email admin@admin.com --username admin  
(Console input) PASSWORD: XXXXXX

11. Correr el servidor  
 python3 manage.py runserver  

IMPORTANT: Initial data, requiered for the project. Run once the database was created.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  -

## API Contract (postman)

https://www.getpostman.com/collections/######################

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  -