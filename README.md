# Inteligencia Artificial Generativa aplicada al marketing y empresa

Entrega del módulo **"IA generativa aplicada al marketing y empresa"** del Máster NTIC en Inteligencia Artificial (UCM) — Profesor: Arnau Vendrell Pérez.

**Autor:** Carlos Oberreuter — *Senior Cloud Solution Architect Manager of Cybersecurity*

Sitio publicado bajo la marca **CSA Latam Hub**.

## 🌐 Blog publicado

El contenido se publica como sitio estático (GitHub Pages):

> **[Ver el blog en vivo](https://oberreu.github.io/Inteligencia-artificial-generativa-aplicado-al-marketing-y-empresa/)**

## 🏗️ Arquitectura del sitio (pillar + cluster)

Un artículo **pilar** rodeado de tres artículos de **clúster** interconectados, para dar profundidad temática y autoridad:

| Página | Rol |
|--------|-----|
| [`index.html`](index.html) | **Pilar:** Ley 21.719 y la nube — el mapa de controles de la CSA |
| [`multas-ley-21719.html`](multas-ley-21719.html) | Clúster: régimen de multas de la Ley 21.719 |
| [`evaluacion-impacto-eipd-ley-21719.html`](evaluacion-impacto-eipd-ley-21719.html) | Clúster: evaluación de impacto (EIPD) |
| [`notificacion-brechas-ley-21719.html`](notificacion-brechas-ley-21719.html) | Clúster: notificación de brechas |

## 📄 Contenido del repositorio

| Archivo | Descripción |
|---------|-------------|
| [`index.html`](index.html) | Artículo pilar (HTML + imagen destacada generada con IA, SEO/GEO con JSON-LD) |
| `*-ley-21719.html` | Tres artículos del clúster (hoja de estilos compartida `assets/blog.css`) |
| [`articulo/Tarea_Articulo_Ley21719_CSA.md`](articulo/Tarea_Articulo_Ley21719_CSA.md) | Documento de la tarea: argumentación, conceptos de clase, herramientas, modelos y proceso/iteraciones seguidas |
| [`RESUMEN_Modulo_y_Clase.md`](RESUMEN_Modulo_y_Clase.md) | Resumen del temario del módulo y de la sesión en vivo |
| `sitemap.xml`, `robots.txt`, `.nojekyll` | Infraestructura de indexación y despliegue |
| `google03337a3ad94d930e.html` | Verificación de Google Search Console |
| `assets/` | Imágenes (imagen destacada, foto del autor, Open Graph) y CSS compartido |

## 🧪 Tema del artículo

**Ley 21.719 y la nube: el mapa de controles de la CSA** — cómo usar la Cloud Controls Matrix (CCM v4.1: 207 controles en 17 dominios) de la Cloud Security Alliance para traducir las obligaciones de la nueva Ley de Protección de Datos de Chile en controles técnicos verificables, antes de su entrada en plena vigencia en diciembre de 2026.

## 🛠️ Metodología y herramientas

- Estrategia de contenido con IA en 5 pasos (contexto con fuentes verificadas → intención de búsqueda + keyword research → datos SEO → sin patrones de IA → valor real).
- **Contenido non-commodity** (Hobo / Google 2026): artefacto único (tabla de mapeo Ley 21.719 → CCM) no replicable por un LLM genérico.
- **E-E-A-T**: autoría real e identificable (nombre, cargo, foto) y transparencia editorial.
- **SEO técnico + GEO**: `sitemap.xml`, `robots.txt`, Google Search Console, datos estructurados JSON-LD (BlogPosting, FAQPage, DefinedTermSet), señales de frescura y párrafo sésamo citable por IA.
- **Verificación de fuentes / anti-alucinación**: cada cifra (UTM, reincidencia, plazos) se contrastó contra el texto oficial de la Ley 21.719 en la **BCN** (idNorma 1209272); se corrigieron datos importados del RGPD.
- **Herramientas:** GitHub Copilot Chat (modo agente) en VS Code · Git + GitHub Pages · HTML/CSS estático · JSON-LD · Google Search Console · Semrush · PowerShell · generación de imágenes (texto a imagen).
- **Modelos:** Claude (Anthropic) para redacción, schema y razonamiento legal-técnico; modelo texto-a-imagen para la portada / Open Graph.

> 📌 La IA aceleró la producción; la verificación humana garantizó la exactitud frente a la fuente oficial antes de cada publicación.
