# Alicia Ruiz Gómez · Web y CV

Mi web personal: **[aliciaruiz.dev](https://aliciaruiz.dev)**

Estudiante del Doble Grado en ADE e Ingeniería Informática (mención en Ingeniería de Computadores) en la Universidad de Granada. En la web reúno mi CV, mis proyectos y algunas notas de lo que voy aprendiendo.

📄 [Descargar el CV en PDF](https://aliciaruiz.dev/CV_Alicia_Ruiz_Gomez.pdf)

## Qué hay en la web

| Página | Contenido |
| --- | --- |
| [Inicio](https://aliciaruiz.dev/) | Sobre mí, habilidades, formación, experiencia, proyectos e idiomas |
| [Proyectos](https://aliciaruiz.dev/proyectos.html) | Detalle de cada proyecto: qué es, cómo lo hice y con qué |
| [Blog](https://aliciaruiz.dev/blog.html) | Notas de lo que voy aprendiendo |
| [Contacto](https://aliciaruiz.dev/contacto.html) | Cómo escribirme |

## Cómo está hecha

- HTML y CSS a mano, sin frameworks ni paso de compilación.
- Tipografías de Google Fonts (Nunito, Fredoka, JetBrains Mono y Caveat).
- Ilustraciones en SVG dentro del propio HTML.
- Publicada con **GitHub Pages** desde la rama `main`, con dominio propio (archivo `CNAME`).

```
index.html             Página principal (y fuente del CV en PDF)
proyectos.html         Proyectos
blog.html              Índice del blog
nota-github-pages.html Entrada: cómo publiqué la web
contacto.html          Contacto
style.css              Estilos de la web y de impresión
CV_Alicia_Ruiz_Gomez.pdf  CV descargable
CNAME                  Dominio propio
```

## Ver la web en local

Basta con abrir `index.html` en el navegador. No hace falta instalar nada.

## Regenerar el CV en PDF

El PDF sale de `index.html`: `style.css` tiene estilos de impresión (`@media print`) que ocultan la navegación y las ilustraciones y ajustan todo a una página A4. Para regenerarlo con Chrome (PowerShell, desde la carpeta del repo):

```powershell
& "C:\Program Files\Google\Chrome\Application\chrome.exe" --headless=new --no-pdf-header-footer --virtual-time-budget=8000 --print-to-pdf="$PWD\CV_Alicia_Ruiz_Gomez.pdf" "file:///$($PWD -replace '\\','/')/index.html"
```

También vale abrir `index.html` en el navegador e imprimir a PDF (A4, sin encabezados ni pies de página).

## Contacto

- GitHub: [@Aliciarg04](https://github.com/Aliciarg04)
- LinkedIn: [Alicia Ruiz Gómez](https://www.linkedin.com/in/alicia-ruiz-g%C3%B3mez-1591bb43b/)
- Correo: en la [página de contacto](https://aliciaruiz.dev/contacto.html)
