# Oráculo de Agendic

## Fuente autorizada

La fuente de verdad funcional para el Editor es:

- **Repositorio:** `bookgy/oraculo`
- **Ruta:** `entradas/entradas_confirmadas/`
- **Acceso:** solo lectura

Esta ruta contiene la información confirmada que puede utilizarse para crear semillas y contenidos editoriales.

## Reglas obligatorias

1. Consultar únicamente `bookgy/oraculo/entradas/entradas_confirmadas/` para afirmar cómo funciona Agendic.
2. No utilizar borradores, entradas pendientes, código fuente, bases de datos u otras fuentes como sustituto de una entrada confirmada.
3. No modificar nunca `bookgy/oraculo` desde las Skills de este repositorio.
4. Si la ruta confirmada no existe, no es accesible o no contiene información suficiente, detener la afirmación. No sustituirla silenciosamente por otra carpeta del Oráculo.
5. Si existe vocabulario funcional definido en el contenido confirmado, respetarlo.
6. Registrar en cada semilla la ruta concreta de la entrada o entradas del Oráculo utilizadas.

## Separación entre evidencia y comunicación

El Oráculo puede contener detalles técnicos utilizados para demostrar un comportamiento del producto. Esa evidencia puede servir para confirmar un hecho, pero nunca es material editorial.

No trasladar a semillas, entradas, newsletters o contenidos sociales:

- nombres de tablas o campos de base de datos;
- nombres de archivos o clases;
- código;
- endpoints;
- consultas SQL;
- arquitectura interna;
- identificadores técnicos;
- mecanismos de implementación que el cliente no necesita conocer.

Transformar siempre la información confirmada en lenguaje funcional y de negocio.

## Información insuficiente

No completar huecos mediante suposiciones.

Si falta información imprescindible para confirmar una afirmación, utilizar cuando sea necesario esta respuesta:

> Me falta información para confirmarlo. Contacta con Atención al Cliente.

La información no confirmada no debe incorporarse como hecho a una semilla.
