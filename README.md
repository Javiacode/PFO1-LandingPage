# Mi Portafolio Personal — PFO1

## Descripción del Proyecto

Este es el Trabajo Práctico N°1 (PFO1) correspondiente a la materia de Desarrollo Web. Se trata de una **Landing Page de Portafolio Personal** construida únicamente con HTML5 y CSS3. El sitio presenta información personal, videojuegos favoritos, películas favoritas, habilidades técnicas y un formulario de contacto, todo bajo una estética de **fantasía medieval oscura** (_dark fantasy_).

El diseño utiliza fuentes ornamentales, paleta de colores en tonos de pergamino quemado y oro antiguo, y animaciones CSS para lograr una experiencia visual memorable y coherente.

> URL de GitHub Pages: **[https://Javiacode.github.io/PFO1-LandingPage/](https://Javiacode.github.io/PFO1-LandingPage/)**

---

## Checklist - Práctica Formativa Obligatoria 1

### • Estructura del Proyecto

- [x] Archivo `index.html` ubicado en la raíz.
- [x] Carpeta `css` que contenga el archivo `styles.css`.
- [x] _(Opcional)_ Carpeta `img` para recursos gráficos.
- [x] Archivo `README.md` creado, que incluya una breve descripción del TP y este checklist.

---

### • Repositorio y Publicación

- [x] Repositorio en GitHub creado.
- [x] Proyecto subido al repositorio.
- [x] Proyecto publicado utilizando GitHub Pages.
- [x] En el `README.md` se indica la URL de GitHub Pages.

---

### • Uso de Google Fonts

- [x] Enlace a Google Fonts incluido en la sección `<head>` del HTML.
- [x] La tipografía importada se aplica en el sitio.
- [x] **¿Por qué elegiste esa fuente?**

  > Se eligieron tres fuentes complementarias: **Cinzel Decorative** para los títulos principales (evoca inscripciones romanas y medievales), **Cinzel** para subtítulos y etiquetas (más legible pero igualmente clásica), e **IM Fell English** para el cuerpo del texto (imita la tipografía de los libros impresos de los siglos XVII-XVIII, coherente con la estética de pergamino y grimorio). La combinación refuerza la narrativa visual del portafolio sin sacrificar legibilidad.

---

### • HTML

- [x] El documento inicia con la declaración `DOCTYPE` y usa el atributo `lang="es"`.
- [x] Se han incluido las metaetiquetas obligatorias: `charset` y `viewport`.
- [x] Se ha definido un título descriptivo: _"Javiacode | Grimorio Digital"_.
- [x] Se han vinculado correctamente el archivo CSS (`css/styles.css`) y el enlace a Google Fonts.

**Secciones obligatorias en `<main>`:**

- [x] Sección `#sobre-mi` con imagen (`alt` incluido) y párrafo descriptivo.
- [x] Sección `#tarjetas` con 4 tarjetas (imagen + texto), organizadas con Flexbox.
- [x] Sección `#peliculas` con 3 películas, cada una con título, imagen y descripción.
- [x] Sección `#habilidades` con tabla de tecnologías y listas de habilidades por aprender y hobbies.
- [x] Sección `#contacto` con formulario que incluye: Nombre, Apellido, Email, Teléfono y botón de submit.
- [x] Barra de navegación (`<nav>`) presente con **5 enlaces** (supera el mínimo de 3).
- [x] Se han insertado **4 comentarios explicativos** en el código HTML (en header, nav, sobre-mi, tarjetas).

---

### • CSS

- [x] Existe el archivo `styles.css` con estilos personalizados.
- [x] Se utilizan selectores basados en **clases** (`.tarjeta`, `.nav-link`, `.form-input`, etc.) e **identificadores** (`#header`, `#nav-principal`, `#sobre-mi`, etc.).
- [x] La tipografía importada desde Google Fonts se aplica correctamente en todos los elementos.

**Layout y Organización:**

- [x] Se ha organizado el layout de `#tarjetas` utilizando **Flexbox** (`display: flex; flex-wrap: wrap`).
- [x] **¿Qué ventajas encontraste al utilizar Flexbox o Grid en tu proyecto?**

  > Flexbox permitió que las tarjetas de proyectos y películas se distribuyan automáticamente en filas y se adapten al ancho disponible sin cálculos complejos. Con `flex-wrap: wrap` y `min-width` en los hijos, el layout se vuelve naturalmente responsivo: en pantallas grandes se muestran en columnas y en mobile se apilan verticalmente, sin necesidad de múltiples media queries. También se usó Flexbox en la navegación, el formulario y el footer para alinear elementos centralmente con gap uniforme.

**Estilización de Componentes:**

- [x] Se han personalizado los estilos de **tablas** (`.habilidades-tabla` con bordes, colores alternados y hover), **botones** (`.form-btn`, `.tarjeta-btn` con transiciones), **enlaces** (`.nav-link`, `.footer-link`) y **formularios** (`.form-input` con focus animado).
- [x] Se han ajustado las dimensiones de imágenes y contenedores utilizando unidades relativas: `%`, `rem`, `vh`, `clamp()`.
- [x] Se ha implementado **más de una animación o transición**:
  - Hover en tarjetas (`translateY` + `box-shadow` + `border-color`)
  - Hover en imagen de tarjeta (zoom con `scale` + cambio de `filter`)
  - Hover en botones (cambio de `background` + `transform`)
  - Animación `@keyframes pulsoDorado` en el emblema del header
  - Animación `@keyframes aparicion` (fade-in + slide-up) en cada sección al cargar
  - Underline animado en links del nav (`width` de 0 a 60%)
- [x] **¿Qué animación o transición implementaste y por qué?**

  > Se priorizó el efecto **hover en tarjetas** (`translateY(-6px)` + cambio de borde dorado) porque genera sensación de profundidad e interactividad sin distraer. Complementariamente, la animación de aparición progresiva (`aparicion`) da un primer impacto visual al cargar la página, simulando cómo un pergamino se despliega ante el lector. La animación `pulsoDorado` en el emblema del header actúa como punto focal que atrae la atención sin ser intrusivo.

---

### • Consideraciones Adicionales

- [x] El diseño es **responsivo**: usa `clamp()`, `flex-wrap`, `min-width` y `@media queries` para adaptarse a mobile, tablet y desktop.
- [x] Se aplicaron **buenas prácticas de accesibilidad**: atributo `alt` descriptivo en todas las imágenes, `aria-label` en links del footer, `id` en campos del formulario vinculados a sus `<label>`, color con contraste adecuado para el texto principal.
- [x] Se añadieron comentarios adicionales describiendo decisiones de diseño y posibles mejoras futuras en cada sección.
- [x] El proyecto fue desarrollado con asistencia de **Claude** (Anthropic) como herramienta de apoyo en la generación y revisión del código HTML, CSS y el contenido del README. Todas las decisiones de diseño, personalización y contenido fueron definidas por el autor.
