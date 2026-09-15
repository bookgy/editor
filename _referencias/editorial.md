# Criterio editorial

## Misión

Cada pieza debe conseguir que una empresa descubra una capacidad útil de Agendic, entienda para qué le sirve y tenga ganas de utilizarla.

No comunicar una funcionalidad por el simple hecho de existir. Partir de un dolor, una necesidad, una fricción, una oportunidad o un resultado deseado por la empresa.

## Modelo

La **semilla** es la unidad maestra de cada tema editorial.

Una semilla reúne:

- los hechos funcionales confirmados;
- el problema que merece comunicar;
- la utilidad para la empresa;
- un ejemplo práctico;
- los límites o condiciones relevantes;
- la idea principal;
- el siguiente paso.

A partir de una semilla pueden generarse:

- una `entrada.md` principal;
- N contenidos para LinkedIn;
- N contenidos para Instagram;
- N contenidos para X;
- N contenidos para TikTok;
- participación en una o varias newsletters.

Las piezas derivadas no son simples versiones recortadas. Comparten hechos, pero adaptan apertura, profundidad, ritmo, ejemplo y llamada a la acción al canal.

## Qué puede originar una semilla

- nueva funcionalidad;
- mejora de una funcionalidad existente;
- capacidad existente poco conocida;
- consejo práctico;
- caso de uso;
- cambio relevante;
- contexto que modifique la forma de trabajar de una empresa.

No limitar el calendario editorial a novedades recientes.

## Regla de selección

Antes de crear una semilla comprobar:

1. que existe información confirmada suficiente;
2. que existe un problema, necesidad, oportunidad o resultado claro;
3. que puede explicarse un beneficio práctico;
4. que el tema puede ser entendido por una empresa sin conocer detalles técnicos.

Si no existe un motivo claro para que una empresa se interese por el tema, no forzar la comunicación.

## Identificación de una entrada

Formato de carpeta:

`AAAA-MM-NNN-contenido`

Ejemplo:

`2026-09-001-cupones-promociones`

Identificador permanente:

`AAAA-MM-NNN`

Ejemplo:

`2026-09-001`

El texto descriptivo de la carpeta puede ajustarse mientras se está creando la entrada, pero el identificador no debe cambiar una vez utilizado.

## Estructura de `semilla.md`

Usar esta estructura como base. Mantenerla concisa y completar solo lo que aporte información útil.

```markdown
# [Nombre interno]

## Identificación
- semilla_id: AAAA-MM-NNN
- fecha: AAAA-MM-DD
- estado: borrador | validada | publicada | archivada
- tipo: nueva funcionalidad | mejora | funcionalidad existente | consejo | caso de uso | cambio relevante | otro
- ámbito: General | Fitness | Pets | Auto | Boat | Otro

## Fuente
- entradas del Oráculo utilizadas:
  - ruta exacta

## Hechos confirmados
- ...

## Condiciones y matices
- ...

## Dolor o necesidad
- dolor principal:
- situación reconocible:
- consecuencia:

## Propuesta de valor
- capacidad de Agendic:
- beneficio principal:
- antes:
- después:

## Público
- tipo: empresas
- sector: general por defecto
- sectores especialmente relacionados: opcional

## Ejemplo práctico
- situación:
- uso de Agendic:
- resultado esperado:

## Mensaje editorial
- idea principal:
- ángulo principal:
- por qué merece comunicarse:

## Acción
- siguiente paso:
- CTA posibles:

## Recursos editoriales
- enlaces, capturas, vídeos o materiales disponibles:
```

## Reglas de la semilla

- Mantener un único dolor principal y una única idea principal.
- Incluir solo hechos confirmados.
- Expresar condiciones desde la perspectiva del usuario, no desde la implementación.
- El ejemplo puede ser ilustrativo, pero debe usar exclusivamente capacidades confirmadas.
- No inventar resultados reales, clientes, métricas ni testimonios.
- Si aparecen dos historias independientes, crear dos semillas.

## Estados

- `borrador`: semilla creada pero todavía susceptible de revisión editorial.
- `validada`: enfoque editorial revisado y aprobado.
- `publicada`: existe al menos una pieza publicada basada en ella.
- `archivada`: ya no debe utilizarse para nuevos contenidos salvo revisión expresa.

La fuente confirmada valida los hechos del producto; no convierte automáticamente una semilla editorial en `validada`.

## Entrada principal

`entrada.md` es la pieza completa y canónica del tema: **explica y convence**.

Estructura recomendada:

1. titular orientado al problema o resultado;
2. situación reconocible;
3. respuesta de Agendic;
4. qué cambia para la empresa;
5. ejemplo práctico;
6. cómo empezar, solo si está confirmado y aporta valor;
7. CTA.

No fijar una longitud rígida.

## Contenidos por canal

Formato:

`canal-NNN.md`

Ejemplos:

- `linkedin-001.md`
- `linkedin-002.md`
- `instagram-001.md`
- `x-001.md`
- `tiktok-001.md`

La numeración empieza en `001` y es independiente por canal.

Cada archivo representa una publicación o concepto creativo autónomo derivado de la misma semilla.

Metadatos mínimos recomendados:

```yaml
semilla_id: AAAA-MM-NNN
canal: linkedin | instagram | x | tiktok
contenido: NNN
estado: borrador | validado | publicado | archivado
```

## Newsletters

Una newsletter es una composición editorial de una o varias entradas y tiene su propia semilla.

Formato:

`newsletters/AAAA-MM-NNN/`

Su `semilla.md` debe definir como mínimo:

- newsletter_id;
- fecha;
- estado;
- objetivo de la edición;
- entrada protagonista;
- entradas secundarias;
- orden;
- hilo editorial;
- CTA principal.

Una newsletter puede recuperar entradas creadas en meses anteriores.

No concatenar entradas sin criterio. Editar la selección para que la edición tenga una idea y una jerarquía claras.

## Composición recomendada de una newsletter

Por defecto:

1. una historia protagonista;
2. entre una y tres historias secundarias cuando existan temas suficientes;
3. mejoras menores agrupadas cuando tenga sentido;
4. apertura breve centrada en valor;
5. CTA principal;
6. asunto y preheader al final del proceso.

No tratar esta pauta como una obligación numérica.
