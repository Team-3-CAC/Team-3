# crud-django

Correr linea de comando

`docker-compose run web django-admin startproject cruddjango .`


Ahora creamos una app que se llama encuestas

`docker-compose run web python manage.py startapp encuestas`


Cada vez que modifiquemos nuestro modelo de datos... vamos a correr el siguiente comando
Toma la información de las estructuras pre-armadas de las aplications que están instaladas
(altera el contenido de la DB pero no modifica el contenido del código fuente)

`docker-compose run web python manage.py migrate` (aplica los nuevos modelos creados con el makemigrations)

** `docker-compose run web python manage.py makemigrations` (crea el nuevo modelo de datos en un .py)

Por ultimo creamos un super usuario
(altera el contenido de la DB pero no modifica el contenido del código fuente)

`docker-compose run web python manage.py createsuperuser`

** superuser (django) creado: root (user and password)


** Para correr los tests:
`docker-compose run web python manage.py test`


## Colaboradores:

- Fernando Camino
- Mauricio Melgaejo
- Marcos Santillan  
- Paola Errazti

## Actividades:

- [x] Cada Miembro del equipo debe cambiar el archivo readme.md en la seccion de contributors (si no la tiene agregarla).

- [x] Cada miembro del equipo debe poder descargar el proyecto del repositorio y probarlo localmente.

- [x] Crear un proyecto de github.

- [x] Crear N urls con N respuestas distintas dependiendo de la cantidad de miembros del equipo.

- [x] Tienen que tener un test escrito en el archivo tests.py.

- [x] Crear un modelo Usuario (o user) crear N properties por cada N integrante del equipo. (# Fernando)

- [x] Integrar los cambios en el repositorio.