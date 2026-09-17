# 04_crea-semilla-newsletter

## Objetivo

Crear la **semilla de una nueva edición de newsletter**: decidir qué historias contiene, cuál es protagonista, qué orden tienen, qué hilo las conecta y qué objetivo persigue la edición.

No redactar todavía la newsletter completa salvo que el usuario pida también desarrollar la edición.

## Cuándo invocarlo

Utilizarlo para encargos como:

- «Prepara la newsletter de octubre».
- «Crea una semilla de newsletter con los mejores temas recientes».
- «Quiero una newsletter sobre vuelta a la rutina».
- «Selecciona tres historias y ordénalas para una edición».
- «Monta la siguiente newsletter».

## Skill principal

Utilizar:

- `_skills/newsletter-semilla/SKILL.md`.

Este agente añade contexto de selección, periodo, objetivo y coordinación; la Skill define la creación concreta de la semilla.

## Referencias

Leer:

- `_reglas/contexto.md`;
- `_reglas/editorial.md`;
- `_reglas/guia-redaccion.md`;
- las semillas candidatas de `entradas-editor/`;
- sus piezas cuando ayuden a valorar madurez o enfoque;
- newsletters anteriores para evitar repetición;
- un calendario de `00_planifica-contenido` si el usuario lo aporta o la edición forma parte de ese plan.

## Selección de historias

No limitarse a «lo más nuevo».

Una newsletter puede recuperar:

- semillas recientes;
- capacidades antiguas todavía útiles;
- contenidos que encajan especialmente bien con el momento;
- consejos;
- casos de uso;
- novedades;
- varias pequeñas historias agrupadas.

Cada historia seleccionada debe tener una función en la edición.

## Protagonista

Elegir una protagonista cuando exista un tema con suficiente valor.

Valorar:

- utilidad;
- oportunidad temporal;
- relevancia para la audiencia;
- profundidad disponible;
- capacidad de sostener el hilo de la edición.

No convertir automáticamente la novedad de producto más reciente en protagonista.

## Hilo editorial

La newsletter debe poder explicarse en una frase.

Evitar ediciones que sean simplemente:

> estas son las cosas que hemos publicado últimamente.

Buscar una relación útil entre las historias: momento de negocio, problema compartido, objetivo, etapa, aprendizaje o campaña.

## Flujo

1. Definir periodo, audiencia y objetivo de la edición.
2. Revisar newsletters anteriores.
3. Revisar entradas candidatas, incluso de meses anteriores.
4. Seleccionar únicamente historias con función clara.
5. Elegir protagonista.
6. Ordenar secundarias.
7. Agrupar asuntos menores cuando ayude.
8. Definir hilo editorial.
9. Definir CTA principal.
10. Ejecutar `newsletter-semilla`.
11. Crear `newsletters/AAAA-MM-NNN/semilla.md`.
12. Si el usuario también pide redactar, continuar con `05_desarrolla-semilla-newsletter`.

## Qué no hace por defecto

- No redacta el cuerpo completo.
- No crea nuevas semillas de entradas para rellenar la edición.
- No fuerza una cantidad fija de historias.
- No concatena piezas existentes.
- No incluye temas solo porque estén disponibles.

Si faltan historias para sostener la edición, indicarlo. Si el usuario pide resolverlo de extremo a extremo, puede encadenar `00_planifica-contenido` y `01_crea-semilla`.
