# test-loopback

Para descargar dependencias escribir:
```
npm install

bower install angular angular-resource angular-ui-router
```

Para iniciar el proyecto:
```
node .

```
Para exportar modelos de LoppBack a angular se puede utilizar el comando ```lb-ng```. Este comando analiza todos los modelos y genera código registrando un factory de AngularJS para cada modelo. Este factory crea un objeto tipo ngResource.$resource, el cual tiene una descripción de todos los métodos publicos de la clase. De esta manera el objeto resource resulta tener un API similar al modelo backend de loopback. 

Ejemplo de comando lb-ng

```
cd client
mkdir js
lb-ng ../server/server.js js/lb-services.js
```
