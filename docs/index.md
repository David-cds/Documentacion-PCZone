# 🖥️ PCZone - Catálogo e Inventario de Componentes

Bienvenido a la documentación técnica de **PCZone**, una aplicación web desarrollada de manera nativa en **PHP** y **MySQL** para la simulación de compras, control de stock y gestión de componentes informáticos.

Este proyecto ha sido estructurado con código limpio y maquetación web adaptada con estilos propios, buscando una integración directa entre la experiencia del usuario y la persistencia de datos en el servidor.

## 📊 Arquitectura General del Proyecto

La estructura interna del software está compuesta por:
* **Frontend:** Vistas dinámicas generadas mediante PHP estructurado, maquetación HTML5 y hojas de estilos CSS personalizadas.
* **Backend:** Controladores en PHP nativo para la gestión de variables de sesión, validaciones de seguridad de formularios y lógica de negocio.
* **Base de Datos:** Motor relacional MySQL para la persistencia del catálogo de productos, registro de transacciones y estados del inventario.
* **Generación de Reportes:** Integración de la biblioteca `fpdf186` para la salida de datos e impresión de comprobantes en formato PDF.
