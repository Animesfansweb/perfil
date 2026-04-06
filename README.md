# Mi primera página web personal

Página de perfil con **HTML** (estructura semántica) y **CSS** básico, para la asignatura de Programación Web.

## Cómo funciona la página

Al abrir `index.html` en el navegador se carga una sola página con varias zonas:

1. **Encabezado (`header`)**  
   Muestra el título de la página, el nombre del estudiante, la foto de perfil y un **menú de navegación**. Los enlaces no abren otras páginas: llevan a **anclas** dentro del mismo documento (por ejemplo `#sobre-mi`, `#contacto`). Al hacer clic, el navegador **desplaza la vista** hasta la sección correspondiente.

2. **Contenido principal (`main`)**  
   Agrupa cuatro **secciones** (`<section>`), cada una con un `id` que coincide con los enlaces del menú:
   - **Sobre mí** — texto de presentación, estudios e intereses generales.
   - **Intereses o gustos** — lista de aficiones y temas que gustan.
   - **Formación y conocimientos** — qué se está aprendiendo y qué se quiere aprender después.
   - **Contacto** — un **formulario** visible en la página.

3. **Pie (`footer`)**  
   Muestra el aviso de copyright. Es información estática.

4. **Hoja de estilos (`styles.css`)**  
   El HTML enlaza este archivo con `<link rel="stylesheet" href="styles.css" />`. El navegador aplica colores de fondo, color del texto, márgenes y el aspecto de la foto circular **después** de construir la página. Sin el CSS la estructura sigue siendo la misma, pero se vería con el estilo por defecto del navegador.

## Funcionamiento del formulario de contacto

El formulario tiene campos para **nombre**, **correo**, un motivo opcional y **mensaje**, más el botón **Enviar**.

- **Validación en el navegador:** los campos obligatorios (`required`) deben completarse; el correo debe tener formato de email. Si falta algo, el navegador avisa y no “envía” hasta que esté válido.
- **Envío:** `action="#"` y `method="post"` están como **marcadores de práctica**. En una página solo con HTML, al enviar no hay servidor que reciba los datos: la página puede recargarse o quedarse igual según el navegador. Para que el mensaje llegue a un correo o base de datos haría falta un **backend** o un servicio de formularios externos y cambiar el `action` del `<form>` a la URL que indique ese servicio.

## Contenido del repositorio

| Archivo / carpeta | Función |
|-------------------|---------|
| `index.html` | Estructura y contenido de la página. |
| `styles.css` | Apariencia básica (fondos, texto, márgenes, secciones). |
| `img/perfil.png` | Imagen usada en el encabezado. |

## Cómo probarla en tu equipo

1. Descarga o clona el proyecto y conserva la carpeta `img` junto a `index.html`.
2. Abre `index.html` con el navegador (doble clic o *Archivo → Abrir archivo*).
3. Prueba los enlaces del menú y el formulario (relleno y botón Enviar).

## Autor

Julio Martín Sánchez Alvarado — Universidad Ecotec.
