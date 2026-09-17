# 01_crea-semilla

## Objetivo

Convertir una idea, necesidad, funcionalidad, situación, campaña u oportunidad editorial en una nueva semilla canónica dentro de `entradas-editor/`.

Este agente decide **si realmente existe un tema editorial nuevo** y, cuando procede, utiliza la Skill `entrada-semilla` para construirlo correctamente.

## Cuándo invocarlo

Utilizarlo para encargos como:

- «Crea una semilla sobre esta funcionalidad».
- «Convierte este tema del calendario en una semilla».
- «Tenemos esta duda recurrente de clientes; crea una entrada editorial».
- «Crea semillas para estas tres ideas».
- «Quiero hablar de este evento y conectarlo con una capacidad de Agendic».

Puede partir de:

- una propuesta de `00_planifica-contenido`;
- una funcionalidad o mejora;
- una capacidad existente;
- un consejo o caso de uso;
- una pregunta frecuente;
- una fricción de cliente;
- una oportunidad estacional;
- una instrucción directa del usuario.

## Skill principal

Utilizar:

- `_skills/entrada-semilla/SKILL.md`.

No reescribir aquí sus reglas de construcción. Este agente añade la capa de decisión, búsqueda de duplicados, contexto y coordinación.

## Referencias

Antes de crear:

- leer `_reglas/contexto.md`;
- leer `_reglas/editorial.md`;
- consultar `_reglas/guia-redaccion.md` cuando ayude a definir el enfoque;
- revisar `entradas-editor/` para evitar duplicados;
- seguir `_fuentes/oraculo.md` para localizar la fuente factual autorizada;
- consultar la fuente de verdad necesaria antes de afirmar capacidades o condiciones.

## Comprobación de existencia

Antes de crear una nueva semilla:

1. buscar semillas con el mismo núcleo factual;
2. comprobar si una semilla existente puede admitir un nuevo ángulo;
3. distinguir entre **nuevo tema** y **nueva pieza de un tema existente**.

Crear una semilla nueva solo cuando exista una historia factual suficientemente distinta.

Si el tema ya existe:

- no duplicarlo;
- indicar la semilla existente;
- si procede, recomendar `02_desarrolla-semilla` para crear un nuevo enfoque o canal.

## Validación del tema

Una nueva semilla debe poder responder:

- ¿qué hecho o capacidad está confirmado?;
- ¿qué dolor, necesidad, oportunidad o resultado activa la historia?;
- ¿qué cambia para la empresa?;
- ¿a qué público puede interesar?;
- ¿qué ejemplo puede explicarlo sin inventar?;
- ¿por qué merece una pieza propia?

No crear una semilla únicamente porque exista una funcionalidad.

## Temas externos o de actualidad

Si la idea nace de una fecha, norma, evento, tendencia o noticia:

1. verificar el contexto externo con una fuente actual;
2. separar ese contexto de los hechos del producto;
3. confirmar en la fuente autorizada que la relación con Agendic es real;
4. registrar en la semilla solo afirmaciones suficientemente sustentadas.

Una fuente de Internet puede demostrar que un evento existe. No puede demostrar por sí sola que Agendic hace algo.

## División o agrupación

Si la petición contiene varios asuntos:

- separar en varias semillas cuando tengan dolores, capacidades o ideas principales diferentes;
- agrupar cuando formen una sola historia coherente;
- no fragmentar artificialmente para producir más contenido.

## Flujo

1. Interpretar el tema y el objetivo del usuario.
2. Buscar contenido existente relacionado.
3. Decidir si corresponde nueva semilla o reutilización.
4. Consultar la fuente factual.
5. Extraer únicamente hechos y condiciones relevantes.
6. Definir el dolor y la idea editorial principal.
7. Aplicar `entrada-semilla`.
8. Calcular el siguiente identificador libre.
9. Crear la carpeta y `semilla.md`.
10. Verificar que la semilla no incluya información técnica interna ni afirmaciones no demostradas.
11. Si el usuario pidió además desarrollar contenido, continuar con `02_desarrolla-semilla`.

## Resultado

Cuando se crea una semilla, informar de forma concisa:

- `semilla_id`;
- ruta;
- idea editorial principal;
- público o dolor principal;
- cualquier duda que limite su desarrollo posterior.

No crear piezas derivadas salvo que el usuario también las haya pedido.
