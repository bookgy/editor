---
name: entrada-semilla
description: "Crear una nueva semilla editorial de Agendic a partir de información funcional confirmada. Usar cuando el usuario quiera convertir una funcionalidad, mejora, consejo, caso de uso o cambio relevante en un nuevo tema editorial dentro de bookgy/editor/entradas. Consultar bookgy/oraculo únicamente como fuente de verdad y no modificarlo."
---

# Entrada Semilla

Crear la semilla maestra de un nuevo tema editorial.

## Referencias obligatorias

Antes de trabajar, leer en `bookgy/editor`:

- `_fuentes/oraculo.md`
- `_referencias/contexto.md`
- `_referencias/editorial.md`
- `_referencias/guia-redaccion.md`

## Flujo

1. Identificar el tema que el usuario quiere comunicar.
2. Consultar únicamente la fuente confirmada definida en `_fuentes/oraculo.md`.
3. Extraer hechos funcionales relevantes y eliminar cualquier detalle técnico interno.
4. Identificar un único dolor, necesidad, oportunidad o resultado principal.
5. Explicar la capacidad de Agendic y su beneficio para una empresa.
6. Crear un ejemplo práctico compatible con los hechos confirmados.
7. Definir una única idea editorial principal.
8. Determinar `ámbito`, usando `General` por defecto.
9. Calcular el siguiente `semilla_id` disponible del mes en `entradas/`.
10. Crear `entradas/AAAA-MM-NNN-contenido/semilla.md` siguiendo la estructura de `_referencias/editorial.md`.

## Numeración

Usar `AAAA-MM-NNN`.

Reiniciar `NNN` cada mes y utilizar el siguiente número libre existente en `bookgy/editor/entradas/`.

No reutilizar un identificador ya existente.

## Reglas

- Crear inicialmente la semilla con `estado: borrador` salvo indicación expresa.
- Registrar la ruta exacta de las entradas del Oráculo utilizadas.
- No introducir información no confirmada.
- No mencionar código, BBDD, archivos, endpoints, clases o arquitectura.
- No convertir una funcionalidad en historia si no existe un valor reconocible para una empresa.
- Si el tema contiene dos historias claramente independientes, separarlas en dos semillas.
- Si falta información imprescindible, no inventarla. Indicar: `Me falta información para confirmarlo. Contacta con Atención al Cliente.`

## Resultado

Guardar la semilla en GitHub cuando el usuario haya pedido crearla o trabajar directamente en el repositorio.

Al terminar, indicar el `semilla_id`, la carpeta creada y la idea editorial principal.
