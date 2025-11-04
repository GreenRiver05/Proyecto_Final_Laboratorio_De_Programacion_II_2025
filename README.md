📖 Narrativa del sistema
El sistema desarrollado corresponde a una plataforma web de ventas para un emprendimiento personal que actualmente comercializa productos a través de redes sociales como Instagram y WhatsApp. El objetivo principal es digitalizar el proceso de compra y gestión de productos, ofreciendo una experiencia más profesional, organizada y accesible tanto para los clientes como para el equipo del negocio.

🧩 Entidades principales
Usuario: Persona que accede al sistema. Puede ser cliente, empleado o administrador. Cada usuario tiene email, contraseña, avatar y datos personales.
Producto: Artículo disponible para la venta. Incluye nombre, descripción, precio, imagen, categoría y estado.
Categoría: Agrupación de productos por tipo o uso. Permite organizar el catálogo.
Pedido: Representa una compra realizada por un cliente. Incluye productos, cantidades, fecha, estado y total.
DetallePedido: Relación entre pedido y productos, con cantidad y precio unitario.
Consulta: Mensaje enviado por un visitante o cliente con dudas sobre productos o el negocio.

🔐 Roles y permisos
Administrador: Puede gestionar usuarios, productos, categorías, pedidos y eliminar entidades. Tiene acceso a vistas de auditoría.
Empleado: Puede agregar productos, ver pedidos, responder consultas y modificar su perfil.
Cliente: Puede registrarse, iniciar sesión, editar su perfil, agregar productos al carrito y realizar pedidos.

⚙️ Funcionalidades clave
Para visitantes (sin login):
Navegar productos por categoría
Buscar productos por nombre o palabra clave
Filtrar por precio, categoría o disponibilidad
Ver detalles del producto
Enviar consultas desde la sección de contacto

Para clientes registrados:
Crear cuenta y editar perfil (incluye avatar)
Agregar/quitar productos del carrito
Ver el contenido del carrito
Realizar pedido (requiere login)
Ver historial de pedidos

Para empleados y administradores:
ABM de productos (con imagen)
ABM de categorías
ABM de promociones y noticias
Ver y gestionar pedidos
Ver y responder consultas
Ver qué usuario creó cada pedido (auditoría)

📊 Informes y listados
Listar todos los productos activos, con filtros por categoría y precio
Listar productos por categoría específica
Listar pedidos realizados por un cliente
Listar pedidos por estado (pendiente, enviado, cancelado)
Listar consultas recibidas con fecha y estado (respondida/no respondida)
Listar productos con stock bajo (ej. menos de 5 unidades)

📑Requisitos técnicos
Login con roles y uso de [Authorize]
Avatar en perfil de usuario
ABM de productos hecho con Vue.js y AJAX
Paginado en listados de productos y pedidos
Búsqueda de productos vía AJAX (no traer todos)
API con JWT para pedidos o productos (ej. para integración futura con app móvil)
Subida de imágenes para productos y avatar
Auditoría: registrar qué usuario creó/modificó cada pedido o producto (visible solo para admins)
