# 🖥️ PCZone - Portal de Componentes Informáticos

Bienvenido a la documentación técnica de **PCZone**, una aplicación web orientada al comercio electrónico, catálogo y gestión de hardware y periféricos informáticos. El proyecto ha sido desarrollado de forma nativa en **PHP** y **MySQL**, prescindiendo de frameworks externos para demostrar solidez en la programación estructurada y maquetación web.

La plataforma permite a los usuarios registrarse, buscar componentes por categorías, añadir artículos a un carrito en tiempo real, realizar pedidos simulados con persistencia en base de datos y obtener facturas automáticas en formato PDF.

## 📊 Arquitectura General del Proyecto

La aplicación se estructura en cuatro capas principales:
1. **Frontend:** Vistas dinámicas generadas mediante PHP estructurado, maquetación HTML5 y hojas de estilos CSS personalizadas.
2. **Backend:** Controladores en PHP nativo para la gestión de variables de sesión, validaciones de formularios y procesamiento de la lógica de negocio.
3. **Persistencia (Base de Datos):** Base de datos relacional MySQL encargada del almacenamiento de usuarios, roles, reseñas, categorías, productos y el histórico de transacciones.
4. **Reportes:** Integración de la biblioteca `FPDF` para la exportación de comprobantes de compra.

---
> 💡 *Utilice el menú de la izquierda para navegar de forma estructurada por los requisitos de instalación, el diseño de la base de datos y los detalles técnicos del código fuente.*
