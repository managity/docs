.. _document/chart-of-accounts-overview:

**Manejando el Catálogo de Cuentas**
====================================

El objeto central de la contabilidad es el catálogo de cuentas.

El catálogo de cuentas normalmente se importa a ADempiere y contiene todas las cuentas que va a utilizar.

En ADempiere se encuentra el catálogo, en la ventana catálogo de cuentas, pestaña cuentas contables, que es donde van a caer las cuentas importadas.

**La Contabilidad Perpetua en ADempiere**
-----------------------------------------

ADempiere maneja la contabilidad de una manera especial, no como la mayoría de sistemas o como hasta ahora están acostumbrados muchos usuarios. Se llama contabilidad perpetua. Bajo este concepto se entiende una contabilidad constante en la cual normalmente no hay cortes ni cierres. Es decir, los valores de las cuentas continúan y no se pasan a cero.

**Gestión del Catálogo de Cuentas**
===================================

Cada empresa tiene su propio plan de cuentas. ADempiere le permite definir su propio plan de cuentas según las necesidades específicas de cada empresa.

Para facilitar a las empresas ADempiere posee incorporado un completo catálogo de cuentas que cumple con la normativa internacional relativa a la presentación de estados financieros, que muy probablemente cumpla la mayor parte de sus requerimientos sobre este punto.

**La contabilidad preconfigurada en ADempiere**
-----------------------------------------------

Cuando se factura, ADempiere toma la configuración contable del socio de negocio, de los productos, los impuestos para realizar los asientos contables. Cuando se recibe o entrega material, se toma la configuración contable de los productos para realizar los asientos contables. Cuando se paga o cobra, se utiliza la configuración contable de las cuentas bancarias y del socio de negocio para realizar los asientos contables.

Así sucesivamente con todos los documentos por contabilizar, ADempiere toma la configuración contable de los objetos involucrados para realizar los asientos contables.

Al crear un socio de negocio (SDN), se toma la configuración contable del grupo de SDN a la que pertenece el SDN como configuración contable del SDN.

Al crear un producto, se toma la configuración contable de la categoría de producto a la que pertenece el producto como  configuración contable del producto.

La contabilidad como efecto colateral de la operación

El contador no tiene que ejecutar la contabilidad porque existe un proceso en ADempiere que corre a una frecuencia determinada. Este proceso se encarga de procesar contablemente cada documento no contabilizado.

