# Tobos Propiedad Intelectual — sitio web

Sitio web oficial de **Tobos Abogados S.A.S.** (www.tobos.com.co).
Es un sitio estático (HTML + CSS). No necesita instalar nada ni compilar: se abre directamente en el navegador.

## Estructura

```
tobos-web/
├── index.html        Página de bienvenida (Inicio)
├── servicios.html    Nuestros servicios
├── equipo.html       Nuestro equipo
├── noticias.html     Noticias
├── contacto.html     Contacto y formulario
├── gracias.html      Página que se muestra después de enviar el formulario
├── 404.html          Página de error (dirección no encontrada)
├── css/styles.css    Estilos generales
├── img/              Logos y favicon
├── robots.txt        Indica a Google que puede rastrear el sitio
└── sitemap.xml       Mapa del sitio para Google
```

## Ver el sitio en su computador

Abra `index.html` con doble clic. Se verá en su navegador.

## Subirlo a GitHub

1. Cree un repositorio nuevo en https://github.com/new (por ejemplo `tobos-web`).
2. En el repositorio, haga clic en **Add file › Upload files** y arrastre **el contenido** de esta carpeta (no la carpeta misma).
3. Haga clic en **Commit changes**.

## Publicarlo gratis con GitHub Pages en www.tobos.com.co

1. En el repositorio: **Settings › Pages**.
2. En *Source* elija **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarde.
3. En *Custom domain* escriba `www.tobos.com.co` y guarde. Luego active **Enforce HTTPS** (aparece cuando el dominio esté verificado).
4. En el panel de su proveedor de dominio (donde compró tobos.com.co), configure el DNS:
   - Registro **CNAME**: `www` → `SU-USUARIO.github.io`
   - Registros **A** para `tobos.com.co` (sin www):
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
5. Los cambios de DNS pueden tardar hasta 24 horas.

> **Ojo con el correo:** si su correo tobos@tobos.com.co funciona con el mismo proveedor, **no borre ni cambie los registros MX**. Solo modifique los registros A y CNAME indicados arriba.

Si prefiere seguir con su hosting actual, basta con subir estos archivos a la carpeta pública del hosting (por FTP o el administrador de archivos) y pedirle al proveedor que active el certificado SSL (HTTPS).

## Formulario de contacto

El formulario usa el servicio gratuito [FormSubmit](https://formsubmit.co), que reenvía cada consulta al correo **tobos@tobos.com.co**.
La **primera vez** que alguien envíe el formulario, llegará un correo de FormSubmit pidiendo activar el formulario: haga clic en el enlace de confirmación. Desde ese momento las consultas llegarán a su bandeja.

## Para aparecer en Google

1. Publique el sitio con HTTPS en www.tobos.com.co.
2. Entre a [Google Search Console](https://search.google.com/search-console), agregue la propiedad `https://www.tobos.com.co` y verifíquela.
3. En *Sitemaps*, envíe `sitemap.xml`.
4. En *Inspección de URL*, pida la indexación de la página de inicio.
5. Cree o actualice su [Perfil de Empresa en Google](https://www.google.com/business/) con la misma dirección, teléfono y sitio web.
6. Publique noticias con regularidad en `noticias.html`: el contenido nuevo ayuda a posicionar el sitio.

Cada página ya incluye título, descripción para Google, enlace canónico, etiquetas para redes sociales y, en el inicio, datos estructurados (schema.org `LegalService`) con la dirección y el teléfono de la firma.

## Pendiente por completar

Busque en los archivos el texto entre corchetes `[ ]` y reemplácelo:

- `equipo.html`: nombres, cargos, fotos y perfiles de los abogados (las fotos van en `img/`).
- `contacto.html`: horario de atención, enlace a la política de tratamiento de datos y mapa de Google.
- `noticias.html`: títulos, fechas y textos de las publicaciones.

## Editar textos

Los textos están directamente en cada archivo `.html`. Puede editarlos en GitHub (botón del lápiz ✏️) o con un editor como Visual Studio Code.

Colores de marca: azul `#2B2F8F`, rojo `#A8433A`. Tipografías: EB Garamond (títulos) y Source Sans 3 (texto), de Google Fonts.
