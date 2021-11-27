# Ejercicio grupal

- Crea un proyecto en node. El nombre debe llamarse grupal_2, descripción el nombre de los integrantes y en autor ponga a un integrante del equipo.
- Instala en tu proyecto de node, el paquete brower sync. Recuerda que al instalar el paquete debe estar en las dependencias de desarrollo
- Crea un archivo index.js y agrega la configuración del browser sync.
```
var browserSync = require("browser-sync").create();

browserSync.init({
    watch: true,
    server: "./app"
});
```
- Debes configurar tu index.js para cuando ejecutes npm start.
- Crea una carpeta app y en su interior debes crear un archivo index.html. Debes agregar bootstrap y un archivo style.css donde agregaras tu propio css
- Agrega un select en tu index.html. Usa la clase de bootstrap para darle estilo.
- Dale al contenedor un 80% de ancho y centra los campos
- Debes crear un nuevo archivo js dentro de la carpeta app con el nombre request.js y en su interior deberas utilizar el método fetch para realizar una solicitud a un servidor.

La url que debes agregar al fetch es https://jsonplaceholder.typicode.com/users
- Una vez obtenido los datos, debes agregar esta información al select por medio de javascript.
- Ya que se muestran los datos en el select, ahora cada vez que el usuario seleccione una opción, deberas recuperar el id del valor seleccionado y deberas hacer una nueva peticiín usando fetch pasando el id seleccionado. 

Ejemplo
https://jsonplaceholder.typicode.com/users/{ID}
```
fetch('https://jsonplaceholder.typicode.com/users/1')
```
- Ya que obtengas la información, deberas mostrar en una card de bootstrap las propiedades name, username, email y de la propiedad address debes mostrar la propiedad street

Nota: Adicionalmente debes agregar un loader para indicar al usuario que esta cargando la información. Tambien debes agregar toastr para notificar cuando pase un error.

### Recursos 

toastr ->  ***https://github.com/CodeSeven/toastr***
loader -> ***https://loading.io/spinner/***


Una vez finalizada, deberas subir este ejercicio al repositorio

```
