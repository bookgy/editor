# 05_desarrolla-semilla-newsletter

## Objetivo

Convertir una semilla de newsletter ya definida en una edición completa, coherente y lista para revisión.

La semilla de newsletter fija la selección y jerarquía. Este agente desarrolla la escritura sin alterar arbitrariamente esa arquitectura.

## Cuándo invocarlo

Utilizarlo para encargos como:

- «Desarrolla la newsletter 2026-10-001».
- «Redacta la edición a partir de esta semilla».
- «Crea asunto, preheader y cuerpo».
- «Termina la newsletter que ya hemos planificado».

## Skill principal

Utilizar:

- `_skills/newsletter/SKILL.md`.

## Referencias

Leer:

- `newsletters/AAAA-MM-NNN/semilla.md`;
- las `semilla.md` de todas las entradas seleccionadas;
- los blogs o piezas derivadas cuando aporten contexto;
- `_reglas/contexto.md`;
- `_reglas/editorial.md`;
- `_reglas/guia-redaccion.md`;
- newsletters anteriores cuando ayude a evitar estructuras, asuntos o cierres repetidos.

## Fidelidad a la semilla de newsletter

Respetar:

- objetivo;
- destinatario;
- protagonista;
- historias seleccionadas;
- orden;
- hilo editorial;
- CTA principal.

Si durante el desarrollo se detecta que una historia no encaja o existe una contradicción importante, no ocultarlo con redacción. Revisar primero la semilla de newsletter cuando el cambio afecte a su arquitectura.

## Desarrollo

Construir la edición como un todo:

- asunto;
- preheader;
- apertura;
- historia protagonista;
- historias secundarias;
- transiciones cuando sean necesarias;
- CTA principal;
- CTA secundarios solo si aportan valor;
- cierre.

No concatenar blogs o posts.

Cada historia debe adaptarse a correo y ocupar el espacio proporcional a su función.

## Asunto y preheader

Redactarlos después de tener claro el cuerpo.

Deben:

- representar el valor real de la edición;
- complementarse;
- evitar clickbait;
- evitar promesas que el cuerpo no cumple;
- ser suficientemente específicos.

Si el usuario pide alternativas, crear opciones realmente diferentes, no variaciones mínimas.

## Flujo

1. Leer la semilla de newsletter.
2. Validar que todas las entradas seleccionadas existen.
3. Leer las fuentes editoriales necesarias.
4. Redactar la apertura.
5. Desarrollar la protagonista.
6. Adaptar y jerarquizar secundarias.
7. Revisar ritmo y escaneabilidad.
8. Redactar CTA.
9. Crear asunto y preheader.
10. Aplicar `newsletter`.
11. Guardar `newsletter.md` en la carpeta de la edición.
12. Realizar una revisión final de coherencia factual.

## Resultado

Indicar:

- newsletter desarrollada;
- ruta de `newsletter.md`;
- asunto y preheader elegidos;
- cualquier cambio de arquitectura que haya quedado pendiente de validar.

No modificar semillas de entradas para hacer que encajen mejor con el correo.
