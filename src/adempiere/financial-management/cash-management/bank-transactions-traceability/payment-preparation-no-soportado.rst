.. _document/payment-preparation-no-soportado:

**Preparación de Depósitos   no soportado**
===========================================

Cuando una empresa recibe pagos de clientes, a menudo se registran en una cuenta bancaria específica como efectivo. Sin embargo, los pagos aparecen en la cuenta bancaria más tarde, cuando se depositan físicamente.

Como regla general, las empresas depositan cheques de clientes y dinero en efectivo en el banco a granel. Por lo tanto, durante la conciliación de las cuentas en efectivo con los estados de cuenta bancarios, a menudo se tiene problemas para hacer coincidir los pagos individuales que ingresan en una cuenta en efectivo con los montos resumidos de los depósitos en un estado de cuenta bancario, que tienen las fechas de los depósitos en el banco. Estas condiciones crean dificultades para realizar un seguimiento preciso del efectivo disponible y para conciliar los saldos de las cuentas en efectivo.

En el sistema, usted utiliza los depósitos bancarios para rastrear los pagos de los clientes que deposita al banco en forma masiva. Cuando ingresa en los pagos del sistema destinados a dichos depósitos, los pagos se registran temporalmente en cuentas especiales de compensación . Estas cuentas retienen los pagos provenientes de las cuentas de Cuentas por cobrar de los clientes.

Antes de realizar un depósito físico en el banco, crea un depósito en el sistema y enumera todos los pagos y el efectivo que conforman el depósito físico. Una vez que haya realizado el depósito en el banco, libere el depósito en el sistema. Como resultado, el sistema genera un lote de transacciones para transferir los montos de pago de las cuentas de compensación a la cuenta bancaria y registrar los cargos incurridos como gastos.

Aquí, leerá acerca de cómo configurar el procesamiento de depósitos bancarios, registrar un depósito en el sistema y hacer las correcciones necesarias.

**Configurando el procesamiento de depósitos**
----------------------------------------------

**Tramitación de Depósitos**
----------------------------

Una vez que se haya configurado el procesamiento de depósitos bancarios, puede utilizar esta funcionalidad de la siguiente manera:

Recolección de pagos de clientes en cuentas de compensación

Ingreso del depósito

**Procesamiento de Cheques posdatados**
---------------------------------------

Algunos cheques de los clientes son posteriores, lo que significa que tienen fechas futuras. Aunque el envío de cheques con fecha posterior no es una práctica común, algunos clientes los envían ocasionalmente. Estos cheques no deben depositarse en un banco antes de la fecha del cheque.

**Anulación de un Depósito**
----------------------------

Si es necesario, puede anular un depósito . El sistema crea un depósito anulado con la misma lista de pagos incluidos y las mismas cuentas involucradas.

Este proceso devuelve a ese importe anulado a la cuenta de compensación.

**Gestión de pagos registrados por error**
------------------------------------------

Para facilitar la creación de depósitos, debe asignar a una cuenta de compensación solo aquellos métodos de pago cuyos pagos deben depositarse en la cuenta bancaria correspondiente. Si los pagos no relacionados se registran en la cuenta de compensación, los usuarios pasarán tiempo adicional seleccionando los pagos apropiados para el depósito de una lista de pagos relacionados y no relacionados. Si con el tiempo detecta que los pagos no relacionados se han registrado en la cuenta de compensación por error (y, por lo tanto, no se pueden incluir en ningún depósito), elimine los pagos de la cuenta de compensación anulándolos y creando nuevos con las cuentas de efectivo adecuadas especificadas.

Si se da cuenta de que los pagos (ventas en efectivo) que se depositarán se registraron en una cuenta de efectivo que no es una cuenta de compensación, debe anularlos y crear nuevos con las cuentas de efectivo adecuadas especificadas.

**Conciliación de varias líneas de la empresa con una línea del Banco**
-----------------------------------------------------------------------

Actualmente el Sistema no soporta este caso.

Solución:

En el caso que se deba conciliar una línea del Banco con varias líneas de la empresa, se deberá modificar las líneas importadas del extracto, sustituyendo esa línea única por las líneas que están registradas en la empresa. De esa manera el registro del Banco quedará igual que el de la empresa.

Una vez que se incorpore en el extracto importado esas líneas, se deberá poner en 0  la línea sustituída e inactivarla.

Para que esto no suceda se debe depositar 1 cheque por depósito.

**Conciliación de varias líneas del Banco con una línea de la Empresa**
-----------------------------------------------------------------------

Actualmente este caso no está soportado

Solución:

En el caso que se deba conciliar una línea de la Empresa con varias líneas del Banco, se deberá modificar las líneas importadas del extracto, unificando las líneas del banco en una sola. Se modifica una línea y las demás líneas del banco se llevan a 0 y se inactivan.

De esta manera quedará igual la empresa y el banco.