# Editor de Agendic

Repositorio editorial de Agendic. Reúne las fuentes autorizadas, las referencias comunes, las Skills y el contenido creado para los distintos canales.

## Estructura

```text
editor/
├── README.md
├── _fuentes/
│   └── oraculo.md
├── _referencias/
│   ├── contexto.md
│   ├── editorial.md
│   └── guia-redaccion.md
├── _skills/
│   ├── entrada-semilla/
│   ├── entrada/
│   ├── entrada-linkedin/
│   ├── entrada-instagram/
│   ├── entrada-x/
│   ├── entrada-tiktok/
│   ├── newsletter-semilla/
│   └── newsletter/
├── entradas/
└── newsletters/
```

## Qué representa cada carpeta

- `_fuentes/`: define de dónde puede obtenerse información factual sobre Agendic.
- `_referencias/`: define el contexto, el criterio editorial y la forma de redactar.
- `_skills/`: contiene los procesos que puede ejecutar la IA.
- `entradas/`: guarda cada tema editorial y todos los contenidos derivados de él.
- `newsletters/`: guarda cada edición de newsletter y su composición.

## Principio general

El flujo editorial es:

**fuente confirmada → semilla → entrada principal → contenidos por canal → newsletter cuando corresponda**

La información factual sobre el producto procede únicamente de la fuente definida en `_fuentes/oraculo.md`.

Las Skills pueden leer el Oráculo, pero nunca modificarlo.

## Identificación de entradas

Cada tema se guarda en una carpeta con este formato:

`AAAA-MM-NNN-contenido`

Ejemplo:

`2026-09-001-cupones-promociones`

Su identificador permanente es:

`2026-09-001`

El contador `NNN` se reinicia cada mes.

## Contenidos por canal

Una misma entrada puede producir tantos contenidos como sea necesario:

```text
2026-09-001-cupones-promociones/
├── semilla.md
├── entrada.md
├── linkedin-001.md
├── linkedin-002.md
├── instagram-001.md
├── instagram-002.md
├── x-001.md
└── tiktok-001.md
```

La numeración es independiente para cada canal. `linkedin-001.md` no tiene relación obligatoria con `instagram-001.md`.

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

Una newsletter puede utilizar entradas creadas en cualquier mes.

## Reglas esenciales

1. Dirigir el contenido a empresas.
2. Partir de un dolor, necesidad, oportunidad o resultado, no de la funcionalidad por sí sola.
3. Usar solo hechos confirmados por la fuente autorizada.
4. No inventar capacidades, métricas, clientes, resultados, rutas o disponibilidad.
5. No trasladar al contenido editorial información técnica interna.
6. Escribir el contenido base de forma genérica; adaptar vocabulario y ejemplos por sector cuando aporte valor.
7. Mantener una única idea principal por semilla.
8. Reutilizar una semilla para generar nuevos contenidos y creatividades sin duplicarla.
