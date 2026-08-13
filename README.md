# 👩‍🎓 Portfolio — Omar Virili

Sitio personal desarrollado con HTML5 y CSS3 (vanilla), sin frameworks ni build tools, presentando mi perfil, formación académica, stack tecnológico y proyectos realizados durante mi formación como desarrollador.

**🔗 Demo publicada:** [porfolio-oceano.vercel.app](https://porfolio-oceano.vercel.app/)
**📂 Repositorio:** [github.com/odv144/curriculum](https://github.com/odv144/curriculum)

---

## 📌 Contenido

- [Sobre el proyecto](#sobre-el-proyecto)
- [Tecnologías](#tecnologías)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Cómo ejecutarlo localmente](#cómo-ejecutarlo-localmente)
- [Secciones del sitio](#secciones-del-sitio)
- [Accesibilidad](#accesibilidad)
- [Declaración sobre el uso de IA](#declaración-sobre-el-uso-de-ia)
- [Contacto](#contacto)

---

## Sobre el proyecto

Landing page de presentación profesional pensada para acompañar mi búsqueda laboral como desarrollador. Incluye mi perfil, habilidades técnicas (front-end, back-end y herramientas), formación académica, proyectos realizados en cursos y simulaciones laborales, y un formulario de contacto.

## Tecnologías

- **HTML5** semántico (`header`, `nav`, `main`, `section`, `article`, `figure`, `form`)
- **CSS3** vanilla, con variables CSS (`:root`) y diseño responsive mediante media queries (desktop / tablet / mobile)
- **Google Fonts** (Raleway)
- **Font Awesome** para iconografía
- Sin frameworks ni dependencias de build — el sitio corre abriendo `index.html` directamente

## Estructura del proyecto

```
curriculum/
├── index.html
├── assets/
│   ├── css/
│   │   ├── style.css      # estilos base (desktop)
│   │   ├── tablet.css     # media query ≤768px
│   │   └── movil.css      # media query ≤360px
│   └── img/                # imágenes, íconos y CV en PDF
└── README.md
```

## Cómo ejecutarlo localmente

No requiere instalación ni dependencias:

```bash
git clone https://github.com/odv144/curriculum.git
cd curriculum
```

Abrí `index.html` en el navegador, o serví la carpeta con cualquier servidor estático (por ejemplo, la extensión Live Server de VS Code) para evitar restricciones de rutas relativas.

## Secciones del sitio

| Sección | Contenido |
|---|---|
| **Sobre mí** | Presentación personal y formación de base |
| **Skills** | Front-end, Back-end y herramientas adicionales, agrupadas por categoría |
| **Formación académica** | UTN Facultad Regional Resistencia, Alura Latam, Codo a Codo 4.0 |
| **Proyectos** | Encriptador de texto (Alura + Oracle), Classmatte (NoCountry), Oceano Hotel (FooTalent) |
| **Contacto** | Formulario con validación nativa HTML5 |

## Accesibilidad

El sitio fue revisado y corregido puntualmente en:

- `lang="es"` correcto en el documento
- Un único `<h1>` por página, con jerarquía `h1 → h2 → h3` sin saltos de nivel
- `alt` en todas las imágenes (descriptivo en fotos/logos con información propia, vacío en íconos puramente decorativos que ya tienen texto al lado)
- `id` únicos + `aria-labelledby` en los grupos de skills
- Foco de teclado visible (`:focus-visible`) en links, botón e inputs
- Transiciones y animaciones respetan `prefers-reduced-motion`

## Declaración sobre el uso de IA

Para este proyecto usé **Claude (Anthropic)** como asistente durante el proceso de revisión y mejora del código ya desarrollado por mí. El uso concreto fue:

- **Revisión de código** contra una rúbrica de evaluación (estructura semántica, maquetación, estilización, interactividad, documentación), identificando puntos débiles concretos con referencias a líneas de código.
- **Correcciones de accesibilidad**: agregado de atributos `alt`, corrección de `lang`, resolución de un `id` HTML duplicado, y `aria-labelledby` en las tarjetas de skills.
- **Transiciones y micro-interacciones CSS**: agregado de `transition` en estados `:hover`/`:focus` que no existían en la versión original, y una animación de entrada (`@keyframes`) en el hero.
- **Propuesta de paleta de colores alternativa**: diseño de un segundo `style.css` con una paleta más profesional/moderna (mantenido el original disponible para comparar), manteniendo la misma estructura HTML y las mismas variables CSS para no romper el responsive existente.
- **Este README**: redacción asistida a partir de la estructura real del proyecto.

La estructura original del sitio, el contenido, las imágenes y los proyectos documentados son de mi autoría. Revisé y entendí cada cambio propuesto antes de incorporarlo al repositorio.

## Contacto

- **GitHub:** [github.com/odv144](https://github.com/odv144)
- **LinkedIn:** [linkedin.com/in/omar-virili](https://www.linkedin.com/in/omar-virili/)

---
© 2026 OdvSystem - Virili Omar
