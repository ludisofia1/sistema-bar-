# Bar Club — Sistema de gestión para bares y restaurantes

Aplicación full-stack para bares y restaurantes: pedidos online (retiro/delivery), reservas de mesa y panel de administración con caja, cocina y ventas en tiempo real.

## 🔗 Demo en vivo (sin backend, no requiere login real)

- **Sitio público:** https://ludisofia1.github.io/sistema-bar-/demo/index-demo.html
- **Panel admin:** https://ludisofia1.github.io/sistema-bar-/demo/panel-demo.html
  - Usuarios de prueba (cualquier contraseña): `admin@demo.com`, `cajero@demo.com`, `cocina@demo.com`, `mozo@demo.com`

> Estos son archivos autocontenidos con datos de ejemplo, pensados para que cualquiera pueda probar la app sin levantar el servidor real.

## Tecnologías

- **Frontend:** HTML, CSS y JavaScript puro (sin frameworks)
- **Backend:** Java 21 + Spring Boot, Spring Security, JPA
- **Base de datos:** MySQL
- **Tiempo real:** WebSocket / STOMP para notificaciones en vivo (pedidos, reservas, ventas)
- **Infraestructura:** Backend en Railway, frontend en Netlify, contenerizado con Docker

## Funcionalidades principales

- Carta de productos con pedidos online (retiro o delivery)
- Reservas de mesa con notificaciones en tiempo real
- Panel de administración con roles (Admin, Cajero, Cocina, Mozo)
- Gestión de caja (apertura/cierre, resumen por medio de pago)
- Historial de ventas y movimientos por jornada
- Sincronización en vivo entre múltiples dispositivos vía WebSocket

## Estructura del proyecto

- `index.html` / `panel.html` — frontend real (conectado al backend)
- `demo/` — versión de demostración autocontenida, sin backend
- `src/`, `pom.xml`, `Dockerfile` — backend Spring Boot
