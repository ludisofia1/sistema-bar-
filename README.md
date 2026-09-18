# Bar Club

Sistema de gestión para bares y restaurantes. Permite hacer pedidos online (retiro o delivery), reservar mesa, y tiene un panel de administración para manejar caja, cocina y ventas.

## Probalo

No hace falta instalar nada, hay una versión demo con datos de ejemplo:

- Sitio público: https://ludisofia1.github.io/sistema-bar-/demo/index-demo.html
- Panel de administración: https://ludisofia1.github.io/sistema-bar-/demo/panel-demo.html (usuarios: admin@demo.com, cajero@demo.com, cocina@demo.com o mozo@demo.com, con cualquier contraseña)

## Cómo está hecho

Frontend en HTML, CSS y JavaScript plano, sin frameworks. Backend en Java 21 con Spring Boot, Spring Security y JPA, con MySQL como base de datos. Las notificaciones (pedidos nuevos, reservas, ventas) se actualizan en tiempo real con WebSocket. Backend desplegado en Railway y frontend en Netlify, con Docker.

## Qué hace

Pedidos online con retiro o delivery, reservas de mesa con aviso en tiempo real, panel con distintos roles (admin, cajero, cocina, mozo), manejo de caja con apertura y cierre, historial de ventas por día, y sincronización entre varios dispositivos usando el mismo panel a la vez.

## Estructura

`index.html` y `panel.html` son el frontend real, conectado al backend. La carpeta `demo/` tiene una versión de esos mismos archivos pero sin depender de ningún servidor, solo para poder probar la app sin instalar nada. El resto (`src/`, `pom.xml`, `Dockerfile`) es el backend en Spring Boot.
