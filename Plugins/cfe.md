# CFE - Crear o Actualizar Factura por Expediente

> Encargado del proceso de facturación del sistema. Agrupa los productos de la entidad actual y crea facturas asociadas.

- Summary
    - [Ejecución](#ejecución)
    - [Proceso](#proceso)
    - [Ejemplo](#ejemplo)
    - [Campos](#campos)
    - [Ubicación](#ubicación)

## Ejecución

Para utilizar el plugin debemos marcar el boton de **Facturar** de la entidad actual, esto inicia el proceso de facturación.

!> <span style='color: red'>Existen Campos Requeridos</span>: **Seguimiento y Expediente**, esto para separar e identificar cada factura

## Proceso

Se toman los productos de la entidad y son separados segun: **Locales o Internacionales, de Reembolso o a Colectar**, creando diferentes facturas para contener los productos dependiendo del tipo de comprobante del **Cliente** y el tipo de comprobante **COL**. Tanto como los productos **Locales** como los de **Reembolso** son creados en facturas con el comprobante del **Cliente**, por otro lado, los productos **Internacionales** como los productos **a Colectar** son agrupados en una sola factura con el comprobante **COL**

?> El tipo de comprobante **COL** es definido dentro de la configuración del sistema.

## Ejemplo

## Campos

| Field     | Type         | Requirement            |
| :-------- | :------- | :------------------------- |
| `Seguimiento` | `Search` | <span style='color: red'>Required</span> |
| `Expediente` | `Search` | <span style='color: red'>Required</span> |

## Ubicación

| Action   | Entity       | Description      |
| :------- | :----------- | :--------------- |
| `CFE` | `Aduana` | `Crear o Actualizar Factura por Expediente y Tipo de NCF` |
| `CFE` | `Embarque` | `Crear o Actualizar Factura por Expediente y Tipo de NCF` |
| `CFE` | `Transporte` | `Crear o Actualizar Factura por Expediente y Tipo de NCF` |