.. |Perdida Ganancia No Realizada| image:: resources/loss-gain-not-realized.png
.. |Reporte de Diferencia de cambio DXC y DXP no Realizada| image:: resources/report.png
.. |Acción Completar| image:: resources/action-complete.png
.. |Diario Contable Completo| image:: resources/daily-accounting-complete.png

.. _document/process-currency-difference:

Proceso de Diferencia de Cambio no Realizada
============================================

El proceso de cálculo de la diferencia de cambio no realizada consta de dos (2) procesos diferentes,

- Revaluar  los saldos abiertos de documentos por cobrar y documentos por pagar nominados en moneda extranjera
- Revaluar los saldos contables de las cuentas monetarias nominadas en moneda extranjera

A continuación les detallaremos cada uno de ellos.

Proceso de Diferencia de Cambio No Realizada de Documentos por Cobrar y Documentos por Pagar
--------------------------------------------------------------------------------------------

ADempiere cuenta con un proceso para realizar el cálculo y aplicación contable correspondiente a la actualización de los saldos contables de los documentos por cobrar y documentos por pagar (que aún no hayan sido canceladas a la fecha de revaluación).

Proceso de Diferencia de Cambio de DXC y DXP No Realizada
---------------------------------------------------------

ADempiere cuenta con un proceso para realizar el cálculo y aplicación contable correspondiente a la actualización de los saldos contables de las cuentas por cobrar y cuentas por pagar (que aún no hayan sido canceladas a la fecha de revaluación).

|Perdida Ganancia No Realizada|

Imagen 1. Ventana Factura Pérdida/Ganancia no Realizada

- **Esquema Contable**: Seleccionar el esquema contable que se quiere registrar la diferencia de cambio.
- **Tipo de Conversión de Revaluación**: Tipo de conversión de la revaluación.
- **Fecha de Revaluación**: Fecha a realizar proceso.
- **CP-CC**: Cuentas x pagar (incluye documentos a pagar como son los cheques diferidos), cuentas x cobrar o ambas.
- **Incluir Todas las Monedas**: No hacer click. Dejar vacío.
- **Moneda**: Dejar vacío.
- **Revalorización Tipo de Documento**: Donde genera el asiento de revaluación (GL Document)- General Ledger (Contabilidad).

Dicho proceso realizará el cálculo necesario para actualizar la aplicación contable de los Saldos de todos aquellos documentos por cobrar y por pagar que se encuentren pendientes a la fecha de revaluación.

El resultado lo mostrará en el reporte de diferencia de cambio no realizada detallando línea a línea los documentos con el cálculo realizado. Descargarlo en XLSX para su análisis.

Reporte de Diferencia de cambio DXC y DXP no Realizada
******************************************************

|Reporte de Diferencia de cambio DXC y DXP no Realizada|

Imagen 2. Reporte de Diferencia de cambio DXC y DXP no Realizada

.. note::

    La emisión del reporte genera un asiento contable en borrador detallando línea a línea los ajustes que se estarían realizando documento por documento.

    El mismo lo podrán encontrar en la ventana de diario contable


El lote del asiento contable deberá completarse

|Acción Completar|

Imagen 3. Acción Completar 

Si desea anular un asiento ya completo deberá anular y corregir para que la fecha de anulación sea la misma que la del asiento.

.. warning::
    
    **CUIDADO**. La acción "**Anular**" y "**Causación**" crea el asiento con la fecha de hoy.




|Diario Contable Completo|

Imagen 4. Diario Contable Completo


Proceso de Diferencia de Cambio Cuentas Monetarias (de Cuentas Monetarias de Ganancia no Realizada)
---------------------------------------------------------------------------------------------------

Este proceso tomará todas las cuentas contables integrales “definidas” como moneda extranjera. Considera la moneda que tenga asignada dicha cuenta.

ver:

- Revaluaciones de Cuentas por Cobrar y Cuentas por Pagar

- Proceso de Revaluacion de Cuentas Integrales Cuentas Monetarias
