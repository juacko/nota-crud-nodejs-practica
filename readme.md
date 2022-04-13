#Modulos a instalar

npm i express socket.io mongoose dotenv

    #dotenv: es una variable de entorno , no se suben a github

    #express : framework permite crear rutas de servidor / app de servidor 

    #socket.io : Modulo nos permite hacer una conexion en tiempo real con 
    el cliente, nos permite enviar evento nos permite comunicar el cliente con el servidor.

    #mongoose: Permite conectarme con la base de datos, modelarlos o guardarlos con cierta estructura que definamos en codigo.

Usar codigo de javascript para importar 
    En el json de configuracion:

    "type": "module"

Otro metodo es instalar los siguientes modulos.

npm i -D nodemon @babel/core @babel/cli @babel/node @babel/preset-env

    * (-D) dependencias de desarrollo

    #nodemon : nos permite reiniciar nuestro servidor cada vez que cambiaemos codigo

    #babel/core : modulo principal 
    #babel/cli : interactuar babel desde la consola
    #babel/node : la forma de utilizar babel con nodejs ( tambien hay para React)
    #babel/preset-env: nos sirven para que caracteristicas de Js estamos usando -env utiliza la ultima version de Js.

Por ultimo creamos el archivo de configuracion .babelrc 

    {
    "presets":["@babel/preset-env"]
    } 

y modificamos el scrip de inicio dev

    "scripts": {
    "dev": "nodemon src/index.js --exec babel-node"
     },