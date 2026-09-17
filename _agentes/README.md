# Agentes del Editor

Esta carpeta define las **órdenes de trabajo invocables** del Editor de Agendic.

Los agentes no sustituyen a las Skills ni duplican sus reglas. Su función es interpretar una intención, decidir qué información y procesos necesita, coordinar una o varias Skills y entregar o guardar el resultado adecuado.

## Arquitectura

```text
_fuentes/         → de dónde sale la verdad factual
_reglas/          → criterios editoriales y de redacción
_agentes/         → qué trabajo queremos realizar y cómo se orquesta
_skills/          → cómo ejecutar tareas editoriales concretas
entradas-editor/  → semillas y piezas derivadas por canal
newsletters/      → semillas y ediciones de newsletter
```

La relación preferida es:

**objetivo del usuario → agente → reglas y fuentes necesarias → Skills necesarias → resultado**

Una Skill puede seguir invocándose directamente cuando el usuario pida una tarea concreta. Los agentes existen para resolver encargos más amplios, flexibles o compuestos.

## Jerarquía de decisión

Al ejecutar un agente:

1. respetar la fuente factual autorizada definida en `_fuentes/`;
2. respetar las reglas vigentes de `_reglas/`;
3. respetar el objetivo, alcance y restricciones expresas del usuario;
4. utilizar este agente para decidir el flujo de trabajo;
5. aplicar las Skills específicas necesarias para ejecutar cada pieza.

Una instrucción puntual puede cambiar canales, público, profundidad, cantidad de piezas, periodo o enfoque. No puede convertir una suposición en un hecho ni invalidar una condición factual confirmada.

## Invocación

Los agentes pueden invocarse por nombre o mediante lenguaje natural.

Ejemplos:

- `00_planifica-contenido`: «Planifica octubre para LinkedIn e Instagram».
- `01_crea-semilla`: «Crea una semilla sobre el problema de los cobros pendientes».
- `02_desarrolla-semilla`: «Desarrolla la semilla 2026-09-001 para LinkedIn y X».
- `03_revisa-contenido`: «Revisa todos los LinkedIn de esta semilla y corrige lo necesario».
- `_radar-externo`: «Investiga qué está funcionando ahora en LinkedIn para empresas de fitness».
- `_radar-interno`: «Busca incoherencias entre reglas, Skills y agentes».

No exigir una sintaxis rígida. Interpretar la petición y utilizar el agente que mejor corresponda.

## Encadenamiento

Un agente puede apoyarse en otro cuando la petición del usuario abarque varias fases.

Ejemplos:

- «Planifica noviembre y crea las semillas nuevas necesarias» → `00_planifica-contenido` + `01_crea-semilla`.
- «Crea una semilla y desarrolla LinkedIn e Instagram» → `01_crea-semilla` + `02_desarrolla-semilla`.
- «Revisa la newsletter y corrígela» → `06_revisa-contenido-newsletter` aplicando después las modificaciones necesarias.

No ejecutar fases adicionales por rutina. Si el usuario pide únicamente planificación, no crear semillas. Si pide únicamente una revisión, no rehacer contenido correcto sin motivo.

## Agentes transversales

### `_radar-externo`

Investiga el entorno exterior: plataformas, tendencias, formatos, referentes, cambios de canal y ejemplos públicos. Propone mejoras basadas en evidencia actual.

Por defecto **investiga y propone; no cambia las reglas automáticamente**.

### `_radar-interno`

Inspecciona el propio proyecto para detectar contradicciones, referencias rotas, duplicidades, reglas incompatibles, nomenclaturas antiguas o flujos incoherentes.

Está diseñado para ser genérico y reutilizable en otros proyectos con estructuras distintas.

Por defecto **audita y propone; no modifica archivos salvo petición expresa**.

## Flujo editorial numerado

### `00_planifica-contenido`

Planifica un calendario editorial y descubre los temas que merece la pena tratar según periodo, estacionalidad, eventos, campañas, necesidades del sector, contenido existente y huecos editoriales.

Integra la función de búsqueda de ideas. No existe un agente separado `busca-ideas`.

### `01_crea-semilla`

Convierte un tema validado o una oportunidad editorial en una nueva `semilla.md`.

### `02_desarrolla-semilla`

Desarrolla una semilla en todo o parte de sus piezas: blog, LinkedIn, Instagram, X y TikTok.

### `03_revisa-contenido`

Revisa y mejora semillas o piezas existentes, comprobando coherencia factual, editorial y de canal.

### `04_crea-semilla-newsletter`

Selecciona y jerarquiza entradas para definir la semilla de una nueva edición de newsletter.

### `05_desarrolla-semilla-newsletter`

Convierte una semilla de newsletter en la edición completa.

### `06_revisa-contenido-newsletter`

Revisa y mejora una semilla de newsletter o una edición ya redactada.

### `07_audita-editorial`

Analiza el conjunto de contenidos para detectar desequilibrios, repeticiones, huecos, infrautilización de semillas y oportunidades de mejora estratégica.

## Principios comunes

- No inventar capacidades, datos, clientes, resultados, eventos ni fuentes.
- No utilizar información técnica interna como argumento editorial.
- No crear una nueva semilla sin comprobar primero si el tema ya existe.
- No convertir todos los encargos en un flujo completo: ejecutar solo las fases necesarias.
- No duplicar en un agente las instrucciones detalladas de una Skill; enlazarla y utilizarla.
- Mantener los identificadores y numeraciones existentes.
- Utilizar información actual y fuentes recientes cuando una decisión dependa de fechas, tendencias, eventos o cambios de plataforma.
- Distinguir entre observación, inferencia y hecho confirmado.
- Si una decisión cambia el funcionamiento del Editor, actualizar el archivo canónico correspondiente y registrarla en `_reglas/decisiones-editoriales.md`.
