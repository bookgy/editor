# Registro de decisiones editoriales

Este archivo registra las decisiones, correcciones y aprendizajes que modifican el funcionamiento del Editor de Agendic.

Su objetivo es evitar que un criterio editorial dependa de una conversación, de memoria externa o de un archivo fuera del repositorio.

## Regla de registro

`bookgy/editor` es la fuente única de verdad del sistema editorial.

Cuando el usuario aporte un comentario, corrección o criterio que cambie la forma de trabajar:

1. identificar si afecta a todo el Editor, a un canal, a una Skill, a una semilla o a una pieza concreta;
2. aplicar el cambio en el archivo canónico correspondiente;
3. registrar aquí la decisión de forma estructurada;
4. indicar los archivos afectados;
5. si una decisión sustituye a otra anterior, marcar la anterior como sustituida y enlazar la nueva.

No dejar reglas operativas únicamente en la conversación.

No utilizar un ZIP, documento local o memoria externa como fuente canónica cuando el cambio pertenece al Editor.

## Formato

```markdown
## DEC-AAAA-MM-NNN — Título

- fecha: AAAA-MM-DD
- estado: vigente | sustituida
- alcance: global | canal | skill | semilla | contenido
- afecta a:
  - `ruta/del/archivo`
- decisión:
  - ...
- aplicación:
  - ...
- sustituye a: opcional
- notas: opcional
```

El registro resume la decisión. La regla operativa completa debe vivir también en el archivo canónico correspondiente.

---

## DEC-2026-09-001 — LinkedIn como canal de autoridad fitness

- fecha: 2026-09-16
- estado: vigente
- alcance: canal
- afecta a:
  - `_referencias/guia-redaccion.md`
  - `_skills/entrada-linkedin/SKILL.md`
- decisión:
  - LinkedIn debe posicionar a Agendic principalmente como una marca experta en la gestión de centros deportivos, gimnasios, Pilates, yoga, entrenamiento, boxes, boxeo y negocios fitness comparables.
  - Cada publicación debe dirigirse a un perfil principal reconocible: CEO o propietario, gerente, director de centro o sede, recepción o administración, entrenador o profesional, u otro perfil cuando proceda.
  - La autoridad debe demostrarse mediante conocimiento de la operativa y de los dolores reales de cada perfil.
- aplicación:
  - Priorizar problemas, criterios, métodos y situaciones reales del sector antes que contenidos de producto.
  - Buscar una voz ágil, fresca y dinámica, con autoridad y conocimiento sectorial.
  - Tomar como referencias estilísticas la agilidad y frescura observadas en Holded y la contundencia y especialización sectorial observadas en Trainingym, sin copiar su voz.

## DEC-2026-09-002 — La marca es el emisor, no la solución explícita

- fecha: 2026-09-16
- estado: vigente
- alcance: canal
- afecta a:
  - `_referencias/guia-redaccion.md`
  - `_skills/entrada-linkedin/SKILL.md`
  - `entradas/2026-09-001-cupones-promocionales/linkedin-001.md`
- decisión:
  - Por defecto, una publicación de LinkedIn no debe mencionar `Agendic` ni presentar el producto como la solución.
  - La marca ya está presente en la cuenta que publica.
  - Una funcionalidad interna debe transformarse editorialmente en conocimiento útil: dolor, principio de gestión, solución genérica y ejemplo.
- aplicación:
  - Explicar cómo resolver el problema mediante una regla, proceso, configuración, automatización, criterio, rutina, métrica o forma de organizar el trabajo.
  - Mencionar producto solo cuando la publicación sea expresamente de producto, novedad, lanzamiento o funcionalidad.
  - Evitar rutas de menú y CTA comerciales en publicaciones editoriales normales.

## DEC-2026-09-003 — Tono de LinkedIn más fluido y menos formularizado

- fecha: 2026-09-16
- estado: vigente
- alcance: canal
- afecta a:
  - `_referencias/guia-redaccion.md`
  - `_skills/entrada-linkedin/SKILL.md`
  - `entradas/2026-09-001-cupones-promocionales/linkedin-001.md`
- decisión:
  - Las publicaciones deben sentirse como una conversación profesional bien pensada, no como una plantilla de marketing o una tesis de consultoría.
- aplicación:
  - Variar ritmo y estructura.
  - No abusar de frases telegráficas, negritas, listas, grandes tesis o transiciones rígidas.
  - Mantener contundencia en la observación y naturalidad en la forma.
  - Cerrar cuando la idea esté completa, sin añadir venta por obligación.

## DEC-2026-09-004 — Cierres participativos basados en experiencia real

- fecha: 2026-09-16
- estado: vigente
- alcance: canal
- afecta a:
  - `_referencias/guia-redaccion.md`
  - `_skills/entrada-linkedin/SKILL.md`
  - `entradas/2026-09-001-cupones-promocionales/linkedin-001.md`
- decisión:
  - Algunas publicaciones pueden cerrar abriendo conversación con una pregunta concreta sobre la experiencia u operativa real del lector.
  - No utilizar preguntas genéricas únicamente para provocar comentarios.
- aplicación:
  - Preferir preguntas fáciles de responder desde una experiencia concreta.
  - `Os leemos` o `Os leemos en comentarios` puede utilizarse cuando resulte natural.
  - Alternar este recurso con conclusiones, recomendaciones y reflexiones; no convertirlo en una coletilla fija.

## DEC-2026-09-005 — GitHub como única fuente de verdad del Editor

- fecha: 2026-09-16
- estado: vigente
- alcance: global
- afecta a:
  - `README.md`
  - `_referencias/decisiones-editoriales.md`
- decisión:
  - Todo comentario, corrección o aprendizaje que cambie el criterio, el proceso o una pieza editorial debe quedar estructurado y registrado dentro de `bookgy/editor`.
- aplicación:
  - Actualizar siempre el archivo canónico afectado.
  - Añadir una entrada a este registro para mantener trazabilidad de la decisión.
  - No considerar la conversación, una Skill empaquetada externamente, un ZIP o un documento local como sustituto del contenido registrado en GitHub.

## DEC-2026-09-006 — Variedad de formatos sin perder lector, dolor ni profundidad

- fecha: 2026-09-16
- estado: vigente
- alcance: canal
- afecta a:
  - `_skills/entrada-linkedin/SKILL.md`
  - `entradas/2026-09-001-cupones-promocionales/linkedin-002.md`
- decisión:
  - Las publicaciones de LinkedIn no deben compartir una misma plantilla, longitud o estructura.
  - La variedad de formato no puede utilizarse como excusa para escribir contenido genérico.
  - Cada publicación debe tener un perfil principal y un dolor principal reconocibles en el propio texto, no solo en los metadatos.
  - La profundidad debe elegirse de manera intencionada: breve, media o desarrollada según lo que necesite la idea.
- aplicación:
  - Permitir variantes como insight breve, tesis desarrollada, escena operativa, consejo o método, caso de uso, historia real, contexto sectorial o producto explícito.
  - Un post breve debe seguir siendo específico y completo.
  - Cuando un gancho abra una tensión relevante, desarrollar suficientemente el problema, sus consecuencias y el criterio para resolverlo.
  - Evitar dolores abstractos como `mejorar la gestión`, `tener más control` o `ser más eficiente` cuando puedan concretarse en una situación operativa.
  - Incorporar en los metadatos `dolor` y `profundidad` para hacer explícitas estas decisiones editoriales.

## DEC-2026-09-007 — La pieza desarrollada pasa de entrada a blog

- fecha: 2026-09-17
- estado: vigente
- alcance: global
- afecta a:
  - `README.md`
  - `_skills/README.md`
  - `_skills/entrada-blog/SKILL.md`
  - `_skills/entrada-blog/agents/openai.yaml`
  - `_skills/entrada-linkedin/SKILL.md`
  - `_skills/entrada-instagram/SKILL.md`
  - `_skills/entrada-x/SKILL.md`
  - `_skills/entrada-tiktok/SKILL.md`
  - `_skills/newsletter/SKILL.md`
  - `_referencias/editorial.md`
  - `_referencias/guia-redaccion.md`
  - `entradas/2026-09-001-cupones-promocionales/blog.md`
- decisión:
  - La Skill genérica `entrada` deja de existir y pasa a llamarse `entrada-blog`.
  - La pieza desarrollada deja de llamarse `entrada.md` y pasa a llamarse `blog.md`.
  - `entrada-semilla`, `entrada-linkedin`, `entrada-instagram`, `entrada-x` y `entrada-tiktok` mantienen sus nombres.
  - La carpeta raíz `entradas/` mantiene su nombre porque representa temas editoriales, no únicamente publicaciones de blog.
  - El blog es una pieza derivada de la semilla y no un paso obligatorio previo a los demás canales.
- aplicación:
  - La estructura de Skills utiliza `_skills/entrada-blog/` en lugar de `_skills/entrada/`.
  - Las Skills de canal leen `blog.md` solo si existe y nunca dependen de él para crear una pieza.
  - Los canales no deben ser resúmenes automáticos del blog; todos derivan de la misma `semilla.md`.
  - Las referencias generales sustituyen el concepto `entrada principal` por `blog` cuando hablan de la pieza desarrollada.
  - El contenido existente `entrada.md` de la semilla `2026-09-001` se migra a `blog.md` sin alterar su contenido editorial.
