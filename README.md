# GRUPO1DBD
Grupo 1 Diseño de Base de Datos 

1. DESCRIPCIÓN DE LA EMPRESA
   La empresa está conformada por un sólido equipo humano con amplia trayectoria, brindando servicios de gestión en cobranzas en el sector público y privado. El éxito de la empresa se debe a la inteligencia financiera implementada que les permite clasificar a los clientes como buenos o malos pagadores, con el objetivo de la concreción de pago, maximizando y garantizando los resultados en la recuperación de deudas. Además, que cuenta con una gran variedad de canales de contacto, como el call center, SMS, WhatsApp, boots, email y redes sociales, los cuales son seleccionados de acuerdo al tipo de cliente. 
1.1 DATOS DE LA EMPRESA
	Nombre de la empresa: GI CORONADO CONTACT CENTER
	RUC: 20609129922
	Razón social: GI CORONADO CONTACT CENTER S.A.C.
	Tipo de empresa: Sociedad Anónima Cerrada
1.1.2.	Misión
Satisfacer las necesidades y expectativas de nuestros clientes, colocando a su disposición todo un equipo de trabajo, integrado por recursos humanos, físicos y técnicos en pro de la defensa, protección y recuperación de sus intereses patrimoniales.
1.1.3.	Visión
Ser una empresa líder en el sector de cobranzas, ventas, ferias internacionales y contact center en constante innovación de su proceso, tecnología y equipo humano.
1.1.4.	Valores
	Compromiso
	Eficiencia
	Servicio
	Honestidad
	Transparencia
	Solidaridad

1.2.	DESCRIPCION DEL PROCESO DE NEGOCIO (AS-IS)
El proceso de negocio elegido es todo el proceso de cobranzas de deuda consumo desde la preparación de la información recibida por la entidad tercerizadora, pasando por la gestión de llamadas y gestión masivas, hasta el cierre de la cobranza con la emisión de reportes y la emisión y envío de la carta de no adeudo.
1.2.1.	Proceso de Cobranza (AS-IS)
Actualmente la empresa realiza su gestión de cobranza consumo a través de un sistema web propio y mediante un proceso previo manual que realiza el área de ti para cargar datos del deudor, su deuda y montos de campaña.
El proceso inicia con la recepción mediante correo electrónico de las bases de la campaña del mes correspondiente, este correo lo recibe el supervisor de cartera y el jefe del área de TI, se deriva con los asistentes de TI quienes se encargan de la creación de la campaña del mes, para darle formato, a la información recibida, de una plantilla que ya manejan para las cargas de “Obligaciones” en formato separado por comas (.csv), inicia con la carga de estas “Obligaciones” en lo que es la Campaña del mes. 
Luego, dentro de la información recibida se encuentra el detalle de los deudores con números de contacto y correo personal, esta información se trabaja realizando búsquedas de información en motores de búsqueda para que inmediatamente darle 2 formatos para la carga de teléfonos y otro para la carga de correos. Cuando ya se tiene cargado toda información, en paralelo se genera un reporte (mapeo inicial) para que el supervisor de cartera realice análisis de estrategias y segmentación para luego asignarlo a los asesores esta información se reenvía a los asistentes de TI para realizar la asignación de los asesores y la segmentación de las estrategias brindadas en la base de datos, 
En la cobranza consumo se solicita el pago de la deuda total. Continuando con la gestión, se envía correos masivos a todos los deudores, los asesores realizan llamadas a través del sistema y guardan la gestión obtenida por la llamada, registrando el tipo de contacto obtenido; en caso tengan una llamada con contacto exitoso y el deudor acepta un compromiso, se procede a generar un compromiso de pago en el sistema, para que luego se genere un recordatorio de pago en la fecha prometida, en caso el deudor requiera una excepción el asesor lo derivara con su supervisor para que pueda dar la aprobación o en todo caso se niega la excepción, si se acepta se procede a generar un compromiso de pago, si se niega se continua con la negociación.
Para finalizar, cuando el deudor realiza el abono de la deuda o del compromiso generado, se tipifica dentro del sistema como pagado y su supervisor valida el pago, y se cambia de estado al deudor para que ya no reciba gestión tecnológica, se solicita la carta de no adeudo a la entidad que compro la deuda y luego de 7 días se hace entrega de la carta de no adeudo mediante correo electrónico. Se generan reportes semanales para validar el comportamiento de cartera y aplicar nuevas estrategias para la cobranza durante la semana.
Se finaliza la campaña con un reporte total del comportamiento de la cartera.

1.3.	Proceso (BPM)

1.4.	Proceso de Cobranzas Consumo – Reestructuración de cobranza consumo (TO-BE)
Se considero todo el proceso de cobranzas de consumo para tener un mayor alcance del proceso, además se consideró que la empresa sea la que adquiere las deudas y no es tercerista, además que los procesos manuales de envíos de herramientas masivas se realicen desde el mismo sistema, automatización de reportes y emisión y envío de cartas de no adeudo.
El proceso iniciaría con el asistente de ti generando por encargo la creación de las entidades que interactuaran con la gestión, al iniciar con una cartera propia se generaría la entidad bancaria de donde se adquirió las deudas, para luego crear la cartera correspondiente y por consiguiente la creación de campaña, se crean las personas que ocuparan el rol de supervisor, asesor y asistente de ti. Para luego asignarles a cada asesor su deudor de la campaña activa.
Se carga la información de la campaña con los datos de la deuda, datos personales y los datos de contacto. Al tener todos los datos cargados el supervisor de cartera extrae el reporte del estado de la campaña para generar un análisis del estado inicial para generar una distribución de que deudores se les realizara el cobro por gestión d llamadas o gestión de herramientas masivas, al inicio de la cartera se envía una gestión de correos masivos a toda la campaña, en caso no sea el inicio de la cartera se seguirán las estrategias del supervisor y se enviaran las gestiones masivas de pendiendo de los criterios indicados, 
La gestión de llamadas inicia y los asesores deben posicionar en el filtro indicado por el supervisor, comienza la gestión con las llamadas a los teléfonos registrados con el deudor hasta tener una respuesta directa indirecta o hasta que se acaben las opciones de llamadas, si no se obtiene respuesta pasas al siguiente deudor, si obtienes respuesta pueden ocurrir  escenarios, uno que te brinden información adicional del deudor, que solicite una excepción o que solicite un compromiso de pago, se registra la gestión, en caso el deudor requiera una excepción esta tendrá que ser validada por el supervisor en caso ser aprobada se comunica al deudor y se registra su compromiso, En caso el deudor pague su compromiso se registra el pago y guarda gestión. 
El supervisor valida el pago y en caso de ser cancelación total aprueba la emisión y el envío de la carta de no adeudo.
Finaliza la campaña con el reporte de cierre, donde además muestra una lista de los deudores que tienen compromisos y negociaciones de pago.
Se identificaron 3 actores o usuarios: Asistente de TI, Asesor y Supervisor. 
, los clientes pueden pagar sus deudas de manera conveniente y recibir recordatorios automáticos. Esto nos ayuda a recuperar deudas más rápido y a dar un mejor servicio a los clientes.

ACTIVIDADES
1.	Creación Entidad, Cartera y Campaña:
Iniciamos con la creación de una nueva entidad(origen) de cuentas por cobrar, luego la cartera relacionada con la entidad para finalmente crear la campaña del mes correspondiente. En caso la entidad y la cartera ya estén creadas solo se creará la campaña.
2.	Creación Persona y asignación de Asesores con Campaña:
Se añaden las personas relacionadas a la gestión de la campaña, que pueden ser asesores, supervisor y asistente de ti.
A cada asesor añadido se asigna la campaña con la que trabajara.
3.	Cargas de Campaña
Se carga la información de la campaña con los datos de la deuda, deuda total, deuda capital, descuento por campaña, y más datos.
4.	Carga de Teléfono y E-mail:
Se relaciona cada teléfono con el deudor y se realiza la carga masiva.
Se relación los correos con los deudores y se realizan la carga masiva.
5.	Carga Datos Deudores:
Se carga los datos de los deudores como el nombre, información personal, documento de identidad y otros.
6.	Reporte Estado Campaña
Se emite un reporte del estado actual de la campaña si es al inicio ayudara para la segmentación de la campaña y las estrategias a aplicar.
7.	Reporte recaudo:
Se emite el reporte de la cartera y del recaudo de los asesores, no se da al inicio de la gestión sino en el proceso.
8.	Reporte llamadas:
Se emite un reporte de la cantidad de llamadas realizadas por los asesores, el estado de contacto de la gestión y mide el rendimiento del asesor.
9.	Reporte de gestión:
Se emite un reporte de la gestión con los datos del contacto de cada deudor.
10.	Asignación de Gestiones
El supervisor analiza el reporte de estado de la campaña y segmenta la cartera para gestión por llamadas y gestión masiva.
11.	Generación de Estrategias
En caso la campaña sea inicial se generará una estrategia, esto varia dependiendo el comportamiento de la campaña según el reporte de estado de la campaña.
12.	Envío de correo masivos
Al inicio de la campaña se envía a todos los deudores para coberturar la campaña, luego se envían según las estrategias del supervisor.
13.	Envío de llamadas masivas 	
Se envían las llamadas masivas hacia los deudores con una redirección al anexo del asesor asignado según las indicaciones del supervisor.
14.	Envío de SMS masivo
Se envían los SMS masivos dirigidas al asesor asignado según las indicaciones del supervisor.
15.	Inicio de Gestión
Los asesores ajustan sus filtros de gestión según las indicaciones del supervisor, e inician la gestión con el primer deudor en la lista y generando su primera llamada.
16.	Actualización de Datos de contacto
En caso de que reciban una actualización de los datos de contacto durante la gestión los asesores podrán registrarlo, o cambiar el estado.
17.	Registro excepciones y compromisos
Cuando se tenga un contacto positivo y el deudor tenga problemas para cancelar con el monto indicado, se podrá solicitar una excepción de pago, esta excepción es enviada al supervisor para su aprobación si se aprueba se podrá generar un compromiso de pago, en caso el deudor se comprometa a pagar se registra el compromiso.
18.	Registro pago
Cuando el deudor pague su monto de promesa el asesor registra en el sistema para su validación por parte del supervisor.
19.	Registro de Gestión
El asesor registrara la gestión dependiendo de la respuesta obtenida si el deudor genera un compromiso, un contacto indirecto, una negativa de pago o desinterés se registrará y se pasara con el siguiente deudor.
20.	Validación de excepciones y pagos:
El supervisor podrá visualizar las solicitudes de excepciones de pago el cual podrá aprobar o rechazar, de igual forma con el pago valida el pago y en caso no se valide la tipificación registrada de la gestión cambiará.
21.	Emisión y envío CNA
Cuando el deudor cancela la totalidad de la deuda se valida y se aprueba la emisión para un próximo envío de la carta de no adeudo.
22.	Reporte Cierre de Campaña
Al finalizar la campaña el supervisor solicitará el reporte de cierre donde podrá revisar el desempeño de la campaña y además generar un reporte de los compromisos a plazos generados para mantenerlos con los asesores que cerraron el compromiso.


1.5 MOTIVACIÓN
Estamos emocionados de hacer esta mejora en la empresa de cobranza porque creemos que hará que la vida de los clientes morosos sea más fácil ya que, a pesar de ser deudores, no se sentirán tan acosados o presionados para pagar su deuda; por otro lado, la empresa será más eficiente y ayudará a reducir los costos tantos en llamadas como en otros servicios que realizan para esta gestión de cobranza. Con un portal web, los clientes pueden pagar sus deudas de manera conveniente y recibir recordatorios automáticos. Esto nos ayuda a recuperar deudas más rápido y a dar un mejor servicio a los clientes.

2. REQUERIMIENTOS
2.1 USUARIOS DEL SISTEMA
   Deudor  
Este rol es el que va a validar por su propia cuenta en la página web si figura 		como deudor, en caso se encuentre podrá visualizar la información de su deuda, 		gestionarla él mismo, solicitar compromisos o excepciones de pago o ser 			atendido por un asesor, realizar el pago mediante los diferentes métodos y 		formas de pago, y por último confirmar el pago cargando su comprobante de 		pago.

   Asesor 
Este rol es el encargado de dar un soporte a todos los deudores que tengan un rango de deuda entre <1000, mas>, que se encuentre en un rango de edad de <22,45> y que tengan números de contactos, aquellos que no tienen número de contacto y si tienen correo, se gestionan por este último medio.
Una vez se envían correos masivos a todos los deudores sin excepción, los asesores realizan llamadas a través del sistema y guardan la gestión obtenida por la llamada, en caso tengan una llamada con contacto exitoso y el deudor acepta un compromiso, se procede a generar un compromiso de pago en el sistema, para que luego se genere un recordatorio de pago en la fecha prometida, en caso el deudor requiera una excepción el asesor lo derivara con su supervisor.

   Supervisor 
Este rol es el encargado que podrá aprobar  las solicitudes de los deudores, asignar los deudores que generaron compromisos a asesores y los deudores que no generaron ninguna solicitud también asignarla a los asesores ,ya que se registró con un numero de contacto, se tipifica dentro del sistema como pagado y su supervisor valida el pago, y se cambia de estado al deudor para que ya no reciba gestión tecnológica, se solicita la carta de no adeudo y luego de 7 días se hace entrega de la carta de no adeudo mediante correo electrónico.

2.1 REQUERIMIENTOS FUNCIONALES
* REQ-01: Creación de registros de información para la gestión 

* REQ-02: Cargas masivas de información de la campaña y del deudor 
1. Caso de Uso 
Cargas masivas de información de la campaña y del deudor 
2. Descripción del Caso de Uso 
El sistema permite subir distintas cargas de información de los deudores, formas de contacto y las campañas con sus respectivos datos relacionados desde los Excel iniciales que proveen los clientes al sistema, modificando que encajen los datos principales. 
3. Actor 
Soporte 
4. Flujo Regular 
Paso 1 
Acción del actor:
El soporte ingresa con su usuario y contraseña al sistema. 
Respuesta:
El sistema muestra el menú de tareas que corresponde al usuario soporte. 

Paso 2 
Acción del actor:
El soporte ingresa al módulo de carga de datos 
Respuesta:
El sistema muestra opciones de carga de datos de deudores, carga de formas de contacto y cargas de campañas 

Paso 3 
Acción del actor:
El soporte selecciona el tipo de carga de datos a subir 
Respuesta:
El sistema mostrara un botón a subir la carga de datos 

Paso 4 
Acción del actor:
El soporte sube la carga de datos seleccionada 
Respuesta:
El sistema mostrara una sección con los datos subidos en columnas ya establecidas. 

Paso 5 
Acción del actor:
El soporte revisa si los datos cargaron correctamente según las columnas, si esta todo conforme presiona el botón guardar 
Respuesta:
El sistema finaliza la operación, guarda los datos cargados y muestra la pantalla de opciones del soporte 

5. Flujo Alternativo 
Paso 5 
Acción del actor:
El soporte revisa si los datos cargaron correctamente según las columnas, si no está todo conforme selecciona el botón de cancelar, para modificar el Excel que iba a subir. 
Respuesta:
El sistema cancela la carga de datos y regresa a la pantalla de opciones del soporte 


* REQ-03: Generación de reportes 

* REQ-04: Asignación y generación de estrategias 
1. Caso de Uso 
Asignación y generación de estrategias
2. Descripción del Caso de Uso 
El sistema permitirá segmentar la cartera para gestión por llamadas o gestión masiva a través del reporte de Estado y reporte de Gestión.
3. Actor 
Supervisor
4. Flujo Regular 
Paso 1 
Acción del actor: El Supervisor ingresa con su usuario y contraseña al sistema. 
Respuesta: El sistema muestra el menú de tareas que corresponde al módulo Supervisor. 

Paso 2 
Acción del actor: El Supervisor ingresa al módulo de Generación de Estrategias. 
Respuesta: El sistema muestra un menú vertical donde están las opciones de Reporte de Estado y Reporte de Gestión para elegir.  

Paso 3 
Acción del actor: El Supervisor selecciona el tipo de Reporte que desea analizar. 
Respuesta: El sistema nos muestra una lista de elementos donde están las opciones en cual se segmento la cartera en general.  

Paso 4 
Acción del actor: El Supervisor selecciona una opción de segmentación de cartera.
Respuesta: El sistema nos muestra una tabla en donde está clasificado la cartera según la opción de segmentación seleccionada y en cada clase se indica la cantidad de deudores, recorrido, monto y cantidad de pagos. 

Paso 5 
Acción del actor: El supervisor selecciona con los checkbox las clases en donde desea definir una estrategia de cobranza. 
Respuesta: El sistema habilita en la parte superior derecha el menú vertical y los dos campos de textos, y en donde se podrá seleccionar el tipo de gestión, ingresar el nombre de estrategia y su fecha y hora programada correspondientemente. 

Paso 6
Acción del actor: El supervisor ingresa lo pedido y hace clic en el botón Asignar.  
Respuesta: El sistema guarda las estrategias generadas, finaliza la tarea. 

5. Flujo Alternativo 
Paso 6
Acción del actor: El Supervisor no ingresa los datos solicitados. Presiona botón Atrás.
Respuesta: El sistema no realiza ningún guardado, finaliza la tarea. 


* REQ-05: Gestión tecnológica masiva 
Caso de Uso: Gestión Tecnológica Masiva
Descripción del Caso de Uso: Este caso de uso permite a los miembros del área de TI gestionar de manera masiva las llamadas automáticas y el envío de correos masivos a los deudores de la empresa de cobranzas. El proceso implica la carga de archivos CSV específicos que contienen información detallada para programar las llamadas y los correos masivos.
Actor: Miembros del área de TI de la empresa de cobranzas.
Flujo Regular:

Paso 1: El actor (miembro del área de TI) inicia sesión en el módulo de gestión tecnológica masiva.

Acción del actor: Inicia sesión en el sistema.
Respuesta: El sistema muestra el menú de opciones de gestión tecnológica masiva.
Paso 2: El actor selecciona la opción de cargar un archivo CSV para las llamadas automáticas.

Acción del actor: Selecciona la carga de llamadas automáticas y carga el archivo CSV.
Respuesta: El sistema procesa el archivo CSV y muestra una vista previa de las llamadas programadas.
Paso 3: El actor selecciona la opción de cargar un archivo CSV para el envío de correos masivos.

Acción del actor: Selecciona la carga de correos masivos y carga el archivo CSV.
Respuesta: El sistema procesa el archivo CSV y muestra una vista previa de los correos masivos programados.
Paso 4: El actor revisa las programaciones y verifica que los datos sean correctos.

Acción del actor: Verifica las programaciones de llamadas y correos masivos.
Respuesta: El sistema muestra las programaciones verificadas.
Paso 5: El actor confirma las programaciones para la ejecución.

Acción del actor: Confirma las programaciones para su ejecución.
Respuesta: El sistema programa automáticamente las llamadas y envía los correos masivos según lo programado.
Flujo Alternativo:

Paso 4: En caso de que los archivos CSV no sean válidos o contengan datos incorrectos, el sistema mostrará un mensaje de error.

Acción del actor: Verifica los mensajes de error y ajusta los archivos CSV según sea necesario.
Respuesta: El sistema muestra un mensaje de error y no realiza ninguna programación hasta que los archivos sean válidos.
Paso 5: Si los miembros del área de TI identifican problemas en las programaciones, pueden realizar ajustes y volver a verificar antes de la ejecución.

Acción del actor: Realiza ajustes en las programaciones y verifica nuevamente.
Respuesta: El sistema muestra las programaciones ajustadas para su revisión.

* REQ-06: Gestión telefónica por deudor 

* REQ-07: Validación de excepciones, pagos y finalización del proceso de cobranza
1. Caso de Uso	Validación de excepciones, pagos y finalización del proceso de cobranza
2. Descripción del Caso de Uso
El sistema permite ingresar a la opción de validación de excepciones de pago y verificación del pago realizado por el deudor; si el pago realizado ha cancelado la deuda en su totalidad, se emite la carta de no adeudo.
3. Actor
Supervisor
4. Flujo Regular
Paso 	Acción del actor	Respuesta
Paso 1	El supervisor inicia sesión en el sistema de gestión.	El sistema muestra el menú de opciones correspondiente al supervisor.
Paso 2	El supervisor selecciona la opción “Validación de Excepciones y Pagos” en el menú.	El sistema muestra las solicitudes pendientes de excepciones y pagos.
Paso 3	El supervisor selecciona una solicitud de excepción o pago para revisión.	El sistema muestra los detalles de la solicitud seleccionada.
Paso 4	El supervisor aprueba/rechaza la excepción de pago o estado de pago.	El sistema registra la acción tomada y actualiza el estado de solicitud.
Paso 5	El supervisor selecciona la aprobación de la excepción / El supervisor selecciona la opción de finalización del pago. 	El sistema actualiza el estado de solicitud y registra la fecha del cambio del estado de solicitud.
Paso 6	El supervisor selecciona la opción de generación de compromiso de pago. / El supervisor selecciona la opción de emisión de carta de no adeudo.	El sistema genera el compromiso y fecha de pago. / El sistema genera la carta de no adeudo del deudor y registra fecha de finalización.
Paso 7	El supervisor retrocede a la sección anterior al seleccionar la opción de “Validación de Excepciones y Pagos” en el menú	El sistema regresa a la lista de solicitudes.
Paso 8	El supervisor selecciona la opción “Finalización de campaña” si las deudas están todas pagadas.	El sistema registra la finalización de la campaña y genera un reporte de cierre.
5. Flujo Alternativo		El sistema mostrara un anuncio de registro exitoso.
Paso 	Acción del actor	Respuesta
Paso 5	El supervisor selecciona la opción de rechazo de la excepción de pago. / El supervisor selecciona la opción de no finalización del pago.	El sistema registra y actualiza el estado de la solicitud.

2.2 REQUERIMIENTOS DE ATRIBUTOS DE CALIDAD
Disponibilidad: El sistema estará siempre disponible para que así el deudor pueda validar su deuda y gestionar su compromiso en cualquier momento del día. 
Seguridad: El sistema solo permitirá acceso a usuarios que se han registrado al portal web con sus datos correspondientes como nombres, apellidos y DNI.  
Rendimiento: Se usarán eficazmente los recursos para garantizar que el sistema pueda procesar grandes cantidades de datos y generar reportes de manera rápida y eficiente. 
Adaptabilidad: El sistema debe funcionar principalmente en los siguientes dispositivos electrónicos: Computadora, laptop, Tablet y teléfono inteligente.  
Usabilidad: El sistema es fácil de usar y comprender, con una interfaz amigable tanto para los usuarios y administradores.  
Fiabilidad: El sistema continuará operando así se presenten problemas, para lograr eso se pondrá a prueba continuamente el rendimiento del sistema.  
Escalabilidad: El sistema tendrá la capacidad de trabajar con una gran cantidad de usuarios. 

2.3 RESTRICCIONES 
3.MÓDULOS
3.1 Arquitectura de módulos
3.2 Especificación de módulos

3.2.2Módulo Cargas Masivas 
Descripción: Es el módulo asignado a los de soporte para subir al sistema las distintas cargas de datos (deudor, contacto y campaña) junto con su respectivo chequeo si lo datos concuerdan con las columnas ya establecidas. 
Responsabilidad: 
Realiza la carga de datos (deudor, contacto y campaña) al sistema 
Realiza el chequeo al subir los datos en las columnas respectivas que muestra el sistema 
Realiza las modificaciones en el Excel que muestra errores de datos para volver a subirlo al sistema 
Interacción: 
-Modulo Registros Nuevos 
-Modulo Generación de Reportes 
3.2.4. Módulo Creación de estrategias 
Descripción: 
Es el módulo asignado al supervisor donde se muestra segmentado el reporte de estado y reporte de gestión de la campaña y, donde gracias a esto, el supervisor analizara y generara estrategias 
Responsabilidad: 
Permite visualizar el reporte de estado y el reporte de gestión segmentado de la actual campaña 
Permite el desarrollo, nombramiento y programación de estrategias de cobranza 
Permite el guardado de estrategias en el sistema 
Interacción: 
-Modulo Generación de Reportes  
-Modulo Gestión Masiva 
-Modulo Gestión Unitaria 
3.2.7.	Módulo Validación
Descripción: 
Es el módulo asignado al supervisor para la validación de excepciones de pago, aprobar pagos realizados por los deudores y gestionar la finalización del proceso de cobranza.
Responsabilidad:
Revisa, evalúa y decide las solicitudes de excepciones de pagos pendientes.
Valida y actualiza que los pagos de los deudores sean correctos correspondiente a su deuda.
Comprueba si el deudor completó su deuda para aprobar su emisión de carta de no adeudo
Registra la finalización del proceso de cobranza para el deudor y genera un reporte
Interacción:
-Módulo de Gestión de Cobranza Masiva
-Módulo de Creación de Registros de Información
-Módulo de Generación de Reportes

4. PROTOTIPOS

* REQ-02: Cargas masivas de información de la campaña y del deudor 
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/82728541/23de51aa-cca5-44b8-9cc1-d14b2c268fde)


9. MODELAMIENTO CONCEPTUAL
10. DOCUMENTACIÓN DE RELACIONES Y REGLAS DE NEGOCIO
11. DICCIONARIO DE DATOS
