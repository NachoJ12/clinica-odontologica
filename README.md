# Clinica odontologica

Proyecto realizado en Backend I de la carrera Certified Tech Developer perteneciente a Digital House.
Cuenta con un front end realizado de manera simple pero funcional a los requerimientos del proyecto.
    
## Tecnologías utilizadas

  - Java
  - Spring Boot
  - H2 DataBase
  - HTML5
  - Bootstrap
  - Javascript
  - Postman
  

## Configuración

1. En la terminal, clonar el repositorio usando el siguiente comanando, el cual descargará el proyecto en la carpeta donde se haya ejecutado.

```
git clone https://github.com/NachoJ12/clinica-odontologica.git
```

2. Abrir y ejecutar el proyecto en su IDE. 

3. Escriba la siguiente url en su navegador
```
http://localhost:8080/login
```

Para iniciar sesión como administrador:

- Username: admin
- Password: admin


Para iniciar sesión como un usuario:
- Username: user
- Password: user


### Tests
Puede ejecutar los test unitarios que se encuentran dentro de la carpeta test.

Para poder visualizar las pruebas realizadas desde postman:
- Abra postman.
- Importe del archivo "clinica-odontologica.postman_collection.json"
- Ejecute la colección.


### Swagger
El proyecto cuenta con documentación de la API en Swagger. Una vez ejecutado, la podrá visualizar escribiendo la siguiente url en su navegador:
```
http://localhost:8080/swagger-ui/index.html
```

## Caracteristicas
### Sistema de reserva de turnos
Se desea implementar un sistema que permita administrar la reserva de turnos para una
clínica odontológica. Este debe cumplir con los siguientes requerimientos:

- Administración de datos de odontólogos: listar, agregar, modificar y eliminar
odontólogos. Registrar apellido, nombre y matrícula de los mismos.
- Administración de datos de los pacientes: listar, agregar, modificar y eliminar
pacientes. De cada uno se almacenan: nombre, apellido, domicilio, DNI y fecha de
alta.
- Registrar turno: se tiene que poder permitir asignar a un paciente un turno con
un odontólogo a una determinada fecha.
- Login: validar el ingreso al sistema mediante un login con usuario y password. Se
debe permitir a cualquier usuario logueado (ROLE_USER) registrar un turno, pero
solo a quienes tengan un rol de administración (ROLE_ADMIN) poder gestionar
odontólogos y pacientes. Un usuario podrá tener un único rol y los mismos se
ingresarán directamente en la base de datos.

### Requerimientos técnicos
La aplicación debe ser desarrollada en capas:

- Capa de entidades de negocio: son las clases Java de nuestro negocio
modelado a través del paradigma orientado a objetos.
- Capa de acceso a datos (Repository): clases encargadas de
acceder a la base de datos.
- Capa de datos (base de datos): es la base de datos del sistema
  modelado a través de un modelo entidad-relación. Uso de la BD H2 por su
  practicidad.
- Capa de negocio: clases service que se encargan de desacoplar el
acceso a datos de la vista.
- Capa de presentación: son las pantallas web desarrolladas
  utilizando el framework de Spring Boot MVC con los controladores con HTML+JavaScript+Bootstrap
  
Manejo de excepciones logueando cualquier excepción que se pueda generar y la realización de test unitarios para garantizar la calidad de los desarrollos.