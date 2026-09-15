---
name: newsletter-semilla
description: "Crear la semilla de una nueva newsletter de Agendic seleccionando y jerarquizando entradas editoriales existentes. Usar cuando el usuario quiera preparar una edición de newsletter, decidir qué historias incluir, cuál será la protagonista y qué hilo editorial conecta la edición antes de redactarla."
---

# Newsletter Semilla

Crear la composición editorial de una nueva newsletter.

## Referencias obligatorias

Leer en `bookgy/editor`:

- `_referencias/contexto.md`;
- `_referencias/editorial.md`;
- `_referencias/guia-redaccion.md`;
- las semillas y entradas candidatas de `entradas/`.

## Flujo

1. Identificar el objetivo de la edición.
2. Revisar entradas existentes relevantes, aunque sean de meses anteriores.
3. Seleccionar solo historias que aporten valor suficiente.
4. Elegir una entrada protagonista.
5. Elegir historias secundarias y agrupar temas menores cuando tenga sentido.
6. Definir el orden y el hilo editorial de la edición.
7. Definir el CTA principal.
8. Calcular el siguiente `newsletter_id` disponible del mes.
9. Crear `newsletters/AAAA-MM-NNN/semilla.md`.

## Estructura mínima

```markdown
# Newsletter AAAA-MM-NNN

- newsletter_id: AAAA-MM-NNN
- fecha: AAAA-MM-DD
- estado: borrador

## Objetivo
...

## Entrada protagonista
- semilla_id: ...
- motivo: ...

## Entradas secundarias
- semilla_id: ...
- función en la edición: ...

## Orden
1. ...

## Hilo editorial
...

## CTA principal
...
```

## Reglas

- No convertir la newsletter en un changelog.
- No incluir temas solo porque sean nuevos.
- Puede combinar novedades, mejoras, capacidades poco conocidas, consejos y casos de uso.
- Una edición puede reutilizar entradas antiguas si son relevantes.
- Crear inicialmente con `estado: borrador` salvo indicación expresa.
