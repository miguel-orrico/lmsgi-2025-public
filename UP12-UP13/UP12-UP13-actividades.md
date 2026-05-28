# UD12 y UD13. Actividades: Gestores de contenido

## Descripción de las prácticas

Vamos a crear una página web en **WordPress** que tendrá los siguientes apartados:

- **Página principal** con información relevante sobre la temática elegida.
- **Blog** con al menos una entrada bien estructurada.
- **Tienda online** configurada con WooCommerce.

Antes de empezar, elige una temática para tu sitio web, por ejemplo: **educación, tecnología, moda, salud, automoción** u otra de tu interés.

### Consideraciones iniciales

Para evitar cambios en el menú de opciones y asegurarnos de que trabajamos con el **editor de bloques predeterminado de WordPress**, en un primer momento utilizaremos la plantilla predeterminada de WordPress, que en la versión actual es "Twenty Twenty-Five".

Como la web se trabajará en local, no será publicada en internet. Por lo tanto, se entregarán **capturas de pantalla completas** de los apartados a valorar. El contenido de la web (textos e imágenes) puede generarse con inteligencia artificial. A continuación, se explica cómo realizar capturas de página completa correctamente.

### Cómo hacer la captura de página completa

Hay varias formas de hacer una captura de pantalla completa, existen extensiones a este efecto. En cualquier caso siempre podemos hacerlo de manera nativa con las herramientas de desarrollo *devtools* de Chrome/Edge:

1. Abre las herramientas de desarrollo (devtools) con F12 o Control + Shift + I (Windows) o Cmd + Option + I (Mac).
2. Pulsa Ctrl + Shift + P (Windows) o Cmd + Shift + P (Mac), escribe "**Capture full size screenshot**" y presiona Enter.
3. La captura que se descargará automáticamente.

![Captura de pantalla completa con DevTools](./img/devtools-captura-completa.png)

Ten en cuenta que la captura refleja el viewport activo en ese momento, es decir, el área visible del navegador descontando el espacio que ocupan las DevTools. Para capturar la página completa, amplía la ventana del navegador, o incluso mueve el panel de DevTools antes de lanzar la captura.

---

## Rúbrica de Evaluación

A continuación, encontrarás la rúbrica de evaluación. Aunque se han propuesto varios ejercicios a lo largo del documento, solo se evaluarán los tres ejercicios que se detallan a continuación.

| Ejercicio | Criterio | Descripción | Puntos |
| --------- | -------- | ----------- | ------ |
| **Ejercicio 1:** Instalación de WordPress, creación de una entrada e instalación del plugin Yoast SEO | Creación de una entrada en WordPress | La entrada incluye título (h1), subtítulos (h2), párrafos, imagen, vídeo, enlaces, listas y código HTML personalizado. | 2 |
| | Optimización SEO con Yoast | Se ha optimizado la entrada utilizando Yoast SEO y se ha obtenido el indicador verde. | 1 |
| **Ejercicio 2:** Modificación de la página inicial (Landing Page) | Estructura, contenido y diseño | La página inicial contiene un Call to Action, una descripción clara del servicio o producto, otros contenedores destacados y está visualmente organizada de forma clara y atractiva. | 3 |
| **Ejercicio 5:** Creación de una tienda online con WooCommerce | Instalación, configuración y creación de productos | Se ha instalado y configurado correctamente WooCommerce, y se han creado al menos dos productos con nombre, descripción, precio, SKU, stock y una imagen destacada. | 2 |
| | Importación de productos desde CSV | Se han importado productos desde un archivo CSV correctamente. | 1 |
| **Entrega general** | Entrega correcta | Se han entregado capturas de pantalla completas correctamente realizadas de todos los ejercicios evaluables con los formatos y los nombres pedidos o un vídeo explicativo mostrando las pantallas y explicándolas de no más de 1 minuto (solo se entregará 1 vídeo): `ejercicio1Tunombreyapellidos.png`, `ejercicio2Tunombreyapellidos.png` y `ejercicio5Tunombreyapellidos.png` o `video.mp4` | 1 |
| **TOTAL** | | | **10** |

---

## Ejercicio 1: Instalación de WordPress, creación de una entrada e instalación del plugin YOAST SEO

### 1.1. Instalación de WordPress en local

Instala WordPress en local mediante el método que consideres:

1. [Instalar WordPress con XAMPP](https://www.eniun.com/descargar-instalar-wordpress-local/)
2. [Instalar WordPress con Docker](https://www.eniun.com/instalar-wordpress-docker-compose/)

Si te decides por la instalación en cloud, también me sirve, pero deberás mostrarme que lo has instalado desde cero sobre una máquina virtual (AWS EC2, Azure Compute, ...) y **NO** con un servicio de hosting que ya tenga WordPress preinstalado.

### 1.2. Creación de una entrada en WordPress

Crea una nueva entrada relacionada con tu temática. Puedes sacar el texto a integrar mediante la herramienta que quieras, por ejemplo, con inteligencia artificial.

1. Accede al panel de administración de WordPress y selecciona "Entradas" > "Añadir nueva".
2. Crea una entrada con un título (h1) que refleje la temática elegida para tu sitio.
3. Incluye al menos una imagen relacionada con la temática de la entrada.
4. Utiliza subtítulos (h2) para organizar el contenido de la entrada en secciones.
5. Escribe varios párrafos que describan y desarrollen el tema de la entrada.
6. Agrega un vídeo incrustado que complemente el contenido de la entrada.
7. Incluye enlaces a recursos relevantes relacionados con la temática.
8. Utiliza viñetas o listas numeradas para presentar información de manera estructurada.
9. Utiliza la opción "editar HTML" e incluye el siguiente código personalizado modificando el texto a tu gusto:

```html
<div>
  <p>💡 <strong>Consejo rápido:</strong> Usa la etiqueta
  <abbr title="HyperText Markup Language">HTML</abbr> para estructurar
  tu contenido de manera clara.</p>
</div>
```

Ejemplo creación de entrada

![Editor de WordPress: creación de entrada](./img/wp-editor-creacion-entrada.png)

![Editor de WordPress: creación de entrada (continuación)](./img/wp-editor-creacion-entrada-2.png)

### 1.3. Instalación y uso del plugin Yoast SEO

Instala y activa el plugin Yoast SEO desde la sección de Plugins en el Panel de Administración. Accede a la entrada creada en el punto anterior y en la pantalla de edición de la entrada, utiliza Yoast SEO para mejorar la optimización SEO. Utiliza la funcionalidad de análisis de contenido para mejorar la legibilidad y SEO de tu entrada y conseguir el punto verde.

![Yoast SEO: análisis de la entrada](./img/yoast-seo-analisis-entrada.png)

Lo normal es que al principio el análisis de Yoast SEO muestre varios puntos rojos o naranjas, lo importante es que vayas mejorando el contenido y la optimización hasta conseguir el punto verde.
![Yoast SEO: puntos rojos y naranjas al inicio](./img/yoast-seo-puntos-naranjas.png)

Paciencia en esta parte, tirar de inteligencia artificial para maneras para arreglar los puntos rojos o naranjas y conseguir el punto verde.

![Yoast SEO: mejora progresiva de la optimización](./img/yoast-seo-mejora-optimizacion.png)

No es preciso resolver todos los puntos rojos o naranjas, con resolver los más importantes y conseguir el punto verde es suficiente para el ejercicio. En cualquier caso, si quieres mejorar más la optimización, puedes seguir mejorando el contenido y la optimización hasta conseguir el punto verde en todos los aspectos. Lo importante es que en la vista de entradas se vea el punto verde de Yoast SEO, lo que indica que la entrada está optimizada para SEO.

![Yoast SEO: punto verde en la lista de entradas](./img/yoast-seo-lista-entradas-verde.png)

![Yoast SEO: indicador verde conseguido](./img/yoast-seo-indicador-verde.png)

### 1.4. Entrega del ejercicio 1

> **Captura de página completa en vista previa llamada `ejercicio1Tunombreyapellidos.png`**

Haz una captura de pantalla **completa** (de todo el sitio web, bien con la herramienta de captura de pantalla del navegador o con una extensión) en vista previa de la entrada creada, asegurándose de que se vea:

- Título (h1), subtítulos (h2), párrafos, imagen, vídeo, enlaces y listas.
- Código HTML personalizado con `<abbr>`.
- Sección de Yoast SEO con la optimización realizada y el indicador en verde. Despliega el Yoast SEO para que se vea la optimización.

---

## Ejercicio 2: Modificación de la página inicial (Landing Page)

**Diseña una página inicial atractiva para tu sitio web.** Puedes incluir los siguientes elementos (no es obligatorio incluirlos todos):

- **Call to Action (CTA):** un bloque que invite al visitante a realizar una acción concreta ("Registrarse", "Comprar ahora", "Suscribirse"…), acompañado de un botón bien visible.
- **Descripción del servicio o producto:** presenta claramente qué ofrece tu sitio, combinando texto e imágenes para captar la atención y comunicar el valor de tu propuesta.
- **Otros contenedores de interés:** características adicionales, testimonios de clientes, beneficios exclusivos, etc.

Si quieres, puedes inspirarte en la web de la consultora que realizaste en el proyecto intermodular de LMSGI — aunque si tienes otra idea, adelante con ella.

Importante es una **página** no una **entrada**. Para ello, puedes crear una página nueva y configurarla como página de inicio en los ajustes de lectura de WordPress.

Además, añade los siguientes elementos de CSS y JavaScript de forma correcta en WordPress, **sin insertar código dentro del contenido de la página**:

**Texto justificado (CSS) — vía CSS adicional:**

Ve a **Apariencia > Personalizar (en el tema activo) > Estilos > Los 3 puntitos > CSS adicional** y añade el siguiente código CSS:

![WordPress: acceso a CSS adicional en ajustes de estilos](./img/wp-css-adicional-ajustes.png)

```css
.wp-block-paragraph {
  text-align: justify;
}
```

Aplicando la clase CSS recién creada, haz que el texto de los párrafos de tu página inicial se justifique correctamente. Con excepción del que tenga sentido tener centrado, como el texto del Call to Action.

> [!TIP]
> Puedes crear grupos de bloques para organizar mejor el contenido y aplicar la clase CSS a todo el grupo, de esta forma se aplicará a todos los bloques de párrafo que estén dentro del grupo.

![WordPress: aplicar clase CSS a un grupo de bloques](./img/wp-bloques-clase-css-grupo.png)

Fíjate en la diferencia entre el primer y el segundo párrafo.

![Comparativa de párrafo con y sin texto justificado](./img/wp-parrafo-texto-justificado.png)

**Efecto de revelado al hacer scroll — vía WPCode:**

Instala el plugin **WPCode - Insert Headers and Footers...**. Este plugin permite añadir código CSS y JavaScript a tu sitio sin editar archivos del tema. Fíjate que una vez instalado se llamará **WPCode Lite** en su versión gratuita.

![Plugin WPCode instalado en WordPress](./img/wp-plugin-wpcode-instalado.png)

**Paso 1 — Añade la clase CSS al bloque**

En el panel lateral del bloque → "Clase CSS adicional" → escribe `reveal`

![WordPress: añadir clase CSS reveal al bloque](./img/wp-bloque-clase-css-reveal.png)

**Paso 2 — Crea un snippet CSS**

Ve a **Code Snippets → Add Snippet → Custom CSS** y añade:

![WPCode: creación de snippet CSS para el efecto reveal](./img/wpcode-snippet-css-reveal.png)

```css
.reveal {
  opacity: 0;
  transform: translateY(30px);
  transition: opacity 0.6s ease, transform 0.6s ease;
}
.reveal.visible {
  opacity: 1;
  transform: none;
}
```

**Paso 3 — Crea un snippet JavaScript**

Ve a **Code Snippets → Add Snippet → Custom JavaScript** y añade:

```js
document.addEventListener('DOMContentLoaded', function () {
  const observer = new IntersectionObserver(function (entries) {
    entries.forEach(function (entry) {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
      }
    });
  });
  document.querySelectorAll('.reveal').forEach(function (el) {
    observer.observe(el);
  });
});
```

> [!NOTE]
> El efecto de revelado requiere de ambas partes, el CSS para definir la animación y el JavaScript para añadir la clase que activa la animación cuando el elemento entra en el viewport al hacer scroll.

Asegúrate de activar ambos snippets para que el efecto funcione correctamente. El resultado será que los elementos con la clase `reveal` se mostrarán con un efecto de desvanecimiento y desplazamiento al hacer scroll, así que ¡no te olvides de añadir la clase `reveal` a los bloques que quieras que tengan este efecto!

Otra **cuestión importante** es que si quieres que el efecto del revelado sea al hacer scroll no podemos usar el truco de darle la clase `reveal` al contenedor padre, ya que sino el efecto se aplicará al contenedor padre y no a los bloques individuales, por lo que el efecto de revelado no se verá al hacer scroll, sino que se verá todo el contenido de golpe cuando el contenedor padre entre en el viewport. Por eso es importante añadir la clase `reveal` a cada bloque individual que queramos que tenga el efecto de revelado. Bastante tedioso pero el efecto es muy chulo, así que merece la pena el esfuerzo.

![WordPress: clase reveal aplicada a bloques individuales](./img/wp-bloques-clase-reveal-individual.png)

Ejemplo

![Demostración del efecto reveal al hacer scroll](./img/efecto-reveal-scroll-demo.gif)

### 2.1. Entrega del ejercicio 2

> **Captura de página completa llamada `ejercicio2Tunombreyapellidos.png`**


---

## Ejercicio 3: Creación de una tienda online con WooCommerce

Aprende a configurar una tienda online utilizando WooCommerce en WordPress.

**Instalación de WooCommerce:**

- Sigue los pasos del [tutorial para instalar WooCommerce](https://www.eniun.com/tutorial-woocommerce/) en tu sitio web de WordPress.
- Activa el plugin una vez que se haya instalado correctamente.

**Configuración inicial de WooCommerce:**

- Completa la configuración inicial utilizando el asistente proporcionado por WooCommerce.
- Establece la ubicación de tu tienda, tipos de productos, opciones de pago y envío, etc.

**Creación de productos:**

- **Crea manualmente** al menos dos productos para tu tienda utilizando WooCommerce.
  - Para cada producto, agrega nombre, descripción, precio, SKU, stock y una imagen destacada.
  - Explora las opciones avanzadas como atributos, variaciones y descuentos si lo deseas.
- **Importa productos desde un archivo CSV o TXT**
  - Descarga los CSV de muestra que proporciona WooCommerce en su carpeta `sample_products`. Los tienes también [enlace sample_products](./assets/sample_products.csv)
  - Sigue estos pasos para importar los productos:
    - En el panel de administración de WordPress, ve a **«Productos»**.
    - Haz clic en **«Importar»** (parte superior de la página).
    - Pulsa **«Elegir archivo»** y selecciona tu archivo CSV.

**Configuración de páginas WooCommerce:**

- Verifica que las páginas esenciales como "Carrito", "Finalizar compra" y "Mi cuenta" estén correctamente configuradas.
- Personaliza estas páginas si deseas añadir contenido adicional.

**Configuración de pagos y envíos:**

- Accede a la configuración de WooCommerce y establece los métodos de pago y envío que deseas ofrecer en tu tienda.
- Conecta tus cuentas de pago y configura las tarifas de envío según tus necesidades.

**Pruebas y gestión de la tienda:**

- Realiza pruebas de compra para verificar que los productos se añaden al carrito y se completan las transacciones correctamente.
- Accede a la sección de "Pedidos" en el panel de administración para gestionar tus pedidos, realizar seguimiento del inventario y ajustar configuraciones según sea necesario.

### 3.1. Entrega del ejercicio 

> **Captura de página completa de la página en la que se muestren los productos creados llamada `ejercicio5Tunombreyapellidos.png`. Se deben visualizar los productos creados manualmente y los creados mediante importación del CSV.**.

Por favor asegúrate de tomar la captura de pantalla de la página completa, tál y cómo se explicó al principio de este documento.

Un ejemplo mínimo de captura de pantalla lo tienes en la siguiente imagen: [Página de tienda con productos WooCommerce](./img/woocomerce-ejemplo.png)

---

