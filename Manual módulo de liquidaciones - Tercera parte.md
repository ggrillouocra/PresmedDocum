# DEBITOS / CREDITOS A EXPEDIENTES

Si durante la etapa de Revisión se han generado débitos al prestador la suma
total es llamada **Débito en revisión** (a)

a

## b

## c

## e

## d

En esta etapa el sistema efectúa una comparación entre los importes de la
factura ingresada y lo que se calculo en base a los convenios cargados. De allí
calcula la diferencia y el desvío. (d)

Esta información es de utilidad para fijar pautas de liquidaciones. Por ejemplo,
ciertas entidades no efectúan débitos cuando el desvío es menor de un porcentaje
estipulado.

También es necesario a esta altura aplicar al expediente los **Copagos por
orden** que para ser aplicados es necesario oprimir el botón (e) que aparece en
la pantalla.

Entonces el Debito total esta integrado por:

-   *Los copagos por orden*, es decir los copagos que se aplican conjuntamente a
    varios ítems de una receta.

-   *Débitos en revisión*, que pueden ser por diferencias de totales calculados
    vs. totales ingresados por orden.

-   *Débitos manuales*, que pueden ser por errores de facturación no imputables
    a un ítem en particular.

Una vez evaluados todos los tipos de débitos explicados el expediente pasa a
etapa de Supervisión.

Si por algún motivo el expediente fuese reabierto esta etapa de análisis de
débitos / créditos deberá ser realizada nuevamente.

En cualquier instancia del expediente es posible ingresar en el **Detalle de la
liquidación del** 1

Una vez allí se visualizan todos los ítems que forman parte del expediente, con
un amplio detalle de información (datos del prestador demandante, efector,
código y descripción de la prestación, etc.)

Y también se visualizan los importes ingresados (o sea facturados por el
prestador del expediente), los convenidos (o sea lo cargado en el/los convenios
que tiene asignado el prestador), montos debitados, copagos del plan, etc.

Para una mejor comprensión veremos varios ejemplos diferenciando el modo en que
fueron cargados los ítems.

-   a

## b

En esta opción durante la carga se ingresa un único valor para toda la orden
(a), para lo cual se debió haber elegido el tipo de carga *Orden* (b)

1

## 2

## 3

## 4

## 6

## 5

## 7

## 8

## 9

1.  *Total ingresado por la orden*, son los cargados por el operador o tomados
    por vía de importación (no se ve si se están ingresando valores a nivel de
    ítem)

    1.  *Totales ingresados a nivel de ítem*, si se ingresa valor por orden los
        mismos deben estar en cero.

    2.  *Total convenido*, son tomados del convenio cargado en el sistema para
        el prestador del expediente.

    3.  *Total a liquidar*, es el menor valor entre el ingresado y el convenido
        (incluye los débitos por orden de existir los mismos)

        En nuestro ejemplo será: 120,00 - 9,48 = 110,52

    4.  *Débitos por orden*, surge de la diferencia de valores entre lo
        ingresado y lo convenido a nivel de orden (no se ve si se están
        ingresando valores a nivel de ítem)

    5.  *Copagos por orden*, son aquellos copagos que fueron configurados en el
        plan a nivel de orden.

    6.  *Total de copagos para la orden*, suma de copagos por orden y por
        prestación (Ya que puede darse el caso que las prestaciones cargadas
        tengan simultáneamente copagos por orden y por prestación)

    7.  *Total a pagar*, es el importe final que se le pagará al prestador por
        la orden cargada, descontando débitos (excepto los del punto 5 que ya
        fueron descontados) y sin descontar los copagos.

        En nuestro ejemplo será: 110,52 - 5,00 = 105,52

    8.  *IVA a debitar*, importe de IVA que corresponde al afiliado gravado

-   a

## b

En esta opción durante la carga se ingresa el valor unitario para cada
prestación (a), para lo cual se debió haber elegido el tipo de carga *Unitario*
(b)

>   **Nota***: De no ingresarse un valor el sistema tomará el del convenio.*

En el detalle del expediente se visualizará de la siguiente manera:

*1*

## 8

## 4

## 5

## 3

## 2

## 9

## 6

## 7

## 10

-   *Total ingresado por la orden (1)*

    -   *Débitos por orden (2)*

    -   *Copagos por orden (3)*

Se mantienen los siguientes datos:

-   *Total convenido (4)*

-   *Total a liquidar (5)*

-   *Total a pagar (7)*

-   *IVA a debitar (6)*

Se agrega detalle en:

-   Totales ingresados a nivel de ítem, ya que los mismos son ahora ingresados
    por el operador. (8)

-   Débitos a nivel del ítem, se da en casos de diferencias entre lo ingresado y
    lo convenido, o débitos efectuados por el operador o los sugeridos por el
    sistema. (9)

-   Copagos por ítem, son los copagos que cada prestación tiene en forma
    individual. (10)

-   b

## a

En esta opción durante la carga no se ingresa el valor de la prestación (a),
para lo cual se debió haber elegido el tipo de carga *No* (b)

1

## 2

## 3

Los datos que se pierden son los mismos que en el caso de carga a nivel de ítem,
y en los que se gana en detalle también.

La diferencia radica en que las columnas de *Total ingresado* (1), *Total
convenido* (2) y *Total a liquidar* (3) tienen los mismos valores (que han sido
tomados del convenio)

Hemos visto hasta aquí como leer e interpretar en este reporte la información de
cada orden. Veremos ahora como entender las sumatorias totales sobre los cuales
se basara la liquidación del expediente.

4

## b

## c

## a

## 5

## 3

## 2

## 1

## d

1.  *Total ingresado*, es la sumatoria de todos los totales ingresados por el
    usuario (ya sea unitario o por orden)

2.  *Total convenido*, es la sumatoria de todos los valores a nivel de ítem
    tomados del convenio del prestador.

3.  *Total a liquidar*, este punto debe analizarse teniendo ante todo en cuenta
    si la orden tiene o no débitos por orden.

Si no tiene débitos por orden

Entonces es la sumatoria de los menores valores entre lo ingresado y lo
convenido. Es decir que el sistema toma el menor valor de cada orden.

Viéndolo con ejemplos será:

>   Valor ingresado 30.00, valor por convenio 31.90. El valor a liquidar será el
>   menor entre ambos, o sea 30.00

Si tiene débitos por orden

>   Entonces es la sumatoria de los valores ingresados menos los *Débitos por
>   orden* (a)

>   Valor ingresado 15.00, valor por convenio 11.84. El debito por orden es de
>   3.16 (surge de la diferencia entre 15.00 y 11.84). El valor a liquidar será
>   el que surge de 15.00 – 3.16 = 11.84

En el caso que estamos analizando la cuenta será: 441.44 – 12.70 = 428.74

1.  *Total a pagar*, es una cuenta muy simple de comprender.

    Total a liquidar (3) 428.74 menos

    Débitos por ítem (b) 27.96 menos

    Copagos por ítem (c) 11.50 menos

    Copagos por orden (d) 20.00

    **369.28**

2.  *Total de IVA a debitar*, es la sumatoria de todas las ordenes efectuadas a
    afiliados gravados

b

## e

## f

## d

El total de débitos del expediente surge entonces de la siguiente suma:

>   Débitos prestaciones o débitos por ítem (b) 27.96 mas

>   Débitos globales (e) 31.50 mas

>   Aquí se incluyen los débitos que no pueden ser aplicados a una orden en
>   particular, como por ejemplo el error de suma de una factura y los copagos
>   por orden (d) y por prestación.

>   IVA debitado (f) 0.00 mas

>   En el caso que presentamos aquí no se aplico debito sino que se solicita al
>   prestador el envío de la nota de debito por el monto de 9.79

>   Débitos por orden 12.70

>   **72.16**

c

## 4

## 3

## b

## a

## 2

## 1

1.  Total de débitos al prestador (sin incluir los débitos globales)

2.  Total exento + gravado, es el importe facturado por el prestador menos el
    valor de IVA

    En este ejemplo será: 455.30 (a) – 26.56 (b) = 428.74

3.  Debito global explicado anteriormente

4.  Diferencia de IVA a favor del prestador.

    *Surge de restarle al IVA calculado por el sistema (c) el valor facturado
    (b) por el prestador. En este ejemplo será: 36.35 (c) – 26.56 (b) = 9.79*

Si hacemos las sumas y restas de los valores detallados obtendremos el valor
neto a pagar en el expediente, que en este caso es de **383.14**.

Para comprobarlo haremos:

>   Importe exento facturado 149.86 mas

>   Importe gravado facturado 278.88

>   **Total exento + gravado 428.74** mas

>   IVA facturado 26.56

>   **Total facturado 455.30**

>   Débitos en ítems 27.96 mas

>   Débitos por orden 12.70

>   **Total débitos en revisión  40.66**

>   Copagos por ítem 11.50 mas

>   Copagos por orden 20.00

>   **Total débitos globales 31.50**

Si ahora calculamos 455.30 – 40.66 – 31.50 = **383.14** Que es el neto a pagar
que figuraba en el listado de la página anterior.

# 

# 3

1

a

## b

Ahora al seleccionar un expediente de la lista para supervisar (a), se despliega
el detalle de la orden de pago en la parte inferior de la pantalla (b) (antes se
desplegaba por el lado derecho)

c

El importe bruto se entiende como la suma de los importes exentos y grabados. En
el ejemplo que adjuntamos si se suma \$ 149.86 y \$ 278,88 nos da la suma total
de \$ 428.74.

Si a este ultimo importe le sumamos el IVA facturado de \$ 26.56 y le restamos
(o sumamos según corresponda) el indicado en la columna *Débitos / créditos* que
en nuestro ejemplo es de \$ –72.16 (recordemos que son 40.66 + 31.50) llegaremos
al total a pagar que figura en pantalla de \$ 383.14.

Como se ve la funcionalidad no ha cambiado en nada, solo se incorporo un dato
que faltaba.

Los pasos para supervisar un expediente son:

1.  Seleccionar si se desea alguno de los filtros de búsqueda de expedientes, lo
    cual en caso de ser un número elevado agiliza la tarea.

2.  Al hacer doble click con el botón izquierdo se marcará el expediente que se
    quiere supervisar. Allí se amplia la pantalla pudiendo ver los datos que
    formaran parte de la orden de pago.

En caso de haber más de un expediente para un mismo periodo es posible generar
una única orden de pago para todos ellos. Basta con marcar todos los expedientes
que aparecen en la lista para que el sistema sume los importe y reste los
débitos a aplicar de todos los expedientes.

Al oprimir el botón **Aceptar** se emitirá la orden de pago.

>   Para la *Supervisión de expedientes de honorarios* basta con chequear el
>   expediente que será próximo a liquidar.

>   En el caso de la *Supervisión de expedientes de órdenes y sanatorios*, se
>   genera otra unidad de pago que se llama “Resumen”.

>   En caso de que el expediente tuviese algún tipo de debito el sistema permite
>   generar la correspondiente nota de debito.

>   En caso de que la Entidad tenga autorización de la AFIP para auto numerar
>   los comprobante el sistema ira controlando la numeración automáticamente.

>   Si por el contrario la Entidad no cuenta con esta autorización, el sistema
>   permite ingresar los números de notas de debito preimpresos.

Al imprimir el resumen fija en el expediente el número asignado para evitar una
duplicación de liquidación. En el caso en que se produzca una diferencia se
puede adjuntar al resumen una nota de debito.

En este resumen se muestran el total bruto, IVA facturado, total del débito (en
ese caso se activarán los campos de número de nota de débito, fecha de nota de
débito y observaciones), IVA debitado, percepción del IVA, e IIBB.

El sistema permite imprimir las observaciones que se detallen en el campo
“Observaciones “ (**Obs**) pudiendo escribir hasta 250 caracteres.

1.  Al clickear con el botón izquierdo en este campo la pantalla mostrará los
    expedientes ya supervisados. Con esta funcionalidad es posible modificar o
    reimprimir estos expedientes.

Una vez supervisado el expediente el mismo pasa a etapa de Cierre de
Liquidación.

>   **Nota***: Mientras el expediente no sea liquidado definitivamente se puede
>   volver atrás la supervisión, la revisión e incluso la carga de ítems.*

>   *Una vez hecho el cierre de liquidación no hay vuelta atrás.*

#   
expedientes especiales

Veremos ahora algunos expedientes que tienen en el sistema un modo de generación
diferente.

Para generar estos expedientes se ingresa en la opción *Supervisión para cierre
de liquidación* en el menú principal y luego en *Globales, Honorarios fijos* y
*Globales capitados* según sea el caso a liquidar.

Estos expedientes son generados automáticamente por el sistema y en forma
masiva, tomando en cuenta el periodo prestacional y la característica del
convenio del prestador.

###   
Expedientes globales

Los expedientes globales están relacionados con aquellos prestadores a los que
se les asignaron convenios por un monto global sin tomar en cuanta la cantidad
de pacientes atendidos.

c

## b

## a

## d

## e

Una vez allí se podrá ver lista de expedientes ya generados para otro periodo
(a) y se podrán generar los nuevos expedientes. Para ello es necesario indicar
el periodo para el cual se generaran los expedientes (b) y oprimir el botón
**Generar expedientes**. (c)

El sistema emite cierta información relacionada con los expedientes.

Y luego nos informara la cantidad de expedientes generados para el periodo
indicado.

**Importante:** *No es posible generar dos o mas veces un mismo periodo. Si un
prestador tuviese más de un convenio global para el mismo grupo de pago se
generará 1 sólo expediente sumando ambos totales*

Una vez que los expedientes han sido generados se puede:

-   1

## 2

## 3

>   **Nota importante**: Los datos ingresados como consumo en estos expedientes
>   son meramente informativos, no serán valorizados en forma unitaria.

-   3

## 1

## 2

En esta opción se ingresan todos los datos incluidos en la facturación, entre
ellos el numero de comprobante, totales facturados (1), etc.

Tomando en cuenta el valor global ingresado en el convenio (2) el sistema genera
automáticamente el debito o crédito (3) por la diferencia.

Una vez que estos datos han sido ingresados es posible pasar al *Circuito de
carga*.

Nótese que el circuito de carga de expedientes globales es distinto al de
expedientes por prestación, (Ver pág. 9 sección Liquidaciones del Manual de
Usuario) ya que se omiten los botones de carga, reabrir, revisar y rectificar
errores que son propios de la liquidación de expedientes por prestación.

Desde esta pantalla se podrán por ejemplo efectuar nuevos débitos, clickeando en
el botón **Débitos** el mecanismo es el explicado en la pág. 34 de la sección
Liquidaciones de este manual.

### Supervisión de expedientes globales

Una vez que el expediente esta listo para ser supervisado (cabe aclarar que no
es necesario el ingreso de los consumos) se marca con el tilde y se oprime el
botón **Aceptar**. Con esta operación los expedientes han quedado supervisados y
listos para ser liquidados.

La liquidación se efectúa junto con el resto de los expedientes, y siguiendo los
pasos explicados en la pág. 29.

###   
Proceso Liquidaciones de expedientes por Capita (clearing)

Para poder administrar todas las cápitas que se administren en la entidad, tanto
en la confección de los padrones de los afiliados por cada período convenida por
zona.,como la detección de aquellos afiliados que han utilizado los servicios
que están dentro de otra capita, exportación de dichos afiliados fuera del
período y liquidación de los expedientes capitados,

Se detallaran todos los pasos a seguir para poder llevar a cabo lo expuesto
anteriormente:, se deberán efectuar algunos pasos previos para ello éstos son:

-   Cargar un prestador del tipo Coordinador según detalle en manual de
    Prestadores

-   Cargar un convenio del tipo capita, colocando el valor de la misma con
    vigencia y asignando la localidad correspondiente como se detalla en el
    manual de Convenio

    1.  **Generación de Padrón**

1.  Mensualmente se le enviará a los prestadores capitados un padrón generado
    por el sistema donde figurarán todos los afiliados incluidos en cada una de
    las cápitas , para obtener dicho padrón se deberá ingresar por
    Liquidaciones/Supervisión de expedientes/Clearing Generación de Padrones

Al accionar ésta opción el sistema traerá automáticamente la siguiente pantalla

Se selecciona el prestador Coordinador correspondiente

Se selecciona la Provincia Correspondiente el período y las localidades que se
deseen según se indica en la pantalla anterior

Al accionar el botón ACEPTAR, el sistema traerá todos aquellos afiliados
empadronados en las localidades y provincias filtradas con los datos que se
detallan a continuación:

En la parte inferior de la pantalla el sistema informa los siguientes datos:

-   Prepaga

-   Número de afiliado

-   Apellido y nombre

-   Fecha de Nacimiento

-   Fecha de ingreso a la entidad

-   Tipo y número de documento

-   Domicilio

-   Localidad

-   Provincia

-   Total de Cápitas

    Estos datos se pueden exportar como habitualmente se hace con todos los
    reportes del sistema.

    1.  **Generación de Clearing**

        Una vez obtenidos los padrones de las distintas cápitas convenidas, se
        procederá a liquidar los expedientes correspondientes como se detalla en
        el manual de liquidaciones en supervisión de expedientes
        capitados.(pagina 45/48)

        Si un afiliado perteneciente a una cápita de una localidad determinada,
        se atiende por otro prestador, de otra cápita u otro prestador , que no
        es un coordinador, el sistema generará en el proceso del **clearing**
        todos ésos registros informándolos en la siguiente pantalla:

        Se ingresa por Supervisión de Expedientes/Clearing/Generación de
        Clearing

Al accionar ésta opción el sistema desplegará la siguiente pantalla:

Se selecciona el período a procesar ye l grupo de pago correspondiente, siempre
y cuando todos los expedientes estén en el estado SUPERVISADOS.

Aquí el sistema traerá todos aquellos registros de afiliados que hayan utilizado
el servicio de la atención médica, con aquellos prestadores no capitados y fuera
de la zona capitada , es decir por ejemplo una persona que está incluída en la
cápita de Mendoza se atiende con un prestador fuera de esa cápita por causas
justificadas., dicho prestador factura las prestaciones correspondientes a la
entidad, y es allí donde el sistema trae identificados los mismos en la pantalla
que se mostró anteriormente.

1.  **Exportación de CLEARING**

Se ingresa por Supervisión de expedientes/Clearing/exportación de clear

Al ingresar por dicha opción el sistema traerá la siguiente pantalla:

Para poder exportar el clearing se deberá seleccionar el período
correspondiente, grupo de pago, la provincia y la localidad que se desean
obtener y también se presiona si se quiere obtener el dato de todos aquellos
expedientes liquidados, al accionar el botón Consulta el sistema emitirá el
detalle de todos los datos que se detallan a continuación:

1.  Número de prestador en Presmed

2.  Razón Social del Coordinador

3.  El número de oficina liquidadora del expediente en que fue cargado la
    prestación fuera de la cápita.

4.  El número de expediente

5.  El período

6.  La entidad correspondiente

7.  El número de afiliado

8.  Apellido y nombre del afiliado

9.  El prestador efector de la prestación fuera de cápita que no es un
    coordinador

10. Código de la práctica ingresada código según nomencladores del sistema

11. Descripción de dicha práctica

12. Cantidad

13. Valor

14. Copago si es que corresponde

15. Valor del débito.

>   Todos estos datos se pueden exportar a un archivo que se desee., Como el
>   sistema actúa en todos los reportes.

Tener en cuenta que cuando se genera el próximo período en la supervisión de
expedientes de todos aquellos prestadores que se han detectado afiliados cuyos
consumos se han realizado en prestador, realizarle los débitos correspondientes
pero en forma manual descontando los montos establecidos en la generación del
clearing.

También se podrán consultar en la misma pantalla todos los datos que ya fueron
exportados tildando la opción en pantalla de **exportados, que si se acciona
nuevamente el botón de exportar el sistema emite el aviso de que ya esos datos
fueron exportados**

###   
Expedientes de honorarios fijos

Para podes liquidar estos expedientes -a diferencia de los demás- no es
necesario que el prestador tenga asignado un convenio.

a

El mecanismo para generar un expediente, y supervisarlo es el mismo que el
explicado para expedientes globales. Aunque ingresando en la opción *Supervisión
para cierre de liquidación / Honorarios fijos*.

**Nota:** *En los expedientes de honorarios fijos no se pueden ingresar
consumos.*

###   
Expedientes globales capitados

Para poder liquidar este tipo de expedientes es necesario que el prestador tenga
asociado un convenio con valores globales por capita. (Para mas información ver
sección Convenios)

Se ingresa en la opción de menú *Supervisión para cierre de liquidación /
Globales capitados*, y se generan los expedientes del mismo modo que los de tipo
global.

a

## b

## c

## d

## e

El sistema calculara también el importe de IVA que correspondía facturar por
aquellos afiliados que han sido cargados en el campo *gravados*. (d) tomando en
cuenta la tasa de IVA cargada en los parámetros de liquidación. (e)

Una vez generados los expedientes se procede del mismo modo que para los
expedientes globales, según lo explicado en la pág. 39.

**Carga de Número de Cheque y Caja en Liquidaciones]**

Para poder editar el número de cheque con el que se ha abonado al prestador(es
decir funciona solamente con expedientes liquidados) y el número de Caja y Bank
que corresponden al circuito interno de la institución.

Se ingresa por Liquidaciones/Carga de Cheques y envíos.

# Al ingresar en la opción marcada el sistema desplegará la siguiente pantalla:

9

10

8

7

5

1

2

6

4

3

Datos que se cargan en la pantalla

1.  Oficina Liquidadora

2.  Número de expediente

3.  Fecha del cheque

4.  Número de cheque

5.  Número de Caja

6.  Número de Bank

7.  Tilde de enviado

8.  ALTA BAJA O MODIFICAR

9.  Listar está la opción como en cualquier reporte del sistema de la impresión

10. Detalles de datos cargados con fecha de alta baja o modficación

    Nota. No permite cargar número de expedientes repetidos y si el mismo número
    de cheque para varios expedientes.

#   
LIQUIDACIÓN DE EXPEDIENTES

Este es el paso final del proceso de liquidación de prestaciones, y es el único
de todo el circuito que es irreversible.

1

## 2

## 3

## 4

Luego se debe:

1.  Colocar el período de los expedientes que se quieran liquidar.

2.  Seleccionar el grupo de pago y oficina liquidadora asignados al expediente
    que se va a liquidar.

    El sistema mostrará la totalidad de los expedientes pendientes de
    liquidación de ese grupo de pago y de ese periodo (3).

    También se podrán ver los expedientes pendientes de supervisión de ese grupo
    seleccionado (4).

    Luego se selecciona cada uno de los expedientes que se liquidaran y se
    oprime el botón **Aceptar**.

#   
Interfaces contables

Las interfaces contables generan archivos que alimentan los sistema de
contabilidad ajenos al *Presmed*.

Para poder correr el proceso de generación de los archivos, es necesario tener
previamente configurada la opción de interfaz contable. (Para mas información
ver sección *Tablas* del Manual del usuario de Presmed)

Depende de la opción de interfaz que se haya seleccionado el proceso será
automático o no.

En el proceso automático cada vez que se produce un evento que requiere la
generación de la interfaz (por ejemplo liquidación de un expediente) el sistema
dispara el proceso que crea el archivo para la interfaz.

1

## 3

## 4

## 2

Una vez allí se despliega la siguiente pantalla.

1.  Indica el directorio donde serán enviados los archivos una vez generados.

2.  Se establece el día que se quiere procesar, esto generara archivos
    conteniendo los datos de todos los cambios generados en esta fecha.

3.  Este tilde permite visualizar la lista de archivos generados (4)

Para disparar la generación de los archivos se oprime el botón **Procesar**.

#   
Exportación de copagos

Esta opción permitirá exportar aquellos copagos que hayan quedado a cargo del
Afiliado, y que deberán ser incluidos en la facturación de sus cuotas.

Para generarlos se ingresa en la opción *Procesos irreversibles / Exportación de
copagos* del menú de liquidaciones.

a
