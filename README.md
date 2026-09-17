# Editor de Agendic

Repositorio editorial de Agendic. Reúne las fuentes autorizadas, las reglas comunes, los agentes invocables, las Skills y el contenido creado para los distintos canales.

## Estructura

```text
editor/
├── README.md
├── _fuentes/
│   └── oraculo.md
├── _reglas/
│   ├── contexto.md
│   ├── editorial.md
│   ├── guia-redaccion.md
│   └── decisiones-editoriales.md
├── _agentes/
│   ├── README.md
│   ├── _radar-externo.md
│   ├── _radar-interno.md
│   ├── 00_planifica-contenido.md
│   ├── 01_crea-semilla.md
│   ├── 02_desarrolla-semilla.md
│   ├── 03_revisa-contenido.md
│   ├── 04_crea-semilla-newsletter.md
│   ├── 05_desarrolla-semilla-newsletter.md
│   ├── 06_revisa-contenido-newsletter.md
│   └── 07_audita-editorial.md
├── _skills/
│   ├── entrada-semilla/
│   ├── entrada-blog/
│   ├── entrada-linkedin/
│   ├── entrada-instagram/
│   ├── entrada-x/
│   ├── entrada-tiktok/
│   ├── newsletter-semilla/
│   └── newsletter/
├── entradas-editor/
└── newsletters/
```

## Qué representa cada carpeta

- `_fuentes/`: define de dónde puede obtenerse información factual sobre Agendic.
- `_reglas/`: define el contexto, el criterio editorial, la forma de redactar y el registro de decisiones.
- `_agentes/`: define los trabajos invocables y cómo se coordinan reglas, fuentes y Skills para resolverlos.
- `_skills/`: contiene los procesos de ejecución especializados que utilizan los agentes o que pueden invocarse directamente.
- `entradas-editor/`: guarda cada tema editorial, su semilla y todos los contenidos derivados de ella.
- `newsletters/`: guarda cada edición de newsletter y su composición.

## Principio general

El flujo editorial es:

**planificación y descubrimiento → validación factual → semilla → piezas derivadas por canal → revisión y auditoría**

A partir de una misma semilla pueden crearse, de forma independiente:

- un blog;
- una o varias publicaciones de LinkedIn;
- una o varias publicaciones de Instagram;
- una o varias publicaciones para X;
- una o varias piezas de TikTok;
- contenidos que después puedan formar parte de una newsletter.

El blog no es un paso obligatorio previo para crear los demás canales. Todas las piezas derivan de la misma semilla y comparten sus hechos, límites y condiciones.

La información factual sobre el producto procede únicamente de la fuente definida en `_fuentes/oraculo.md`.

Las Skills pueden leer el Oráculo, pero nunca modificarlo.

## Agentes y Skills

Los agentes son la capa de **orquestación** del Editor.

Interpretan encargos como planificar un mes, crear una semilla, desarrollar varios canales, revisar contenido o auditar el conjunto. Pueden coordinar una o varias Skills según el alcance solicitado.

Las Skills son la capa de **ejecución especializada**. Definen cómo crear correctamente una semilla, un blog, un LinkedIn, una pieza de Instagram, X, TikTok o una newsletter.

Regla de diseño:

**el agente decide el flujo; la Skill ejecuta la tarea concreta; las reglas y las fuentes mantienen la coherencia y la verdad.**

Los dos radares de `_agentes/` son transversales:

- `_radar-externo`: investiga el entorno, los canales, los formatos y las prácticas actuales y propone mejoras;
- `_radar-interno`: inspecciona la coherencia del propio proyecto y está diseñado para poder reutilizarse en otros repositorios.

El flujo numerado comienza en `00_planifica-contenido`. Este agente incluye también el descubrimiento de nuevas ideas: no existe un agente independiente `busca-ideas`.

Consultar `_agentes/README.md` para la jerarquía, invocación y encadenamiento de agentes.

## Fuente única de verdad del Editor

`bookgy/editor` es la fuente única de verdad del sistema editorial.

Una regla, corrección, preferencia o aprendizaje que cambie la forma de trabajar no puede quedar únicamente en una conversación, memoria externa, ZIP, documento local o copia de una Skill.

Cuando exista feedback editorial:

1. identificar su alcance: global, canal, Skill, semilla o contenido concreto;
2. modificar el archivo canónico correspondiente dentro del repositorio;
3. registrar la decisión en `_reglas/decisiones-editoriales.md`;
4. indicar allí qué archivos se han visto afectados;
5. si una decisión sustituye a otra anterior, dejar trazabilidad de la sustitución.

El registro de decisiones conserva el historial y la razón del cambio. La regla operativa vigente debe quedar también integrada en el archivo que realmente utiliza el Editor: `contexto.md`, `editorial.md`, `guia-redaccion.md`, una Skill o la pieza concreta que corresponda.

De esta forma, una nueva conversación o una nueva ejecución puede reconstruir el criterio editorial únicamente leyendo el repositorio.

## Identificación de entradas

Cada tema se guarda dentro de `entradas-editor/` en una carpeta con este formato:

`AAAA-MM-NNN-contenido`

Ejemplo:

`entradas-editor/2026-09-001-cupones-promociones`

Su identificador permanente es:

`2026-09-001`

El contador `NNN` se reinicia cada mes.

## Contenidos por canal

Una misma entrada puede producir tantos contenidos como sea necesario:

```text
entradas-editor/2026-09-001-cupones-promociones/
├── semilla.md
├── blog.md
├── linkedin-001.md
├── linkedin-002.md
├── instagram-001.md
├── instagram-002.md
├── x-001.md
└── tiktok-001.md
```

La numeración es independiente para cada canal. `linkedin-001.md` no tiene relación obligatoria con `instagram-001.md`.

`blog.md` es la pieza desarrollada para formato blog. Puede existir o no; los demás canales no dependen de ella.

Todos los contenidos de una carpeta derivan de la misma semilla y deben mantener los mismos hechos, límites y condiciones funcionales.

## Newsletters

Cada newsletter tiene su propia semilla porque es una composición editorial de una o varias entradas.

Formato:

`newsletters/AAAA-MM-NNN/`

Ejemplo:

```text
newsletters/2026-09-001/
├── semilla.md
└── newsletter.md
```

Una newsletter puede utilizar entradas creadas en cualquier mes desde `entradas-editor/`.

## Reglas esenciales

1. Dirigir el contenido a empresas.
2. Partir de un dolor, necesidad, oportunidad o resultado, no de la funcionalidad por sí sola.
3. Usar solo hechos confirmados por la fuente autorizada.
4. No inventar capacidades, métricas, clientes, resultados, rutas o disponibilidad.
5. No trasladar al contenido editorial información técnica interna.
6. Escribir el contenido base de forma genérica; adaptar vocabulario y ejemplos por sector cuando aporte valor.
7. Mantener una única idea principal por semilla.
8. Reutilizar una semilla para generar nuevos contenidos y creatividades sin duplicarla.
9. Registrar en GitHub cualquier decisión editorial que modifique criterios, procesos o piezas.
