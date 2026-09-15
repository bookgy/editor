---
name: entrada-linkedin
description: "Crear nuevas publicaciones de LinkedIn para una entrada editorial de Agendic. Usar cuando el usuario quiera reutilizar una semilla existente en LinkedIn con uno o varios ángulos, generando el siguiente archivo linkedin-NNN.md sin duplicar innecesariamente publicaciones anteriores."
---

# Entrada LinkedIn

Crear una publicación nativa de LinkedIn derivada de una semilla existente.

## Referencias obligatorias

Leer:

- `semilla.md` de la entrada;
- `entrada.md` si existe;
- los `linkedin-NNN.md` existentes de esa carpeta;
- `_referencias/contexto.md`;
- `_referencias/guia-redaccion.md`.

## Flujo

1. Revisar qué contenidos de LinkedIn existen ya para evitar repetir el mismo enfoque.
2. Elegir un ángulo útil y coherente con la semilla.
3. Abrir con una observación, problema o situación reconocible.
4. Desarrollar por qué importa en la gestión de una empresa.
5. Introducir la respuesta de Agendic de forma natural.
6. Incluir un ejemplo o consecuencia concreta cuando aporte valor.
7. Cerrar con una idea, pregunta o CTA coherente.
8. Asignar el siguiente número libre de LinkedIn.
9. Guardar como `linkedin-NNN.md`.

## Reglas

- No hacer una versión recortada de `entrada.md`.
- No usar tono de anuncio corporativo genérico.
- No inventar datos, resultados o casos reales.
- Mantener los hechos y límites de la semilla.
- Cada nuevo archivo debe aportar un ángulo, ejemplo o creatividad suficientemente distinto de los anteriores.

## Metadatos

Incluir al inicio:

```yaml
semilla_id: AAAA-MM-NNN
canal: linkedin
contenido: NNN
estado: borrador
```
