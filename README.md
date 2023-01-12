# **Desafío: MEJORAR LA ARQUITECTURA DE NUESTRA API**. Curso CoderHouse Backend Node.Js

## Consignas:

* Modificar la capa de persistencia incorporando los conceptos de Factory, DAO, y DTO.
* Los DAOs deben presentar la misma interfaz hacia la lógica de negocio de nuestro servidor.
* El DAO seleccionado (por un parámetro en línea de comandos como lo hicimos anteriormente) será devuelto por una Factory para que la capa de negocio opere con el.
* Cada uno de estos casos de persistencia, deberán ser implementados usando el patrón singleton que impida crear nuevas instancias de estos mecanismos de acceso a los datos.
* Comprobar que si llamo a la factory dos veces, con una misma opción elegida, devuelva la misma instancia.
* Implementar el patrón Repository para la persistencia de productos y mensajes.

## Como ejecutar el proyecto de manera local:

* Ejecutar el comando `npm install`
* Se debe crear un archivo de configuraracion `.env` con los siguientes datos

```
MONGO_USER = "<usuario Mongo Atlas>"
MONGO_PASS = "<contraseña Mongo Atlas>"
MONGO_CLUSTER = "<@clusterx.asd123.mongodb.net/test>"
GOOGLE_APLICATION_CREDENTIALS = "<google credentials>"
PUERTO = 8080

ACCOUNT_SID = ""
AUTH_TOKEN = ""
NRO_WSP = "<número whatsapp aporbado para recibir mensajes>"
NRO_TWILIO = "<número de twilio>"

TEST_MAIL = "<cuenta de correo gmail>"
TEST_MAIL_PASS = "<contraseña correo prueba>"
```

* Ejecutar el comando `npm run start` o ` npm run start -- --puerto <n° de puerto>`
* Para probar/testear los diferentes rutas y funcionalidades, se recomienda utilizar [Postman](https://www.postman.com/downloads/)´
