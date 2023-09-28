# GRUPO1DBD
Grupo 1 Diseño de Base de Datos 

1. DESCRIPCIÓN DE LA EMPRESA

1.1 DATOS DE LA EMPRESA

1.2 DESCRIPCIÓN DEL PROCESO DE NEGOCIO
   El proceso de negocio elegido es todo el proceso de cobranzas de deuda consumo y deuda AFP, desde la automatización de los procesos de cargas de datos y la reportaría manual, ya que estos procesos generan mucho tiempo de retraso en todo el proceso. 

1.2.1 PROCESO DE COBRANZA (AS-IS)
      Actualmente la empresa realiza su gestión de cobranza consumo y AFP a través de un sistema web propio y mediante un proceso previo manual que realiza el área de ti para cargar datos del deudor, su deuda y montos de campaña.
El proceso inicia con la recepción mediante correo electrónico de las bases de la campaña del mes correspondiente, este correo lo recibe el supervisor de cartera y el jefe del área de TI, el jefe del área de TI, en caso la cartera recibida sea de AFP se recibe también información sobre los factores del mes correspondiente con el que se actualizara el del mes anterior, se deriva con los asistentes de TI quienes se encargan de la creación de la campaña del mes, para darle formato ,a la información recibida, de una plantilla que ya manejan para las cargas de “Obligaciones” en formato separado por comas (.csv), inicia con la carga de estas “Obligaciones” en lo que es la Campaña del mes. 
Luego, dentro de la información recibida se encuentra el detalle de los deudores con números de contacto y correo personal, esta información se trabaja realizando búsquedas de información en motores de búsqueda para que inmediatamente darle 2 formatos para la carga de teléfonos y otro para la carga de correos. Cuando ya se tiene cargado toda información, en caso la cartera sea AFP se remite la información de deudores con sus correos para que la misma entidad AFP envíe un correo inicial que permite iniciar con la gestión, en paralelo se genera un reporte (mapeo inicial) para que el supervisor de cartera realice análisis y segmentación para luego asignarlo a los asesores esta información se reenvía a los asistentes de TI para realizar la asignación en la base de datos, 
En el caso de la cobranza AFP se solicita el pago de la deuda AFP y de los gastos administrativos y en la cobranza consumo se solicita el pago de la deuda total. Continuando con la gestión, se envía correos masivos a todos los deudores, los asesores realizan llamadas a través del sistema y guardan la gestión obtenida por la llamada, registrando el tipo de contacto obtenido; en caso tengan una llamada con contacto exitoso y el deudor acepta un compromiso, se procede a generar un compromiso de pago en el sistema, para que luego se genere un recordatorio de pago en la fecha prometida, en caso el deudor requiera una excepción el asesor lo derivara con su supervisor para que pueda dar el alta o en todo caso se niega la excepción, si se acepta se procede a generar un compromiso de pago, si se niega se continua con la negociación.
Para finalizar, en el caso de AFP la cobranza finaliza cuando se cancela la deuda de AFP y la deuda de gastos administrativos, cuando el deudor realiza el abono de la deuda o del compromiso generado, se tipifica dentro del sistema como pagado y su supervisor valida el pago, y se cambia de estado al deudor para que ya no reciba gestión tecnológica, para la deuda consumo se solicita la carta de no adeudo y luego de 7 días se hace entrega de la carta de no adeudo mediante correo electrónico.
Se finaliza la campaña con un reporte total del comportamiento de la cartera, con una comparación de los últimos 3 meses.

1.2.2 PROCESO DE COBRANZA (TO-BE)

1.3 MOTIVACIÓN

3. REQUERIMIENTOS
2.1 USUARIOS DEL SISTEMA
2.1 REQUERIMIENTOS FUNCIONALES
2.2 REQUERIMIENTOS DE ATRIBUTOS DE CALIDAD
2.3 RESTRICCIONES 
3.MÓDULOS
3.1 Arquitectura de módulos
3.2 Especificación de módulos
8. PROTOTIPOS
9. MODELAMIENTO CONCEPTUAL
10. DOCUMENTACIÓN DE RELACIONES Y REGLAS DE NEGOCIO
11. DICCIONARIO DE DATOS
