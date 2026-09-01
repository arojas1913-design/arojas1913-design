## Iván Andrés Rojas García

Ingeniero de la Universidad de los Andes con opción académica en Economía.
Vengo del back office de la mesa de divisas y derivados de BBVA Colombia.

Construyo sistemas que **vigilan una fuente, detectan qué cambió, interpretan la
consecuencia y se niegan a afirmar lo que no pueden respaldar**. Lo he hecho
sobre portales de empleo, sobre normativa tributaria y sobre mercados
financieros. Cambia la fuente; el problema es el mismo.

Bogotá, Colombia · [LinkedIn](https://www.linkedin.com/in/iv%C3%A1n-andr%C3%A9s-rojas-garc%C3%ADa-766580180) · arojas1913@gmail.com

---

### Chamba · plataforma de búsqueda de empleo automatizada

**[chamba-e4x.pages.dev](https://chamba-e4x.pages.dev)** — en producción, en piloto cerrado.

Nació de un problema propio: buscar trabajo consume horas en tareas que no
aportan criterio. Empezó como un radar personal y hoy es una plataforma
multiusuario.

Cada madrugada, sin intervención:

- Rastrea cuatro fuentes de vacantes (LinkedIn, Computrabajo, Magneto365 y el
  Servicio Público de Empleo) y deduplica por empresa, cargo y ciudad
  normalizados — no por URL, porque los agregadores republican la misma oferta.
- Califica cada vacante contra el perfil de cada persona con una rúbrica de 100
  puntos y guarda el desglose completo: cuánto aporta la experiencia, la
  ubicación, el idioma, el nivel de estudios y las competencias.
- Adapta la hoja de vida a cada oferta en cuatro versiones —español e inglés, una
  y dos páginas— y recomienda cuál enviar.
- Redacta el mensaje al reclutador y la carta de presentación.

**La regla que gobierna el producto:** ningún documento generado dice algo que la
persona no pueda respaldar en una entrevista. Un verificador contrasta cada PDF
contra la información real de su dueño y lo bloquea si aparece un dato que no
está en la fuente. Ya ha detenido fabricaciones reales — una certificación con
el nombre ligeramente cambiado, por ejemplo.

Chamba nunca se postula por nadie. Prepara; la persona decide y envía.

**Construido con** Python, Supabase (PostgreSQL con Row Level Security y
pgvector), HTML y JavaScript sin dependencias, y Cloudflare Pages. Los
embeddings corren en local, sin coste por consulta.

---

### Radar regulatorio · vigilancia de normativa DIAN

Reto técnico para un rol de Product Regulation Analyst. Vigila la normativa
colombiana de facturación electrónica, detecta cambios comparando capturas del
texto oficial en momentos distintos, e **interpreta el impacto sobre el
producto** — no entrega el diff crudo. El resultado es un dashboard que se abre
con una URL, sin instalar nada.

Tres decisiones que definen el sistema:

**Trazabilidad como condición de publicación.** Toda afirmación lleva documento,
artículo, fecha, versión y cita literal. Antes de publicar, la cita se busca
carácter por carácter dentro de la captura oficial. Si no aparece, no se
publica: se enruta a revisión humana. Es la respuesta a la objeción obvia —
«usaste un modelo de lenguaje sobre normas»— y la respuesta es sí, y cada frase
que produjo está anclada a un texto oficial que el sistema verificó.

**Severidad por consecuencia operativa, no por retórica.** Bloqueante significa
que un documento emitido con la lógica actual sería rechazado a partir de una
fecha cierta. Mayor obliga a cambiar antes de una fecha, pero no rompe la
emisión. Menor es informativo. Y la regla de oro: ante la duda entre dos
niveles, nunca se sube para impresionar ni se baja para simplificar — se marca
revisión humana y se dice por qué. Un radar que grita ante todo es tan inútil
como uno que no avisa.

**Las fuentes viven en configuración, nunca en la lógica.** Si para agregar un
país hay que tocar código de negocio, el diseño está mal.

---

### Kara Atelier · marca de indumentaria

Cofundador desde 2023. Llevo la planificación financiera, el control de costos y
los precios. Más de $60 millones COP de ingresos acumulados y estatus de
proveedor oficial de la Universidad de los Andes, con más de 700 prendas
producidas.

---

### Herramientas

**Finanzas** — Terminal Bloomberg · Certificado AMV, Operador Básico ·
Bloomberg BMC, BFF, ESG y BQL · matemática financiera · valoración de proyectos

**Datos** — Python · Excel avanzado · automatización de procesos con agentes de
IA · SQL sobre PostgreSQL

**Idiomas** — Español nativo · Inglés B2

---

### Sobre los repositorios privados

La mayoría de mis proyectos están en privado porque son productos en curso o
manejan datos personales de terceros. Con gusto muestro el código en una
conversación o doy acceso puntual si el proceso lo requiere.
