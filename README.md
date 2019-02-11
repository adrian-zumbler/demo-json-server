# Demo json Server

Inserta descripcion

## Instalacion de Herramientas

Para comenzar es necesario preparar nuestro ambiente instalando las siguientes herramientas. El proceso de instalacion asumira que se esta trabajando con ubuntu en su version 16.04.

Primero instalaremos la herramienta curl para poder realizar peticiones http por linea de comandos.

```sh
    sudo apt install curl
```

Por medio de curl descargaremos el repositorio oficial de node y lo añadiremos a Ubuntu.

```sh
    curl -sL https://deb.nodesource.com/setup_10.x | sudo bash -
```

Teniendo nuestro repositorio, procederemos a instalarlo por medio de apt

```sh
    sudo apt install nodejs
```

Verificamos que este instalando la version de node y npm

```sh
    node -v
    npm -v
```

Por ultimo instalaremos por medio de npm nuestro binario para crear el json server

```sh
    sudo npm install -g json-server
```

puedes encontrar mas informacion visitando su repositorio en el siguiente [Link](https://github.com/typicode/json-server)

**Para poder probar los endpoints se recomienda usar la herramienta Postman y la puedes instalar desde el siguiente [Link](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=es)**

## Ejecutar el servidor

Para iniciar el json server es nesesario ejecutar el siguiente comando en tu linea de comandos

```sh
    json-server --watch db.json --routes routes.json
```

Dirigite a tu navegador a la siguiente ruta **http:localhost:3000**