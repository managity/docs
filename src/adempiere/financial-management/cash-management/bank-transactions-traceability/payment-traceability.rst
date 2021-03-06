.. _document/payment-traceability:

**Trazabilidad de Pago/Cobros**
===============================

Este capítulo lo ayudará a comprender cómo configurar y procesar aún más los pagos desconocidos, los cargos financieros y los depósitos bancarios.

**Reclasificación de pagos desconocidos**
-----------------------------------------

**Configurando el proceso de pagos desconocidos**
-------------------------------------------------

**Procesando pagos desconocidos**
---------------------------------

Cuando detecta un pago desconocido en el extracto bancario, lo procesa de la siguiente manera:

Cree una transacción Pago/Cobro y use el cargo apropiado para el pago desconocido.

Una vez que se conozcan los detalles del pago, reasigne el pago

**Registro de gastos financieros**
----------------------------------

**Configuración de Cargos Financieros**
***************************************

**Registro de Cargos Financieros**
**********************************

**Preparación de Depósitos**
----------------------------

Cuando una empresa recibe pagos de clientes, a menudo se registran en una cuenta bancaria específica. Sin embargo, los pagos aparecen en la cuenta bancaria más tarde, cuando se depositan físicamente.

Como regla general, las empresas depositan cheques de clientes y dinero en efectivo en el banco a granel. Por lo tanto, durante la conciliación de las cuentas de Banco con los estados de cuenta bancarios, los empleados a menudo tienen problemas para hacer coincidir los pagos individuales que ingresan en una cuenta en efectivo con los montos resumidos de los depósitos en un estado de cuenta bancario, que tienen las fechas de los depósitos en el banco. Estas condiciones crean dificultades para realizar un seguimiento preciso del efectivo disponible y para conciliar los saldos de las cuentas en efectivo.

En el sistema, usted utiliza los depósitos bancarios para rastrear los pagos de los clientes que deposita al banco en forma masiva. Cuando ingresa en los pagos del sistema destinados a dichos depósitos, los pagos se registran temporalmente en cuentas especiales de compensación . Estas cuentas retienen los pagos provenientes de las cuentas de Cuentas por cobrar de los clientes. Antes de realizar un depósito físico en el banco, crea un depósito en el sistema y enumera todos los pagos y el efectivo que conforman el depósito físico. Una vez que haya realizado el depósito en el banco, libere el depósito en el sistema. Como resultado, el sistema genera un lote de transacciones para transferir los montos de pago de las cuentas de compensación a la cuenta bancaria y registrar los cargos incurridos como gastos.

Aquí, leerá acerca de cómo configurar el procesamiento de depósitos bancarios, registrar un depósito en el sistema y hacer las correcciones necesarias.

**Configurando el procesamiento de depósitos**
**********************************************

**Tramitación de Depósitos**
****************************

Una vez que se haya configurado el procesamiento de depósitos bancarios, puede utilizar esta funcionalidad de la siguiente manera:

Recolección de pagos de clientes en cuentas de compensación

Ingreso del depósito

**Procesamiento de Cheques posdatados**
---------------------------------------

Algunos cheques de los clientes son posteriores, lo que significa que tienen fechas futuras. Aunque el envío de cheques con fecha posterior no es una práctica común, algunos clientes los envían ocasionalmente. Estos cheques no deben depositarse en un banco antes de la fecha del cheque.

**Anulación de un Depósito**
****************************

Si es necesario, puede anular un depósito . El sistema crea un depósito anulado con la misma lista de pagos incluidos y las mismas cuentas involucradas.

Este proceso devuelve a ese importe anulado a la cuenta de compensación.

**Gestión de pagos registrados por error**
******************************************

Para facilitar la creación de depósitos, debe asignar a una cuenta de compensación solo aquellos métodos de pago cuyos pagos deben depositarse en la cuenta bancaria correspondiente. Si los pagos no relacionados se registran en la cuenta de compensación, los usuarios pasarán tiempo adicional seleccionando los pagos apropiados para el depósito de una lista de pagos relacionados y no relacionados. Si con el tiempo detecta que los pagos no relacionados se han registrado en la cuenta de compensación por error (y, por lo tanto, no se pueden incluir en ningún depósito), elimine los pagos de la cuenta de compensación anulándolos y creando nuevos con las cuentas de efectivo adecuadas especificadas.

Si se da cuenta de que los pagos (ventas en efectivo) que se depositarán se registraron en una cuenta de efectivo que no es una cuenta de compensación, debe anularlos y crear nuevos con las cuentas de efectivo adecuadas especificadas.