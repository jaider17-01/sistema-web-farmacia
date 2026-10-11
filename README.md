# Sistema Web de Farmacia

Proyecto de grado (Tecnología en Desarrollo de Sistemas Informáticos, UTS) — **en desarrollo**.

Aplicación web con arquitectura **MVC en PHP** para gestionar el inventario de una farmacia.

## Estado actual

| Funcionalidad | Estado |
|---|---|
| Inicio y cierre de sesión (contraseñas con bcrypt, protección CSRF) | Implementado |
| Panel (dashboard) | Implementado |
| Gestión de productos (listar, crear, editar) | Implementado |
| Ventas, compras y fórmulas médicas | Pendiente (el esquema incluye la tabla `ventas`, aún sin pantallas) |

## Tecnologías

PHP · MySQL · patrón MVC (router, controladores, modelos y vistas propios) · Apache (`public/.htaccess`)

## Contenido del repositorio

El código está empaquetado en `farmacia.zip`. Al descomprimirlo obtienes:

```
farmacia/
├── app/            Controllers, Core, Helpers, Models, Views
├── config/         env, errores, sesión
├── database/       schema.sql
├── public/         index.php y .htaccess (raíz web)
├── routes/         web.php
└── README.md
```

## Cómo ejecutarlo

1. Descomprime `farmacia.zip`.
2. Importa `farmacia/database/schema.sql` en MySQL (phpMyAdmin o consola).
3. Configura tu archivo `.env` con los datos de tu base de datos (`DB_HOST`, `DB_NAME`, `DB_USER`, `DB_PASS`). No subas este archivo a Git.
4. Sirve la carpeta `public/` con XAMPP o Laragon.
5. Abre `http://localhost/farmacia/public/`.

El esquema crea un usuario administrador inicial; cambia su contraseña antes de usarlo fuera de un entorno local.

## Autores

Jaider Javier Jaimes Picón y Jefferson David Aguilar Rojas.
Director: Edgar Alfonso Grimaldos Quintero.
