# Convenios con prestadores

### Consideraciones generales

Este módulo permite la creación y actualización de los convenios que definen las
prestaciones, sus valores para cada cartilla y lugar de atención de acuerdo a
cada prestador.

Se pueden definir diferentes tipos de convenios:

-   **Por prestación**, cuando se paga cada prestación realizada por el
    prestador al que se le aplica el convenio

-   **Por cápita,** se aplica al caso en el que un prestador recibe una cápita
    para afiliados de una zona o conjunto de localidades determinado. En este
    caso se indican las prestaciones que están capitadas. El sistema puede
    discriminar, cuando un afiliado de dicha zona se realiza una prestación
    fuera de la zona, y generar la observación para debitarla del prestador
    capitado. (Clearing).

-   **Para atención ambulatoria / General**, los prestadores pueden tener un
    convenio único para las prestaciones se desarrollen en atención ambulatoria
    o en internación

-   **Para Internacion**, los prestadores tienen un convenio específico para
    internación que se diferencia del de ambulatorio, en alguno de los
    parámetros que lo definen. Si se indican valores de días de internación o de
    módulos, deben estar obligatoriamente en convenios de internación.

    Un prestador puede tener convenio para una misma prestación en un mismo
    lugar de atención para una misma cartilla siempre y cuando se hayan
    registrado bajo diferentes Tipos de convenio **(General – Internaciòn)**

    Cabe aclarar que al momento de la liquidación de una prestación si ésta fue
    efectuada en forma ambulatoria el sistema validará la prestación bajo el
    convenio de tipo: General. En cambio si la prestación se efectúo por la vía
    de la internación el sistema validará la prestación bajo el convenio de
    tipo: internaciòn, y en el caso de que la prestación no exista en éste tipo
    de convenio para el prestador al cual se le liquida o bien tenga algún tipo
    de error como por ej: Prestación sin valor en el convenio, el sistema
    validará la prestación bajo el convenio de tipo: ambulatoria / General

Un prestador puede tener un conjunto de prestaciones a cierto valor para atender
a una población determinada en un *Centro Médico*, y otro conjunto de
prestaciones con valores diferentes para hacerlo con otras poblaciones en otro
Centro Médico.

La construcción de un convenio puede desarrollarse en varios niveles:

-   **Convenios básicos,** son aquellos que incluyen prestaciones con valores
    predefinidos que se aplican habitualmente a un conjunto de prestadores.
    Estos convenios deben ser luego asignados a uno o varios prestadores para
    que opere en una cartilla y un lugar de atención de los definidos para el
    mismo

-   **Valorización de convenios básicos**, se fija valores a las distintas
    prestaciones incluidas en el convenio básico.

Para un prestador específico, se puede generar un convenio particular nuevo o
partiendo de los convenios de prestaciones básicas predeterminadas, pueden
efectuarse modificaciones o ajustes, incorporando o eliminando prestaciones.

-   **Convenios propios**, a diferencia de los básicos éstos son los propios de
    cada prestador es decir no se pueden agrupar prestaciones y asignárselos a
    distintos prestadores. Se abre un convenio para cada uno y se incluyen todas
    las prestaciones que tienen distintos valores.

#   
Alta de convenios básicos

Para manejarnos con mas claridad en este tema explicaremos en una primera
instancia los puntos generales y comunes del alta de cualquier tipo de convenio
para luego focalizar nuestra atención en explicar las diferencias puntuales.

Para acceder a esta pantalla se debe ingresar por la opción del menú
**Convenios** / **Carga de Convenios**.

1

## 2

## 3

## 4

## 5

## 6

## 7

## 8

## 9

## 10

1.  **Nombre de convenio**, con el cual se lo reconocerá en el sistema.

2.  **Tipo de convenio**, se debe seleccionar según las siguientes opciones:

-   *General*, se utiliza para convenios ambulatorios básicos o propios.

-   *Internación*, se usa para los casos que tengan prestaciones en internación
    habilitándose la opción de módulos días.

1.  **Tipo de Servicio**, se selecciona de la lista cargada en el sistema.

2.  Se asigna una **especialidad** de las cargadas en el sistema.

3.  **Categoría**, solo para los casos de convenios asociados con Círculos
    Médicos. (Ver sección círculos médicos del presente manual)

4.  **Básico**, se seleccionara *Sí* si será aplicable a varios prestadores y
    *No* si será un convenio propio de algún prestador.

5.  Se puede ingresar un texto en **Observaciones**

6.  Si el convenio es quirúrgico puede definirse si incluye pago de
    Instrumentadora y los valores o porcentajes sobre el honorario del
    Especialista que corresponde. Puede definirse también si corresponde un
    esquema de importes mínimos por cirugías pequeñas. Se elige la opción en
    **“usa el criterio de valor mínimo”**.

7.  Nomencladores, se seleccionan los nomencladores de los cuales se elegirán
    las prestaciones que quedaran incluidas en el convenio.

Explicaremos ahora cada uno de los botones que forman parte de esta pantalla,
describiendo las funcionalidades de cada uno de ellos.

### Prestaciones

b

## a

## c

## d

1.  De haber seleccionado mas de un nomenclador en la pantalla anterior se
    tendrá que elegir el nomenclador sobre el cual se trabajará en primera
    instancia.

2.  Se marcan los conceptos que corresponden (Honorarios y/o Gastos)

3.  Se trasladan de izquierda a derecha las prestaciones que se incluirán en el
    convenio, que pueden ser todas de un mismo nomenclador o solo algunas (d).

###   
Valores

1

## 2

## 3

## 5

## 6

## 7

## 4

Existen tres tipos de valores para los convenios, por monto global, por monto
global capitado o por prestación.

-   Global total

    Este tipo de convenios esta relacionado con aquellos prestadores a los que
    se les liquida un monto determinado de dinero sin tomar en cuanta la
    cantidad de prestaciones efectuadas.

-   Global por capita

    El concepto es similar al anterior con la diferencia que en estos convenios
    se toman en cuenta la cantidad de afiliados que conforman la capita de la
    entidad que el prestador esta autorizado a atender.

-   Por prestación

    Cada prestación tiene un valor propio.

-   Alta de valores

    Para valorizar los convenios Globales y Globales por capita se debe:

1.  Seleccionar el nomenclador sobre el cual se va a trabajar y luego las
    prestaciones haciendo sobre ellas click con el botón derecho del mouse.

2.  Fecha de vigencia del convenio.

3.  Se ingresa el importe.

    Para valorizar convenios por prestación se deben asignar los valores para
    cada uno de los conceptos a

## b

## c

## d

## e

## f

*(Área ampliada)*

1.  Fecha a partir de la cual entran en vigencia los precios del convenio.

2.  Ajustes al valor del nomenclador en Porcentajes en más o en menos (%+) ó
    (%-)

3.  Ajustes al valor del nomenclador mediante factores de multiplicación (\*)

4.  Asignación de valor fijo en \$ para las prestaciones seleccionadas (Valor)

5.  Asignación de valor del Galeno (si son Honorarios) o del Gasto (Uni)

6.  Se asignan los Porcentajes de Urgencias Diurnas y Nocturnas(%UD/%UN)

    Al oprimir **Aceptar** (5) la prestación aparece resaltadas en negrita (1).

    Al hacer doble click en una de esas prácticas valorizada aparecerá en la
    parte inferior de la derecha el detalle del valor ingresado. (7)

-   Modificación de valores de prestaciones ya ingresados

-   Para efectuar una modificación de alguno de los valores definidos
    previamente, se seleccionan las prestaciones haciendo doble click en el
    árbol del lado izquierdo.

-   En la ventana inferior derecha se despliegan los valores seleccionados.

-   Se selecciona la prestación cuyos valores se desea cambiar y se efectúa la
    modificación en la ventana habilitada.

-   Se oprime **Aceptar**.

-   Agregado o eliminación de valores a partir de otras fechas de vigencia

Si se quiere definir nuevos valores a partir de otra fecha de vigencia de oprime
el icono de Agregar ítems desplegándose las opciones explicadas anteriormente.
(ver área ampliada)

Para eliminar valores de alguna prestación se la selecciona en la ventana
inferior derecha haciendo doble click (prestando especial atención en las fechas
de vigencia) y se oprime el icono Borrar ítems y luego el botón **Aceptar**.

Para eliminar de la ventana superior derecha los valores desplegados se oprime
el icono Limpiar (esta función no elimina los valores sino que los limpia de la
visualización de la pantalla)

Luego de dar de baja los valores de las prestaciones es conveniente eliminarlas
de la lista. Para ello basta con oprimir el botón **Baja prestaciones sin
valor** (6)

### Modulo día

1

## 2

Para valorizarlo se debe:

1.  Asignar una vigencia desde la cual se tomaran en cuenta estos valores.

2.  Ingresar el valor de cada modulo.

###   
Copiar

Este botón permite traer las prestaciones que forman parte de otro convenio y
evitar así el paso de selección de cada una de las prestaciones. (Botón
prestaciones)

Los pasos 1 al 7 explicados para el alta de convenios (Pág. 2) deben efectuarse
antes de copiar las prestaciones.

Luego se oprime el botón **Copiar**, allí se despliega la siguiente pantalla que
nos permitirá buscar entre los convenios existentes aquel que utilizaremos como
base para el nuevo.

Una vez encontrado el convenio a copiar se hace sobre el doble click con el
botón izquierdo del mouse.

Entonces el sistema nos solicitara la confirmación de la operación.

Al oprimir el botón **Aceptar** el sistema habrá asignado un número al nuevo
convenio y habrá copiado todas las prestaciones que están incluidas en el
convenio de referencia.

Luego será necesario valorizadas, ya que los valores, vigencias, etc. no son
copiados.

###   
Baja

Da de baja todo el convenio.

Si bien la baja del convenio puede ser revertida, solo se recuperan las
prestaciones que forman parte del mismo. Los datos de valores, vigencias, etc.
**no** se recuperan.

### Normas

1

## 2

## 3

## 4

1.  Se selecciona la prestación a la cual se le aplicaran normas.

2.  Si el sistema detecta que en otro convenio existen normas aplicadas para
    esta prestación las mismas serán desplegadas.

3.  Haciendo doble click sobre ellas con el botón izquierdo del mouse son
    copiadas. En este espacio se pueden agregar y quitar comentarios.

4.  Cantidad máxima de días incluidos y sector de internación.

Una vez configuradas las normas se oprime el botón **Aceptar**.

###   
Copagos

Desde esta opción se define que TODAS las prestaciones incluidas en el convenio
tienen copago y son descontadas al prestador.

En caso de incompatibilidad con la modalidad definida en el plan de cobertura,
se prioriza ésta configuración.

Se asigna una fecha de vigencia y se selecciona el tipo de unidad de calculo,
que puede ser por porcentaje (%) o un monto determinado (\$). Luego se oprime el
botón **Aceptar** y las mismas quedan grabadas.

# 

# Una vez dado de alta el copago el mismo queda registrado en la cabecera del convenio.

### Consultas

# Desde esta pantalla se podrán buscar los convenios tomando en cuenta los distintos filtros proporcionados.

#   
Alta de convenios propios

En esta etapa explicaremos solo aquellos puntos que diferencian un convenio
propios de uno básico.

Los convenios propios se diferencian de los básicos entre otras cosas por su
numeración (a) ya que los básicos pueden numerarse desde el 1 hasta el 9999.
mientras que los propios comienzan su numeración a partir del 10.000.

Y además porque los convenios propios sólo pueden asignarse a un único
prestador.

b

## a

Los pasos para el alta del convenio son iguales a los explicados en la pag. 2
con la salvedad que para los convenios propios debe seleccionarse la opción
**No**. (b)

*(Área ampliada)*

Como los convenios propios son aplicables a un único prestador debe
seleccionarse aquí la entidad o profesional al que se les aplicaran los valores
del convenio.

Si se desconoce el código se inicia la búsqueda del mismo en el sistema
oprimiendo el icono.

Una vez seleccionado el prestador se deberá indicar a que cartillas de las que
tiene habilitadas será aplicable este convenio.

Para ello se oprime el icono de Cartillas y se despliega la lista de cartillas
asociadas con este prestador.

Allí se marca con el tilde las cartillas.

Se asignan las cartillas correspondientes

Si por el contrario se quieren definir las prestaciones incluidas en el convenio
una a una, se eligen los nomencladores sobre los que se seleccionarán las
prestaciones y se oprime el botón **Prestaciones**. (Ver Pág. 3)

Luego se procede a valorizar el convenio como se explicó anteriormente. (Ver
Pág. 4)

>   **Nota***: El tipo de servicio y la especialidad pueden no corresponder
>   exactamente con los definidos para el prestador, particularmente cuando son
>   convenios que abarcan varias especialidades.*

#   
Convenios de Cápitas

Estos convenios se aplican en los casos en los que un prestador recibe una
cápita para afiliados de una zona o conjunto de localidades determinado.

El sistema puede discriminar, cuando un afiliado de dicha zona se realiza una
prestación fuera de la zona, y generar la observación para debitarla del
prestador capitado (Clearing).

Estos convenios son propios y el prestador debe ser del tipo *Coordinador*.

La única diferencia con el convenio propio es que en el de capita es necesario
definir las zonas relacionadas con el convenio. Para ello se oprime el icono

*(Área ampliada)*

3

## 1

Los pasos son:

1.  Seleccionar la provincia para que se despliegue la lista de códigos postales
    que la integran.

2.  Lista de códigos postales que no están incluidos en la zonificación.

3.  Lista de códigos postales que están incluidos en la zonificación.

#   
convenios de círculos médicos

Los convenios de los círculos médicos se diferencian principalmente porque se
efectúan por categorías (1), por lo que se deberán realizar tantos convenios
como categorías haya.

>   1
