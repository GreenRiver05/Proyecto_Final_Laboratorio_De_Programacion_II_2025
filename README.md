### 📄 Presentación del proyecto

[📂 Ver presentación en Google Drive](https://docs.google.com/document/d/1q6TZyCuTYKILoUcFNR_0_dcI8NxfvsNRRzU2FIbEa-A/edit?usp=sharing)

# 🛍️ Plataforma Web de Ventas para Emprendimiento Personal

Este proyecto corresponde a una **plataforma web de ventas** desarrollada para digitalizar y profesionalizar un emprendimiento que actualmente comercializa productos a través de redes sociales como **Instagram** y **WhatsApp**. El sistema permite gestionar productos, pedidos y consultas, brindando una experiencia más organizada y accesible tanto para los clientes como para el equipo del negocio.

---

## 🚀 Objetivos del sistema

- Digitalizar el proceso de compra y gestión de productos.
- Mejorar la experiencia del cliente con una interfaz clara y moderna.
- Optimizar la administración del catálogo, pedidos y consultas.
- Preparar la base para futuras integraciones móviles mediante API.

---

## 🧩 Entidades principales

| Entidad         | Descripción funcional |
|-----------------|-----------------------|
| **Usuario**      | Persona que accede al sistema. Puede tener rol de cliente, empleado o administrador. Gestiona su perfil y participa en acciones según permisos. |
| **Cliente**      | Usuario que realiza compras. Tiene historial de pedidos, puede enviar consultas y actualizar sus datos personales. |
| **Producto**     | Artículo disponible para la venta. Incluye información comercial, estado de disponibilidad y stock. |
| **Categoría**    | Agrupación lógica de productos por tipo o uso. Facilita la navegación y organización del catálogo. |
| **Pedido**       | Transacción de compra realizada por un cliente. Registra fecha, estado, total y productos involucrados. |
| **DetallePedido**| Componentes individuales de un pedido. Relaciona productos con cantidades y precios unitarios. |
| **Consulta**     | Mensaje enviado por un cliente con dudas o comentarios. Puede ser respondido por el equipo del negocio. |
| **Auditoría**    | Registro de acciones realizadas por usuarios sobre entidades del sistema. Visible solo para administradores. |

#### Diagrama de Clases
![Diagrama de Clases](docs/diagramas/DiagramaDeClases.jpg)

---

## 🔐 Roles y permisos

| Rol             | Permisos principales |
|-----------------|----------------------|
| **Administrador** | Realiza todas las acciones disponibles para el rol de Empleado y además puede gestionar usuarios, eliminar entidades y acceder a vistas de auditoría. |
| **Empleado**      | Inicia sesión, agrega y modifica productos, responde consultas de clientes, administra promociones y descuentos, visualiza pedidos y edita su propio perfil. |
| **Cliente**       | Se registra e inicia sesión, edita su perfil y avatar, navega y filtra productos, visualiza detalles, agrega o quita productos del carrito, realiza pedidos, consulta su historial y envía consultas al negocio. |


#### Diagrama de Casos de Uso
![Diagrama de Casos de Uso](docs/diagramas/CasosDeUso.jpg)

---

## ⚙️ Funcionalidades clave

### Para visitantes (sin login)
- 🔍 Navegar productos por categoría
- 🧠 Buscar por nombre o palabra clave
- 🎯 Filtrar por precio, categoría o disponibilidad
- 📄 Ver detalles del producto
- ✉️ Enviar consultas desde la sección de contacto

### Para clientes registrados
- 👤 Crear cuenta y editar perfil (incluye avatar)
- 🛒 Agregar/quitar productos del carrito
- 📦 Ver el contenido del carrito y realizar pedidos
- 📜 Consultar historial de compras

### Para empleados y administradores
- 🧰 ABM de productos, categorías, promociones y noticias
- 📬 Ver y responder consultas
- 📊 Gestionar pedidos y ver auditoría de acciones

---

## 📊 Informes y listados

- Listar productos activos con filtros por categoría y precio
- Listar productos por categoría específica
- Listar pedidos por cliente o por estado (pendiente, enviado, cancelado)
- Listar consultas con fecha y estado (respondida/no respondida)
- Listar productos con stock bajo (menos de 5 unidades)

---

## 🧪 Requisitos técnicos

- 🔐 Login con roles y uso de `[Authorize]`
- 🖼️ Subida de imágenes para productos y avatar
- ⚙️ ABM de productos con **Vue.js** y **AJAX**
- 🔎 Búsqueda de productos vía AJAX (sin traer todos)
- 📄 Paginado en listados de productos y pedidos
- 🔐 API con **JWT** para pedidos y productos (pensado para integración móvil)
- 🕵️ Auditoría de acciones (registro de usuario que crea/modifica pedidos o productos)

---


### 🧪 Prototipos y diseño visual

#### Wireframes y prototipos en Figma
[🔗Figma – Proyecto de interfaz](https://www.figma.com/design/AbqPECEezeyW8UD9lFEL7M/Sin-t%C3%ADtulo?node-id=79-3478&t=nA7LzktQpI77TqAD-1)
