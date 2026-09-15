---
name: entrada-x
description: "Crear nuevas publicaciones para X a partir de una semilla editorial de Agendic. Usar cuando el usuario quiera comunicar una idea de una entrada en X de forma breve, específica y nativa del canal, guardando cada nueva pieza como x-NNN.md."
---

# Entrada X

Crear una publicación para X derivada de una semilla existente.

## Referencias obligatorias

Leer:

- `semilla.md`;
- `entrada.md` si existe;
- los `x-NNN.md` existentes;
- `_referencias/contexto.md`;
- `_referencias/guia-redaccion.md`.

## Flujo

1. Revisar qué se ha publicado ya desde esa semilla.
2. Elegir una idea concreta y suficientemente distinta.
3. Expresarla de forma directa y específica.
4. Añadir ejemplo, dato funcional confirmado o CTA solo si mejora el mensaje.
5. Proponer apoyo visual cuando tenga sentido.
6. Crear hilo únicamente si una sola publicación no permite comunicar bien la idea.
7. Asignar el siguiente número libre de X.
8. Guardar como `x-NNN.md`.

## Reglas

- Evitar relleno y frases genéricas.
- No sacrificar precisión por brevedad.
- No introducir hechos no presentes en la semilla sin verificarlos.
- No utilizar información técnica interna.

## Metadatos

```yaml
semilla_id: AAAA-MM-NNN
canal: x
contenido: NNN
estado: borrador
```
