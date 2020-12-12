# Ensayo examen backend

Este proyecto fue construido con el template del curso (ya visto por ustedes en el proyecto) y expone una API REST de prueba.

## Pre-requisitos para correr proyecto:
* PostgreSQL
  * Crear una base de datos en PostgreSQL con un nombre (ejemplo, `examen_dev`) y asignarle un user/password válido
  * Configurar base de datos con nombre y user/password dentro de `src/config/database.js`. Se pueden usar variables de ambiente o modificar directamente el archivo (si les parece más simple)
  * En caso de utilizar variables de ambiente, especificar tres:
    * `DB_NAME`
    * `DB_USERNAME`
    * `DB_PASSWORD`
* Node.js LTS (ojalá 12.x, pero también puede ser 10.x)
* [Yarn](https://yarnpkg.com)

## Setup proyecto

* Clonar repositorio
* (Opcional) Si usan `nvm`, cambiar a versión válida para el proyecto
  * `nvm use`
* Instalar dependencias:
  * `yarn install`
* Correr migraciones
  * `yarn sequelize db:migrate`

## Ejecutar aplicación

```sh
yarn dev # o yarn start
```

## Probar endpoint

Para verificar que todo está bien:
- Ingresar (por browser, curl, Postman o similar) al endpoint: http://localhost:3000/api
- El resultado debiese ser un JSON con la siguiente estructura
  ```json
  {
    "message": "Bienvenido a la API del examen del curso IIC2513",
    "usersCount": 0
  }
  ```

¡Listo! Ya estás de condiciones de correr una API con el template del curso. En el examen tendrás que seguir pasos similares, pero con otro repositorio.
