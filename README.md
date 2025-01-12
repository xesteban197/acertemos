
## **** comandos para ejecutar el proyecto *******
##
##  *** ejecutar migraciones y datos de prueba ***
##  php artisan migrate --seed
##  **********************************************

##  *** endpoins *********************************
##  *** crear usuarios ***
##  POST
##  http://localhost:8000/api/usuarios
##  {
##    "nombre": "Pepito Perez", // nombre deseado 
##    "correo": "pepito@example.com", //correo deseado
##    "saldo": 100.00 //valor deseado "mayor a 0"
##  }
##
##  *** actualizar usuarios ***
##  PUT
##  http://localhost:8000/api/usuarios/11
##  {
##    "nombre": "Pepito Perez Oso", //nombre a actualizar
##    "saldo": 200.00 //valor a actualizar "mayor a 0"
##  }
##
##  *** crear apuesta ***
##  POST
##  http://127.0.0.1:8000/api/apuestas
##  {
##  "usuario_id": 1, //id usuario existente
##  "evento": 1, //id evento existente
##  "valor": 100, //valor deseado "mayor a 0"
##  "cuota": 1.5 //valor cuota de apuesta
##  }
##
##  *** listar eventos *** 
##  GET
##  http://127.0.0.1:8000/api/eventos-deportivos
##
##  *** actualizar eventos ***
##  PUT
##  http://localhost:8000/apuestas/1/estado
##  {
##  "estado": "perdida" //estado a actualizar 
##  }
##
##  ***********************************************************


##  **** comando para ejecutar test ******
##  php vendor/bin/phpunit
##
##
##  *** comando para ver cobertura ******
##  php vendor/bin/phpunit --coverage-html=coverage-report
##
##  ************************************************************
