# Casa Fresca Florida

Sitio estático de contenido en español para dueños de casa en Florida: cuidado del
aire acondicionado, humedad y moho, ahorro de energía en el hogar, mantenimiento
preventivo y preparación para la temporada de huracanes.

Es el embudo público del producto de Brayan en Hotmart **«AC Bajo Control»** (en
preparación): el sitio educa, genera confianza y prepara la audiencia; cuando el
producto exista, los cierres de los artículos apuntarán a su página de ventas.
Puede llevar enlaces de afiliado de Hotmart **solo** donde un producto encaje de
verdad con el tema del artículo (ver reglas abajo).

**URL final esperada:** https://mashlanzer.github.io/casa-fresca-florida/

## Estructura

```
sitio-casa-fresca/
├── index.html              Portada: promesa, lista de artículos, divulgación
├── plantilla-articulo.html Plantilla oficial para artículos nuevos
├── articulos/              Un .html por artículo (publicados desde la plantilla)
├── sitemap.xml             Mapa del sitio (actualizar con cada artículo)
├── robots.txt              Permite todo y declara el sitemap
└── README.md               Este archivo
```

Todo es HTML + CSS dentro de cada archivo: sin dependencias externas, sin build,
sin JavaScript. Rápido y publicable tal cual.

## Cómo se publica (GitHub Pages)

1. Crear un repositorio público llamado `casa-fresca-florida` en la cuenta de
   GitHub de Brayan (MashLanzer).
2. Subir el contenido completo de esta carpeta a la raíz del repositorio
   (index.html debe quedar en la raíz, `articulos/` como carpeta).
3. En el repositorio: Settings → Pages → Build and deployment → Source:
   «Deploy from a branch», rama `main`, carpeta `/ (root)`. Guardar.
4. Esperar el despliegue y verificar la URL final y que los enlaces internos
   (portada → artículos → volver a portada) carguen bien.
5. Cada artículo nuevo es un commit más: archivo en `articulos/`, tarjeta en
   `index.html` y URL nueva en `sitemap.xml`.

Nota: `plantilla-articulo.html` y este README pueden vivir en el repo sin
problema (no afectan al sitio), pero la plantilla nunca se añade ni al sitemap
ni al índice de artículos.

## Reglas de contenido (no negociables)

- **Datos verificados:** toda cifra o recomendación técnica (rangos de humedad,
  intervalos de mantenimiento, pasos de seguridad) se verifica con búsqueda en
  fuentes confiables (EPA, fabricantes, guías HVAC establecidas) antes de
  publicar. Nada de datos inventados.
- **Seguridad del lector:** nada de instrucciones peligrosas. Refrigerante,
  electricidad interna, abrir el equipo o trabajos en el panel = siempre
  «llama a un técnico licenciado». Cada artículo lleva su bloque de seguridad
  cuando el tema lo toque.
- **Sin promesas mágicas:** prohibido prometer ahorros o resultados garantizados
  («baja tu factura un 40%»). Se habla de buenas prácticas y de lo que puede
  pasar, no de milagros.
- **Afiliados con honestidad:** un enlace de afiliado solo entra si el producto
  ayuda de verdad con el tema EXACTO del artículo (bloque `.afiliado` de la
  plantilla, marcado como enlace de afiliado). Si ninguno encaja, el artículo
  va sin enlaces. En este nicho lo normal es que no encaje ninguno: el activo
  del sitio es el contenido y el embudo a «AC Bajo Control».
- **Divulgación siempre visible:** el pie con la divulgación de afiliados va en
  todas las páginas, haya o no enlaces en esa página.

## Especificación de la rutina semanal de contenido

**Cadencia:** 2 artículos nuevos por semana, generados desde
`plantilla-articulo.html`, sin tocar el estilo ni la estructura.

**Flujo por artículo:**

1. **Tema:** elegir del banco de temas del nicho (mantenimiento del AC,
   humedad/moho, ahorro de energía, calidad del aire, huracanes, señales de
   alerta, mitos comunes). No repetir temas ya publicados; favorecer lo
   estacional (huracanes en primavera, humedad en verano, filtros todo el año).
2. **Investigación:** búsqueda web del tema; verificar cada dato técnico clave
   en al menos una fuente confiable y anotar las fuentes en el pie del artículo
   («Fuentes consultadas»).
3. **Redacción:** escribir desde la plantilla — título, meta descripción, H1,
   secciones, bloque de seguridad si aplica, cierre estándar con la llamada
   suave a «AC Bajo Control» y pie con divulgación. Tono claro para dueños de
   casa, sin tecnicismos sin explicar.
4. **Revisión de seguridad:** releer buscando instrucciones peligrosas o
   promesas mágicas; si aparece alguna, se corrige o se deriva a «llama a un
   técnico» antes de publicar.
5. **Publicación:** guardar en `articulos/<slug>.html`, añadir su tarjeta en
   `index.html` (arriba de la lista, lo más nuevo primero) y su URL en
   `sitemap.xml`.
6. **Registro:** anotar en un registro de publicación (fecha, título, slug,
   fuentes usadas, si llevó enlace de afiliado y por qué). El registro vive
   junto al estado de la rutina, no en este paquete público.

**Reporte:** la rutina NO reporta artículo por artículo. Solo entrega:
(a) un **resumen mensual** (artículos publicados, temas, cualquier enlace de
afiliado usado con su justificación), o (b) un aviso inmediato si hay un
**problema** (un dato que no se pudo verificar y frenó un artículo, un error
en el sitio, una corrección necesaria en algo ya publicado).
