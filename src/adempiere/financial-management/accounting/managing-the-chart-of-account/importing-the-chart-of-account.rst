.. _document/importing-the-chart-of-account:

De manera similar a toda importación de datos en ADempiere, es posible importar el plan de cuentas (o también llamado el "Catálogo de Cuentas").

Para ello es necesario primero definir un "Formato de Importación" que haga referencia a la tabla de importación "I_Element__Value"._Es preciso definir los siguientes campos:

- Código
- Nombre
- Descripción
- Explicación de la cuenta.
- Tipo de cuenta (Activo, Pasivo, Gastos, Ingresos, etc.)
- Entidad Acumulada Si lo es, entonces se trata de una cuenta intermedia; de lo contrario una cuenta final.
- Referencia a cuenta padre
En caso que la cuenta tenga padre, se pone aquí el código de dicha cuenta.

Luego se crea un archivo csv que contenga una línea por cada cuenta contable a ser importada; y cada línea tendrá como columnas delimitadas por el símbolo ";" los campos arriba mencionados.

Al llamar el proceso "Cargador de Archivos", se seleccionan el archivo de importación y el formato de importación explicados anteriormente. Se ejecuta la carga de las líneas de importación. El proceso indica de cuántas líneas consta el archivo de importación, y cuántas líneas se importaron correctamente.

El resultado del proceso "Cargador de Archivos" se puede ver en la ventana "Importar Cuentas Contables". Aquí se revisan los datos de la importación, y en caso que todo esté correcto, se ejecuta la importación de cuentas contables propiamente dicha, al pulsar el botón "Importa Cuentas".

En la ventana "Elemento Contable" se puede ver el resultado de la importación.

Luego de haber importado el Plan de Cuentas, éstas pueden ser utilizadas en la configuración contable.
