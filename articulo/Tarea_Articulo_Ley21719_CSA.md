# MÁSTER EN INTELIGENCIA ARTIFICIAL GENERATIVA Y NO CODE

Universidad Complutense de Madrid · ntic master

**TAREA**

**IA GENERATIVA APLICADA AL MARKETING Y EMPRESA**

Alumno: Carlos Oberreuter

Profesor: Arnau Vendrell Pérez

Junio 2026

# 1. TAREA

Generar 1 artículo de 500 palabras máximo con su correspondiente: Título, meta descripción, contenido e imagen destacada.

Para la elección del artículo, escoged una web sobre cuya temática tengáis conocimiento experto, como si fuerais a publicar realmente en ella (ej.: web.com/blog).

Por ejemplo: si soy abogado especializado en divorcios, crearé un artículo pensado para publicarse en abogadofamiliasevilla.com/blog. Si no se os ocurre ninguna, podéis usar como referencia vuela.ai/es/blog.

Se valorarán los siguientes aspectos:

- Argumentación sobre por qué se ha elegido ese tipo de artículo y cómo se ha identificado la oportunidad.
- Coherencia del artículo con el tono, estilo y línea visual del proyecto Vuela.ai, incluyendo el valor y la pertinencia de la imagen destacada.
- Correcta aplicación y justificación de las metodologías y herramientas vistas en el curso, así como de cualquier otra que consideréis relevante.

# Desarrollo

# Elección del Tema

La propuesta aborda una necesidad inmediata del mercado chileno: traducir la Ley 21.719 desde el lenguaje jurídico hacia controles técnicos verificables antes de su entrada en vigencia el 1 de diciembre de 2026. El tema conecta una búsqueda coyuntural, cómo prepararse para la nueva ley, con la autoridad profesional del autor en cloud security, Zero Trust y el ecosistema de Cloud Security Alliance.

Ángulo diferencial

La ley no se presenta como un problema exclusivamente legal: se demuestra que la capacidad de responder a una fiscalización depende de evidencia técnica , inventarios, accesos, logs, cifrado y gestión de incidentes, que el CCM ayuda a estructurar.

# Intención y valor del contenido

- Responde a una necesidad informacional con impacto comercial: preparación técnica para la Ley 21.719.
- Conecta un asunto local y urgente con un framework internacional reconocido.
- Evita el contenido genérico al incorporar experiencia de campo y una recomendación priorizada.
- Puede generar conversaciones de assessment, readiness, arquitectura y gobierno de datos.

# Uso de IA y revisión humana

La IA se empleó para organizar la oportunidad editorial, proponer alternativas de título, condensar el artículo, revisar patrones de redacción y generar la imagen destacada. La revisión humana aportó el conocimiento experto, ajustó el tono y corrigió afirmaciones legales o técnicas que podían parecer plausibles, pero no eran exactas.

Entre las correcciones verificadas se encuentran: el régimen real de multas de la ley, la ausencia de un plazo general de 72 horas para notificar brechas y la composición vigente del CCM v4.1, que reúne 207 controles en 17 dominios.

**URL:** <https://oberreu.github.io/Inteligencia-artificial-generativa-aplicado-al-marketing-y-empresa/>

Articulo publicado (entregable): Ley 21.719 y la nube: el mapa de controles de la CSA

# Conceptos de clase aplicados

| Concepto visto en clase | Como se aplico en el entregable |
| --- | --- |
| Contenido non-commodity vs commodity (Hobo / Google 2026) | Se evito el contenido generico replicable por cualquier LLM. Se aporto un artefacto unico: la tabla de mapeo Ley 21.719 - CCM, no disponible en otra fuente. |
| E-E-A-T (Experience, Expertise, Authoritativeness, Trust) | Autoria real e identificable (nombre, cargo, foto), framing de experiencia en primera persona, transparencia editorial e independencia en el footer. |
| GEO (Generative Engine Optimization) | Parrafo sesamo citable por IA, glosario con datos estructurados, lenguaje declarativo y entidades nombradas para facilitar la cita por motores generativos. |
| SEO tecnico | sitemap.xml, robots.txt, verificacion en Google Search Console, frescura (dateModified / article:modified_time). |
| Datos estructurados (Schema.org) | Tres bloques JSON-LD: BlogPosting, FAQPage y DefinedTermSet, con publisher (url + logo) y author enriquecidos para Entity Trust. |
| Arquitectura pillar + cluster | Articulo pilar + tres articulos de cluster (multas, EIPD, notificacion de brechas) interconectados. |
| Evitar AI-tells | Revision de estilo para eliminar marcas delatoras de IA (en especial el guion largo / em-dash). |
| Prompting iterativo y validacion | Trabajo por iteraciones cortas con verificacion factual contra fuente oficial (BCN) tras cada generacion. |
| Voz y autoridad del autor | Posicionamiento desde la experiencia en ciberseguridad cloud, no generico. |

# Herramientas utilizadas

- GitHub Copilot Chat (modo agente) en VS Code - asistente de IA generativa para redaccion, refactor de HTML/CSS, generación de datos estructurados y automatizacion del flujo.
- VS Code - entorno de edicion y orquestación.
- Git + GitHub Pages - control de versiones y despliegue continuo del sitio estatico.
- HTML estático + CSS - pilar con CSS inline y cluster con hoja compartida assets/blog.css. Sin dependencias de runtime.
- JSON-LD (Schema.org) - datos estructurados para SEO y GEO.
- Google Search Console - verificación de propiedad, indexacion y envío de sitemap.
- Semrush - diagnostico de visibilidad y palabras clave.
- Biblioteca del Congreso Nacional de Chile (BCN) - fuente oficial para validar cifras y articulos legales.
- PowerShell (pwsh) - automatizacion de copia de archivos (sincronizacion pilar/mirror), commits y push.
- Generación de imagen (modelo de difusion) - imagen Open Graph ley-21719-og.jpg (1200x675) para compartir en redes y como publisher.logo.

# Modelos de IA utilizados

- Claude (Anthropic) - modelo principal de lenguaje detrás del asistente, usado para redacción experta, generacion de schema, validacion de razonamiento legal-técnico y automatizacion del flujo de publicacion.
- Modelo de generación de imagenes (texto a imagen) - para la imagen de portada / Open Graph.
- Nota de metodo: ningun dato legal se dio por valido por el solo hecho de provenir del modelo. Cada cifra (UTM, porcentajes de reincidencia, plazos) se contrasto contra el texto oficial de la Ley 21.719 en la BCN antes de publicar. La IA acelero la produccion; la verificacion humana garantizo la exactitud.

# 2. Proceso e iteraciones seguidas

El entregable se construyó mediante prompting iterativo en GitHub Copilot Chat (modo agente) sobre VS Code, con verificación humana en cada paso. A continuación se documenta la secuencia real de iteraciones que llevó del análisis de la tarea al sitio publicado y validado.

1. **Análisis de la tarea y la clase.** Resumen del módulo, la sesión y la rúbrica a partir del temario (PDF), la transcripción de la clase y el PDF de la tarea, para fijar criterios de evaluación.
2. **Borrador del artículo.** Redacción del primer entregable y de una versión mejorada (v2) integrando los conceptos de clase (E-E-A-T, contenido non-commodity, GEO).
3. **Alineación con Vuela.ai y la rúbrica.** Análisis de cumplimiento contra la rúbrica y ajuste del tono, estilo y línea visual (paleta e imagen destacada) al proyecto de referencia.
4. **Implementación del blog.** Construcción del artículo pilar en HTML/CSS estático y verificación del render.
5. **Publicación inicial en GitHub Pages.** Carga del contenido al repositorio y activación de GitHub Pages; verificación del sitio en vivo.
6. **Rediseño profesional y marca CSA Latam Hub.** Rebranding a 'CSA Latam Hub' (paleta navy/teal), incorporación del rol 'Senior Cloud Solution Architect Manager of Cybersecurity' e imagen destacada de marca.
7. **Arquitectura pillar + cluster.** Creación de tres artículos de clúster (multas, EIPD y notificación de brechas) interconectados con el pilar para dar profundidad temática.
8. **Validación factual contra fuente oficial.** Contraste de todas las cifras (UTM, plazos, reincidencia) y la composición del CCM v4.1 (207 controles, 17 dominios) contra el texto oficial de la Ley 21.719 en la BCN (idNorma 1209272), corrigiendo datos imprecisos.
9. **SEO técnico y GEO.** sitemap.xml, robots.txt, verificación en Google Search Console, datos estructurados JSON-LD (BlogPosting, FAQPage, DefinedTermSet), señales de frescura (dateModified / article:modified_time) y párrafo sésamo citable por IA.
10. **Pulido editorial y eliminación de AI-tells.** Revisión de estilo para eliminar marcas delatoras de IA (en especial el em-dash) y aplicación de prácticas de contenido non-commodity (Hobo / Google 2026).
11. **Autoría y confianza.** Sección 'Sobre el autor' con foto real y datos de contacto, reforzando E-E-A-T y Entity Trust.
12. **Documentación de la metodología.** Registro de iteraciones, herramientas, modelos y prompts utilizados, y generación de este documento como evidencia del proceso.

Nota de método: ningún dato legal se dio por válido por provenir del modelo. La IA aceleró la producción (organización, redacción, refactor de HTML/CSS, generación de schema e imágenes); la verificación humana garantizó la exactitud frente a la fuente oficial antes de cada publicación.
