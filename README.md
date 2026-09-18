# ProcedencIA

Trazabilidad del uso de IA en un manuscrito académico, en un único HTML.

**App:** https://fborrasumh.github.io/procedencia/

Registra la evolución del manuscrito en puntos de control (borrador humano, pre-IA, post-IA, revisión humana y versión final) sellados con una cadena SHA-256 y fechados automáticamente, de modo que cualquier alteración posterior rompe la verificación. Incluye un registro de cada uso de IA, comparación por palabras entre versiones, un análisis con OpenAI que busca contenido sustantivo nuevo introducido entre dos versiones y la exportación de un dossier de procedencia (Markdown o PDF) con borrador de declaración de uso de IA. Está pensado para responder a políticas como la del NeurIPS 2026 Position Paper Track, que exige un punto previo a la IA, uno posterior y la versión final.

- Vanilla JS, persistencia en IndexedDB, clave de OpenAI en el navegador (`ia_openai_key`), gpt-4o-mini por defecto y selector con los modelos de la cuenta.
- Lee PDF, DOCX, TXT, MD y TEX. Importa las reescrituras de [AutorIA](https://github.com/fborrasumh/autoria) como punto de control.

**Nota:** es una herramienta de documentación, no de ocultación. No modifica el texto, no permite fechar versiones a mano y no sustituye al historial de versiones del editor original (Overleaf, Google Docs, Git), que conviene conservar y enlazar en el dossier.

Autor: Fernando Borrás Rocher (UMH) · ORCID [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573) · Licencia MIT
