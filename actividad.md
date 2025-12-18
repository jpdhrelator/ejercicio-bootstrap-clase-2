# 🚀 Desafío Práctico: "El Lanzamiento del Producto Revolucionario"


**Tecnologías:** HTML5, Bootstrap 4 CSS, Bootstrap 4 JS (jQuery)

---

## 📝 Contexto y Misión

Imagina que eres el desarrollador web principal de una *startup* tecnológica (o mágica, o futurista). Tu empresa está a punto de lanzar un producto que cambiará el mundo.

**Tu misión:** Crear una "One Page" (página única) para presentar este producto.

**El Producto:** ¡Tú decides! Puede ser una patineta voladora, una poción de invisibilidad, una app para hablar con gatos o un robot de cocina nuclear. **Sé creativo con la temática.**

---

## ⚙️ Requisitos Técnicos Obligatorios

Para el desafío, tu página debe integrar funcionalmente los siguientes componentes JavaScript de Bootstrap 4. No basta con copiar el HTML, debes asegurarte de que la interactividad funcione.

1.  **Navegación Dinámica:** Navbar con Dropdowns.
2.  **Showcase Visual:** Carrusel de imágenes.
3.  **Gestión de Espacio:** Acordeón (Collapse) para preguntas frecuentes.
4.  **Micro-interacciones:** Tooltips y Popovers inicializados vía JS.
5.  **Flujos de Usuario:** Modal para "comprar/reservar" y Alertas dinámicas.

---

## ⏱️ Cronograma de Trabajo

### Fase 1: Estructura y Navegación
1.  Crea tu archivo `index.html` y conecta las librerías de Bootstrap 4 (CSS y los scripts JS/jQuery en el orden correcto).
2.  Diseña una **Barra de Navegación** (`.navbar`) que se quede fija en la parte superior (`fixed-top`).
3.  **Requisito JS:** La barra debe incluir un menú desplegable (`.dropdown`) en la sección de "Características" que muestre al menos 3 sub-opciones.

### Fase 2: La Galería del Producto 
1.  En el encabezado (Header), implementa un **Carrusel** (`.carousel`) que ocupe un ancho considerable.
2.  Debe tener al menos 3 diapositivas (`slides`) mostrando tu producto.
3.  **Requisito JS:** Configura mediante atributos `data-` o JavaScript que el carrusel pase las imágenes automáticamente cada 3 segundos.

### Fase 3: Detalles y Secretos 
1.  Crea una sección de "Especificaciones Técnicas" usando el sistema de grillas (Cards o Columnas).
2.  **Requisito JS (Tooltips):** Algunos términos técnicos (ej: "Motor de iones", "Sabor a fresa", "IA integrada") deben tener un **Tooltip** que explique qué es al pasar el mouse.
    * *Recuerda:* Los tooltips deben inicializarse manualmente en tu script.
3.  **Requisito JS (Popovers):** Añade un botón que diga "Ver condiciones de garantía" o "Letra chica". Al hacer clic, debe salir un **Popover** con información extra.

### Fase 4: Preguntas Frecuentes (FAQ) 
1.  Diseña una sección de "Preguntas Frecuentes" al final de la página.
2.  **Requisito JS:** Utiliza el componente **Accordion** (basado en `.collapse`).
3.  Debe haber al menos 3 preguntas. Al abrir una pregunta, las otras deben cerrarse automáticamente.

### Fase 5: El Gran Final  - ¡Atención aquí! 🧠
Esta es la parte de mayor lógica.
1.  Crea un botón grande y llamativo que diga **"RESERVAR AHORA"**.
2.  **Requisito JS (Modal):** Al hacer clic, debe abrirse una ventana **Modal** con un formulario simple (Nombre y Correo).
3.  Dentro del Modal, el botón de "Confirmar" **NO** debe recargar la página.
4.  **Requisito JS (Evento + Alerta):**
    * Programar en JavaScript/jQuery que, al hacer clic en "Confirmar" dentro del modal:
        1.  Se cierre el modal (`.modal('hide')`).
        2.  Aparezca una **Alerta** (`.alert`) de éxito en la parte superior de la página diciendo "¡Gracias por tu reserva!".
        3.  La alerta debe poder cerrarse haciendo clic en su "X".

---

### 💡 Pistas

* Recuerda que `Tooltips` y `Popovers` **NO** funcionan si no agregas el código de inicialización en tu `<script>`:
    ```javascript
    $(function () {
      $('[data-toggle="tooltip"]').tooltip()
    })
    ```
* Para conectar el Modal con la Alerta, necesitarás usar un ID en tu botón de confirmar y escuchar el evento `click`.
* ¡Revisa la consola del navegador (F12) si algo no funciona!

¡Buena suerte, desarrolladores! 🚀