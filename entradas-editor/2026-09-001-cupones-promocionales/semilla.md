# Cupones promocionales

## Identificación
- semilla_id: 2026-09-001
- fecha: 2026-09-16
- estado: borrador
- tipo: funcionalidad existente
- ámbito: General

## Fuente
- rutas exactas del Oráculo utilizadas:
  - `entradas/entradas_confirmadas/marketing/00-mapa.md`

## Hechos confirmados
- Agendic permite crear promociones y descuentos desde **Marketing → Herramientas Comerciales → Promociones y Descuentos**.
- Una promoción define las condiciones del descuento.
- Un cupón es un código asociado a una promoción.
- La promoción puede definir a quién afecta.
- Puede aplicarse a todos los clientes o restringirse mediante criterios como cliente concreto, tipo de cliente, cuota, curso/actividad, cargo programado o grupo.
- La promoción puede definir a qué conceptos afecta, entre ellos Agendas de Servicios, Agendas de Instalaciones/Clases y Artículos de Tienda.
- El descuento puede configurarse como porcentaje sobre el precio original, importe a restar o precio fijo que sustituye al precio original.
- La promoción puede limitarse a un periodo mediante fecha de inicio y fecha de fin.
- Cada cupón puede activarse o desactivarse de forma independiente.
- Para poder utilizar un código deben estar activos tanto el cupón como la promoción asociada.

## Condiciones y matices
- El código del cupón no contiene por sí mismo las reglas del descuento: porcentaje o importe, fechas, destinatarios y conceptos afectados pertenecen a la promoción asociada.
- La vigencia del cupón ordinario depende de las fechas de la promoción; el cupón no tiene fechas propias.
- No existe una opción genérica confirmada de máximo de usos para un cupón ordinario.
- Si un cupón ya se ha utilizado, no puede eliminarse mediante el flujo estándar; puede desactivarse para impedir nuevos usos.
- No generalizar al cupón ordinario comportamientos propios de Tarjetas Regalo u otros flujos.

## Dolor o necesidad
- problema principal: lanzar descuentos sin unas reglas claras puede obligar al equipo a comprobar manualmente cuándo, a quién y sobre qué debe aplicarse cada oferta.
- situación reconocible: una empresa quiere hacer una campaña promocional para un periodo, un grupo de clientes o determinados servicios, pero no quiere aplicar el descuento de forma indiscriminada.
- consecuencia: más comprobaciones manuales, más posibilidades de aplicar una condición incorrecta y menos control sobre cómo se utiliza la promoción.

## Propuesta de valor
- capacidad de Agendic: crear promociones con condiciones definidas y asociarles uno o varios códigos de cupón cuando se quiera comunicar o exigir un código concreto.
- cambio que permite: centralizar las reglas de la promoción y decidir a quién, a qué y durante qué periodo se aplica.
- beneficio principal: lanzar acciones promocionales con más control y menos comprobaciones manuales.
- antes: el equipo tiene que recordar o revisar manualmente las condiciones de una oferta antes de aplicarla.
- después: las condiciones quedan configuradas en la promoción y el cupón actúa como código para acceder a ella cuando corresponda.

## Público
- tipo: empresas
- sector: general
- sectores especialmente relacionados: negocios que trabajen con servicios, clases o instalaciones, tienda o grupos de clientes y quieran realizar acciones promocionales.

## Ejemplo práctico
- tipo: ilustrativo
- situación: una empresa quiere lanzar durante una semana una campaña con el código `VERANO20` para ofrecer un 20 % de descuento sobre determinados servicios.
- uso de Agendic: crea una promoción, define el 20 % de descuento, selecciona los conceptos y destinatarios a los que afecta, limita su vigencia y añade el código `VERANO20` en la sección de Cupones.
- resultado esperable: la empresa puede comunicar un código sencillo mientras mantiene centralizadas en Agendic las condiciones reales de la promoción.

## Mensaje editorial
- idea principal: un cupón no tiene por qué ser un descuento aplicado sin control; en Agendic puedes definir primero las condiciones de la promoción y utilizar después un código para comunicarla o activarla cuando corresponda.
- ángulo principal: control y flexibilidad en campañas promocionales.
- por qué merece comunicarse: es una capacidad práctica de marketing que puede ayudar a empresas que todavía gestionan descuentos de forma manual o demasiado genérica y permite mostrar que Agendic conecta la acción comercial con reglas concretas de negocio.
- posibles ángulos secundarios:
  - campañas dirigidas a grupos concretos de clientes;
  - promociones limitadas a determinados servicios, clases o productos;
  - campañas estacionales con fecha de inicio y fin;
  - diferencia entre promoción y cupón;
  - desactivar un cupón sin perder el histórico cuando ya se ha utilizado.

## Acción
- siguiente paso útil: revisar **Marketing → Herramientas Comerciales → Promociones y Descuentos** y valorar una primera campaña con condiciones concretas.
- CTA posibles:
  - `Descubre cómo funcionan las promociones y cupones.`
  - `Revisa qué promociones puedes crear en Agendic.`
  - `Configura una promoción y crea el código que quieras comunicar.`

## Recursos editoriales
- captura de la pantalla **Promociones y Descuentos**, si se dispone de una versión actualizada y sin datos sensibles.
- ejemplo visual con el código `VERANO20` y las condiciones de la promoción.
- posible creatividad antes/después: “descuento manual” frente a “promoción con reglas definidas”.

## Notas
- Mantener siempre clara la diferencia entre promoción y cupón: la promoción contiene las reglas; el cupón es el código asociado.
- No afirmar que existe un límite genérico de usos por cupón.
- No trasladar a contenidos editoriales ninguna evidencia técnica interna utilizada por el Oráculo para validar el comportamiento.
