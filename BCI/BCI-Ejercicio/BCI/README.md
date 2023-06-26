# Proyecto para Global Logic BCI

Proyecto Personal Banco BCI

Desarrollo de API para poder crear un usuario y loguearse con el mismo.

## Tech Stack

Java, Spring, H2 database, built using Gradle



## Installation

Para poder utilizarlo se debe clonar el proyecto y realizar las peticiones al mismo mediante Postman.


    
## Examples


Recomiendo para realizar este proceso importar desde el postman el archivo bci.postman_collection.json el cual se encuentra en el root de este mismo proyecto.


##
##

Tambien puede realizarno de forma manual utilizando este ejemplo (copiar y pegar los request en postman,detallados abajo) 
```json

localhost:8080/api/v1/sign_up
{
  "username": "global",
  "email": "global@logic.com",
  "password": "globaLLog14",
  "phones": [
    {
      "number": 54113012,
      "cityCode": 7777,
      "countryCode": "ARG"
    }
  ]
}
        
localhost:8080/api/v1/login
{
  "username": "global",
  "password": "globaLLog14"
}
```
## IMPORTANTE
Recordar agregar el JWT Token generado en nuestro sign_up cuando hagamos el login, hay un filtro de seguridad activado para esto, en el caso de que el cliente quiera podemos desactivarlo

## Used By

This project is used by the following companies:

- GlobalLogic
- BCI


## Edgardo Javier Patiño
