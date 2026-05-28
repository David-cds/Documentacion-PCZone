# 🗄️ Base de Datos

El sistema utiliza **MySQL** para gestionar la información de la tienda. La estructura consta de las siguientes tablas:

### 📦 Tabla `productos`
Guarda el catálogo y el inventario disponible.
* **`id`**: Identificador único del producto.
* **`nombre`**: Nombre del componente de hardware.
* **`descripcion`**: Detalles técnicos.
* **`precio`**: Precio unitario.
* **`stock`**: Unidades disponibles (campo que disminuye al comprar).
* **`imagen`**: Ruta de la imagen del producto.
* **`destacado`**: Controla si se muestra en la portada.

### 👥 Tabla `usuarios`
Gestiona las cuentas y accesos al sistema.
* **`id`**: Identificador único del usuario.
* **`nombre`**: Nombre del cliente.
* **`email`**: Correo electrónico de acceso.
* **`password`**: Contraseña de seguridad.
* **`rol`**: Tipo de usuario (Cliente / Administrador).

### 🛒 Tabla `pedidos` (Cabecera)
Registra los datos generales de cada compra realizada.
* **`id`**: Identificador único del pedido.
* **`id_usuario`**: Quién realizó la compra (relacionado con `usuarios`).
* **`fecha`**: Día y hora de la transacción.
* **`total`**: Importe total facturado.

### 📋 Tabla `detalles_pedido`
Guarda el desglose de los productos dentro de cada pedido (necesario para FPDF).
* **`id`**: Identificador del registro.
* **`id_pedido`**: Al qué pedido pertenece (relacionado con `pedidos`).
* **`id_producto`**: Qué producto compró (relacionado con `productos`).
* **`cantidad`**: Cuántas unidades compró de ese artículo.
* **`precio_unitario`**: El precio del producto en el momento de la compra.

---

## 🔄 Lógica de Actualización de Stock
Al confirmar un pedido, el sistema realiza dos acciones clave:
1. Registra la información en las tablas `pedidos` y `detalles_pedido`.
2. Ejecuta un `UPDATE` en la tabla `productos` restando la `cantidad` comprada al campo `stock` según el `id` del componente, asegurando que las existencias bajen al instante.
