Este proyecto es una Single Page Application (SPA) desarrollada con JavaScript Vanilla y Bootstrap, que permite:

Registrar y autenticar usuarios.

Realizar operaciones CRUD sobre eventos.

Mostrar un historial de inicios de sesión.

Control de acceso para administradores.

🚀 Tecnologías utilizadas
JavaScript Vanilla (ES6 Modules)

Bootstrap 5.3

JSON Server (Fake REST API)

HTML5

📁 Estructura del proyecto
pgsql
Copiar
Editar
crud-spa-final/
├── index.html
├── db.json
└── assets/
    └── js/
        ├── routes.js
        ├── auth.js
        ├── products.js
        └── main.js
👤 Roles
Usuario administrador:


{
  "email": "johanrivera@correo.com",
  "password": "johan123",
  "role": "admin"
}
El administrador puede acceder a la vista de historial de logins (#logins).

⚙️ Instrucciones de uso
1. Instalar JSON Server (si no lo tienes)
bash
Copiar
Editar
npm install -g json-server
2. Iniciar el servidor
Desde la raíz del proyecto:

json-server --watch db.json
Por defecto corre en: http://localhost:3000

3. Abrir la aplicación
Abre index.html en el navegador. No necesita servidor web adicional, solo el json-server.

✨ Funcionalidades
Registro/Login de usuarios.

CRUD de productos vinculados al usuario autenticado.

Edición y eliminación de productos.

Historial de accesos (solo visible para administrador).

SPA basada en location.hash con enrutamiento manual.

📌 Notas
No se usan frameworks ni librerías externas aparte de Bootstrap.



