# 🛒 Proyecto Integrador – E-commerce Contenerizado con Docker

Este proyecto fue desarrollado como parte del Trabajo Integrador de la **Tecnicatura Universitaria en Programación**. Consiste en una aplicación e-commerce construida con Node.js, Express, MongoDB y Handlebars, contenerizada utilizando Docker.

Este proyecto es una tienda en línea para la venta de zapatillas. La aplicación utiliza diversas tecnologías y librerías para proporcionar una experiencia de usuario fluida y segura, incluyendo autenticación, compresión de datos, manejo de cookies, conexiones en tiempo real y más.

## 📦 Objetivo

Aplicar los conceptos de virtualización de aplicaciones mediante **Docker**, logrando empaquetar todo el entorno de desarrollo y ejecución en contenedores portables y reutilizables.

---



## Instalación local

1. Clonar el repositorio:

   ```bash
    git clone https://github.com/tu-usuario/nombre-del-repo.git
    cd nombre-del-repo

   ```

2. Instalar las dependencias:

````bash
  npm install

   ```

3. Configurar las variables de entorno en un archivo .env:

```env
  Copiar código
  PORT=3000
  DB_URI=your_mongodb_uri
  SESSION_SECRET=your_session_secret
  JWT_SECRET=your_jwt_secret
```


3.  Ejecución
```Para iniciar la aplicación en modo desarrollo:

```bash
  npm run dev

```Para iniciar la aplicación en modo producción:
  npm start
```

src/
│
├── config/
│   ├── passport.config.js          # Configuración de estrategias de autenticación Passport.
│   └── config.js                   # Configuración general de la aplicación.
├── helpers/
│   ├── multiply.js                 # Funciones auxiliares, como la función 'multiply'.
│   └── swagger/
│       └── swagger.js              # Configuración y setup de Swagger para la documentación de la API.
├── middleware/
│   └── errors.js                   # Middleware para el manejo de errores.
├── mongoDb/
│   └── connection/
│       └── mongooseConnection.js   # Configuración y conexión a la base de datos MongoDB.
├── public/
│   └── (archivos estáticos como CSS, JavaScript, imágenes)
├── routes/
│   └── routes.js                  # Definición de rutas de la aplicación.
├── socket/
│   └── socket.io.js               # Configuración de Socket.io para comunicación en tiempo real.
├── utils/
│   └── logger.js                  # Configuración de Winston para el registro de logs.
└── views/
    └── (plantillas Handlebars para vistas dinámicas)


Descripción de los Archivos Principales
app.js: Archivo principal que configura y arranca el servidor.
mongooseConnection.js: Configuración y conexión a la base de datos MongoDB.
passport.config.js: Configuración de estrategias de autenticación.
routes.js: Definición de rutas de la aplicación.
socket.io.js: Configuración de Socket.io para comunicación en tiempo real.
swagger.js: Configuración y setup de Swagger para la documentación de la API.
logger.js: Configuración de Winston para el registro de logs.
errors.js: Middleware para el manejo de errores.
Funcionalidades Clave
Autenticación: Utiliza Passport.js con estrategias locales y de terceros (GitHub).
Compresión: Middleware para comprimir las respuestas HTTP.
Manejo de Errores: Middleware centralizado para el manejo de errores.
Documentación de API: Swagger para documentar y probar la API.
Subida de Archivos: Utiliza Multer para gestionar la subida de archivos.
Pagos: Integración con MercadoPago para procesar pagos.
Vistas Dinámicas: Utiliza Handlebars para generar vistas dinámicas.
Logs: Utiliza Winston para el registro de eventos y errores.
Notificaciones: Utiliza SweetAlert2 para mostrar notificaciones al usuario.

````


