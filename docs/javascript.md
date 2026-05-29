# Documentación JavaScript

## Introducción

En el proyecto se utilizan diferentes técnicas JavaScript para mejorar la experiencia del usuario.

---

# Manipulación DOM

Se utiliza DOM para modificar dinámicamente elementos HTML.

## contacto.js

Archivo encargado de gestionar el formulario de contacto.

### Funciones desarrolladas

#### document.addEventListener()

Permite esperar a que cargue completamente el DOM.

```javascript
 document.addEventListener("DOMContentLoaded", function(){

addEventListener("submit")
Captura el envío del formulario.
  formulario.addEventListener("submit", function(e){

preventDefault()
Evita que la página se recargue.

e.preventDefault();

createElement()
Crea elementos dinámicamente.

let caja = document.createElement("div");

appendChild()
Inserta elementos en el documento.

contenedor.appendChild(caja);

reset()
Limpia el formulario automáticamente.

formulario.reset();

Slider JavaScript

Se utiliza un slider automático para mostrar imágenes destacadas.

Funcionalidades
Cambio automático
Rotación de imágenes
Responsive
AJAX

Se utiliza AJAX para cargar productos.

Objetivos
Evitar recargas completas
Mejorar rendimiento
Mejor experiencia de usuario
jQuery

Se utiliza jQuery para mostrar y ocultar productos.

Funciones utilizadas
hide()

Oculta elementos.

show()

Muestra elementos.

toggle()

Alterna visibilidad.

