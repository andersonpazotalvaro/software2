# ARQUITECTURA DE REFERENCIA

Smart Parking Lot es un proyecto que se desarrollara a partir de una arquitectura de referencia web.
![MapaEmp](/assets/images/ArquitecturadeReferencia.PNG)

- 1- El front end es la parte con la que el usuario interactúa y es la primera capa con la que el usuario tiene contacto

- 2- El api Gateway es el encargado de centralizar el llamado desde el front end para que entren por un mismo lugar, para posteriormente tomar la decisión si redirige el llamado a una base transicional o de consulta, ayuda a tener puertas de enlace seguras, así como la monitorización del mismo

- 3- El back end se divide en 2, transicional y de consulta, esto es debido a que algunos llamados solo son de lectura y otros de lectura y escritura

- 4- Baúl de secretos es el que guarda las contraseñas en la nube

- 5- Fuentes de información, esta al igual que el back end esta dividida en 2 ya que hay información que no es transicional, de forma que no puede ser editada o eliminada

- 6- Mecanismo de integración ETL , su principal propósito es que haya cohesión de datos, se utiliza mayormente cuando se mezclan datos de múltiples fuentes  

- 7- Identity provider es un servicio  especializado en dar seguridad y manejar niveles de acceso así como la autentificacion de usuarios
![MapaEmp](/assets/images/ArquitecturadeReferencia2.PNG)
