# API Rest Usuarios
Esta API permite gestionar usuarios en un sistema.

## Funcionalidad de Registro de Peticiones HTTP

Esta API incluye un sistema de registro de peticiones HTTP, que permite visualizar en la consola cada solicitud realizada al servidor.

### Implementación:
El siguiente código ha sido añadido en `app.js`:

```js
// EvoUsers - Registro de peticiones HTTP
app.use((req, res, next) => {
    console.log(`Petición: ${req.method} ${req.url}`);
    next();
});

