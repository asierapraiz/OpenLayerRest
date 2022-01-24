# MapHurricane REST

## Comandos Maven

- ```mvn clean```: limpia la carpeta ```target```.
- ```mvn compile```: compila el proyecto entero y crea las clases que utiliza la libreria ```querydsl```.
- ```mvn spring-boot:run```: arranca la aplicación por terminal.
- ```mvn test```: ejecuta todas las pruebas de la aplicación.
- ```mvn package```: ejecuta todas las pruebas y si pasa, genera el fichero jar con el proyecto y el análisis de cobertura de las pruebas
- ```mvn package -Dmaven.test.skip=true```: genera el fichero jar sin pasar los test
## Instalaciones

- [Instalación PostgreSQL](doc/instalacion-postgresql/README.md)
- [Instalación QGIS](doc/instalacion-QGIS/README.md)
- [Instalación Lombok](doc/instalacion-lombok/README.md)

## Copias de seguridad

### BBDD

La copia que se encuentra en el fichero ```copia-BBDD-maphurricane.sql``` se ha realizado con el programa ```pgAdmin```
de PostgreSQL por lo que se recomienda hacer su restauración con este mismo programa ya que con DBeaver ha dado
problemas. Para la consulta de datos o modificación de las tablas se puede utilizar cualquiera de los dos. Lo único, si
se actualizan las tablas, **actualizar la copia para tener siempre la última versión.**

También hay que crear una base de datos de pruebas con el nombre ```maphurricane_test``` y restaurarla con el
fichero ```copia-BBDD-maphurricane_test.sql```
para poder realizar las pruebas sin problemas.

### Postman

Dentro de la carpeta ```Postman``` tenéis una copia de las llamadas al servicio REST para que realices las pruebas de
este.

### Ejecución por terminal

Para ejecutar la aplicación directamente en un terminal, ejecutamos el siguiente comando:

```terminal
java -jar MapHurricaneServidor-0.0.1-SNAPSHOT.jar
```


## Más documentación

Mira el fichero ```Guia MVC Spring.docx``` en el directorio ```doc```.
