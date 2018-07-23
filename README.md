ESTRUCTURA DEL PROYECTO
=======================
**raml-editor**
```sh
├── template/
├── assets/
├── raml-files/  
│   └── proyecto/
│       ├── assets/
│       ├── samples/
│       └── index.raml
├── bs-config.json
├── gulpfile.js
├── package.json
└── README.md
```

* **templates** contiene el esquema de la interfaz de documentación
* **assets** contiene los estilos de los templates de documentación
* **raml-files** contiene el archivo RAML con las rutas y métodos que soporta el API
* **raml-files/proyecto/assets** contiene estilos particulares para los RAML del API
* **raml-files/samples/samples** contiene ejemplos en formato JSON a importarse en los archivos RAML
* **raml-files/proyecto/assets** contiene estilos particulares para los RAML del API
* **bs-config.json, gulpfile.js y package.json** archivos de configuración del proyecto

GUIA DE USO
===========
```sh
# Instalar las dependencias del proyecto
$ npm install
# Construir html en base a estructura RAML y servir web
$ gulp --path raml-files/proyecto/index.raml
# Servir proyecto ya construído
$ npm run serve
```
