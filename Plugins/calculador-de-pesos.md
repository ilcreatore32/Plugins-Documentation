# Calculador de Pesos

> Encargado de hacer las conversiones entre distintas unidades con los campos: Toneladas, Kilogramos, Libras, Metros Cúbicos, Pies Cúbicos y  Centimetros Cúbicos

- Summary
    - [Ejecución](#ejecución)
    - [Ejemplo](#ejemplo)
    - [Campos](#campos)
    - [Ubicación](#ubicación)

## Ejecución

Para utilizar el plugin basta con rellenar 1 o 2 campos de dimensiones, los cuales son agrupados en:
- Toneladas, Kilogramos y Libras
- Metros Cúbicos, Pies Cúbicos y  Centimetros Cúbicos

Esto funciona tanto al crear o actualizar un registro, para lograr de manera efectiva la conversión solo se puede rellenar o actualizar 1 solo campo por grupo.

## Ejemplo

?> Si tenemos todos los campos vacios podemos rellenar tan solo el campo toneladas, lo cual realizara la debida conversión a Kilogramos y Libras

?> Si tenemos los campos del grupo 2 con datos y queremos calcular desde Centimetros Cúbicos basta con cambiar el valor en este campo para realizar la conversión

!> **No se debe cambiar o rellenar el valor de más de un campo por grupo a la vez**, esto causara un Error al no poder determinar cual es la unidad de preferencia para realizar la conversión

## Campos

| Field     | Type         | Requirement            |
| :-------- | :------- | :------------------------- |
| `Toneladas` | `decimal` | Optional |
| `Kilogramos` | `decimal` | Optional |
| `Libras` | `decimal` | Optional |
| `Metros Cúbicos` | `decimal` | Optional |
| `Pies Cúbicos` | `decimal` | Optional |
| `Centimetros Cúbicos` | `decimal` | Optional |

## Ubicación

| Action   | Entity       | Description      |
| :------- | :----------- | :--------------- |
| `CalculadorPesos` | `Aduanas` | `Calculo automatico de las dimensiones` |
| `CalculadorPesos` | `Consolidado` | `Calculo automatico de las dimensiones` |
| `CalculadorPesos` | `Cotizacion` | `Calculo automatico de las dimensiones` |
| `CalculadorPesos` | `Embarque` | `Calculo automatico de las dimensiones` |
| `CalculadorPesos` | `Oportunidad` | `Calculo automatico de las dimensiones` |
| `CalculadorPesos` | `Transporte` | `Calculo automatico de las dimensiones` |