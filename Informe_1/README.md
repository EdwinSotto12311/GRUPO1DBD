# **GI CORONADO CONTACT CENTER S.A.C.**

## 1. DESCRIPCIÓN DE LA EMPRESA
La empresa está conformada por un sólido equipo humano con amplia trayectoria, brindando servicios de gestión en cobranzas en el sector público y privado. El éxito de la empresa se debe a la inteligencia financiera implementada que les permite clasificar a los clientes como buenos o malos pagadores, con el objetivo de la concreción de pago, maximizando y garantizando los resultados en la recuperación de deudas. Además, que cuenta con una gran variedad de canales de contacto, como el call center, SMS, WhatsApp, boots, email y redes sociales, los cuales son seleccionados de acuerdo al tipo de cliente.

### 1.1. DATOS DE LA EMPRESA
* Nombre de la empresa: GI CORONADO CONTACT CENTER
* RUC: 20609129922
* Razón social: GI CORONADO CONTACT CENTER S.A.C.
* Tipo de empresa: Sociedad Anónima Cerrada
#### 1.1.2.	Misión
Satisfacer las necesidades y expectativas de nuestros clientes, colocando a su disposición todo un equipo de trabajo, integrado por recursos humanos, físicos y técnicos en pro de la defensa, protección y recuperación de sus intereses patrimoniales.
#### 1.1.3.	Visión
Ser una empresa líder en el sector de cobranzas, ventas, ferias internacionales y contact center en constante innovación de su proceso, tecnología y equipo humano.
#### 1.1.4.	Valores
* Compromiso
* Eficiencia
* Servicio
* Honestidad
* Transparencia
* Solidaridad

### 1.2.	DESCRIPCION DEL PROCESO DE NEGOCIO (AS-IS)
El proceso de negocio elegido es todo el proceso de cobranzas de deuda consumo desde la preparación de la información recibida por la entidad tercerizadora, pasando por la gestión de llamadas y gestión masivas, hasta el cierre de la cobranza con la emisión de reportes y la emisión y envío de la carta de no adeudo.
#### 1.2.1.	Proceso de Cobranza (AS-IS)
Actualmente la empresa realiza su gestión de cobranza consumo a través de un sistema web propio y mediante un proceso previo manual que realiza el área de ti para cargar datos del deudor, su deuda y montos de campaña.
El proceso inicia con la recepción mediante correo electrónico de las bases de la campaña del mes correspondiente, este correo lo recibe el supervisor de cartera y el jefe del área de TI, se deriva con los asistentes de TI quienes se encargan de la creación de la campaña del mes, para darle formato, a la información recibida, de una plantilla que ya manejan para las cargas de “Obligaciones” en formato separado por comas (.csv), inicia con la carga de estas “Obligaciones” en lo que es la Campaña del mes. 
Luego, dentro de la información recibida se encuentra el detalle de los deudores con números de contacto y correo personal, esta información se trabaja realizando búsquedas de información en motores de búsqueda para que inmediatamente darle 2 formatos para la carga de teléfonos y otro para la carga de correos. Cuando ya se tiene cargado toda información, en paralelo se genera un reporte (mapeo inicial) para que el supervisor de cartera realice análisis de estrategias y segmentación para luego asignarlo a los asesores esta información se reenvía a los asistentes de TI para realizar la asignación de los asesores y la segmentación de las estrategias brindadas en la base de datos, 
En la cobranza consumo se solicita el pago de la deuda total. Continuando con la gestión, se envía correos masivos a todos los deudores, los asesores realizan llamadas a través del sistema y guardan la gestión obtenida por la llamada, registrando el tipo de contacto obtenido; en caso tengan una llamada con contacto exitoso y el deudor acepta un compromiso, se procede a generar un compromiso de pago en el sistema, para que luego se genere un recordatorio de pago en la fecha prometida, en caso el deudor requiera una excepción el asesor lo derivara con su supervisor para que pueda dar la aprobación o en todo caso se niega la excepción, si se acepta se procede a generar un compromiso de pago, si se niega se continua con la negociación.
Para finalizar, cuando el deudor realiza el abono de la deuda o del compromiso generado, se tipifica dentro del sistema como pagado y su supervisor valida el pago, y se cambia de estado al deudor para que ya no reciba gestión tecnológica, se solicita la carta de no adeudo a la entidad que compro la deuda y luego de 7 días se hace entrega de la carta de no adeudo mediante correo electrónico. Se generan reportes semanales para validar el comportamiento de cartera y aplicar nuevas estrategias para la cobranza durante la semana.
Se finaliza la campaña con un reporte total del comportamiento de la cartera.

### 1.3.	Proceso (BPM)

### 1.4.	Proceso de Cobranzas Consumo – Reestructuración de cobranza consumo (TO-BE)
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


### 1.5 MOTIVACIÓN
La elección de la empresa de cobranzas se dio porque no había otra propuesta donde nos brinden toda la información relacionada; se llego a contactar con Oscar Cuba que laboro en el año 2022 por un periodo de 6 meses y tuvo la predisposición de brindarnos la entrevista, la información del proceso de cobranzas nos genero mayor curiosidad y nos animamos por el proceso de cobranzas de cartera consumo.

## 2. REQUERIMIENTOS
### 2.1 USUARIOS DEL SISTEMA
+ **Supervisor**
Este rol es el encargado de validar que el proceso de gestión por parte de los asesores se realice de manera correcta, analiza los reportes para asignar la gestión adecuada según los criterios que valide en los reportes, toda esta información es enviada a los asistentes de ti y a los asesores, podrá aprobar estados de excepciones y de pago y aceptara la emisión de la carta de no adeudo, además que el también podrá gestionar a los deudores que no puedan gestionar los asesores. 

+ **Ejecutor**
Este rol es el encargado de ejecutar la gestión por llamadas, sigue las indicaciones del supervisor y puede visualizar la información de los deudores, llamarlos hasta generar el pago o en tal caso un compromiso de pago, es intermediario del deudor con el supervisor para poder aprobar las excepciones solicitadas 

+ **Soporte**
Este rol es el encargado de preparar toda la información para iniciar la gestión inicial de una nueva entidad, desde la creación de personas y entidades, además atenderá a las solicitudes del supervisor y de preparar la información para realizar la gestión masiva mediante correos y para finalizar genera los reportes necesarios para el análisis del supervisor. 

### 2.1 REQUERIMIENTOS FUNCIONALES
* REQ-01: Creación de registros de información para la gestión
1. Caso de Uso	Gestionar la campaña por llamadas siguiendo los filtros que el supervisor generó en su análisis
2. Descripción del Caso de Uso
El sistema permitirá ingresar el usuario de ejecutor donde le mostrará solo las opciones que le permite su rol, por el que podrá movilizarse entre las campañas asignadas y colocarse en el filtro que por indicación del supervisor podrá gestionar llamada tras llamada por cada deudor, permitiéndole registrar el tipo de respuesta que le brindo su gestión, los compromisos y registrar pagos que indican los deudores.
3. Actor
Soporte
4. Flujo Regular		
Paso 1
Acción del actor
El ejecutor ingresa con su usuario y contraseña al sistema.
Respuesta
El sistema muestra el menú de tareas que corresponde al usuario ejecutor.
Paso 2
Acción del actor
El ejecutor ingresa al módulo de gestión de campañas.
Respuesta
El sistema muestra una lista desplegable con las campañas activas asignadas al ejecutor.
Paso 3
Acción del actor
El ejecutor selecciona la campaña, coloca el filtro a posicionarse y da clic en el botón iniciar gestión
Respuesta
El sistema muestra los datos de la deuda con la información del deudor, permitiendo llenar datos de respuesta de la gestión. El sistema activa el botón registrar gestión.
Paso 4
Acción del actor
El ejecutor da clic en el botón de registrar gestión.
Respuesta
El sistema guarda la información registrada y notifica el registro exitoso y automáticamente avanza al siguiente deudor.

6. Flujo Alternativo	
Paso 3
Acción del actor
El Ejecutor podrá registrar un compromiso, excepción o un pago.
Respuesta
El sistema muestra las casillas a rellenar dependiendo del tipo de registro.
Paso 4
Acción del actor
El ejecutor realiza el registro y da en el botón aceptar.
Respuesta
El sistema notifica el registro con éxito y finaliza la gestión, automáticamente avanza al siguiente deudor.

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
1. Caso de Uso 
Generación de reportes 
2. Descripción del Caso de Uso 
El sistema permite generar reportes del estado de la campaña, de la cartera y del recaudo de los asesores, de la cantidad de llamadas realizadas por los asesores y de la gestión con los datos del contacto de cada deudor. 
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
El soporte ingresa al módulo de generación de reportes. 
Respuesta:
El sistema muestra opciones de generación de reportes del estado de la campaña, de la cartera y del recaudo de los asesores, de la cantidad de llamadas realizadas por los asesores y de la gestión con los datos del contacto de cada deudor. 

Paso 3 
Acción del actor:
El soporte selecciona el tipo de reporte para descargar. 
Respuesta:
El sistema mostrará el reporte que se desea descargar. 

Paso 4 
Acción del actor:
El soporte visualizará el reporte y presionará el botón de descargar. 
Respuesta:
El sistema descargará el reporte en formato de excel. Finaliza la tarea.  

5. Flujo Alternativo 
Paso 3 
Acción del actor:
El soporte presiona el botón Imprimir.  
Respuesta:
El sistema descarga el reporte en formato PDF, finalizando la tarea
 
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
El sistema permitirá al personal de soporte, que cuenta con un rol específico, configurar y gestionar la automatización de la gestión tecnológica masiva mediante la subida de archivos CSV en la página web. Estos archivos CSV se envían automáticamente a proveedores externos seleccionados para ejecutar llamadas automáticas, envío de correos masivos y mensajes SMS a los deudores. El personal de soporte puede definir detalles como el tipo de gestión, el proveedor disponible, el mensaje a enviar, y el nombre de la gestión para su reconocimiento. Además, puede monitorear en tiempo real el estado del servicio proporcionado por el proveedor y descargar los resultados una vez estén disponibles
Actor: Personal de soporte
Flujo Regular:

Paso 1:El Personal de Soporte inicia sesión en el sistema.
Respuesta: El sistema autentica al usuario y muestra el menú de tareas correspondiente.

Paso 2: El Personal de Soporte selecciona "Opciones y Configuración de Tercerización de Mensajes Automáticos". 
Respuesta: El sistema muestra las opciones disponibles, incluyendo "Archivos Recibidos". 

Paso 3: El Personal de Soporte hace clic en "Archivos Recibidos". 
Respuesta: El sistema proporciona una opción para comprimir los archivos recibidos en formato ZIP. El Personal de Soporte descarga los archivos CSV correspondientes a cada tipo de gestión. 

Paso 4: El Personal de Soporte regresa a la sección de configuración y hace clic en "Configuración de Mensajes". 
Respuesta:El sistema muestra una interfaz para configurar mensajes automáticos.

Paso 5: El Personal de Soporte carga un archivo CSV y selecciona el tipo de gestión. Luego, elige "Filtros Personalizados" y completa los datos del deudor y del asesor. Se añade la estructura del mensaje predeterminado. 
Respuesta: El sistema permite agregar el mensaje y guarda la configuración 

Paso 6: El Personal de Soporte selecciona "Filtros Masivos". Sube archivos de lista de datos de asesores y sus días disponibles. Configura el rango de montos, fecha de envío y días de disponibilidad. Luego, añade la estructura del mensaje predeterminado. 
Respuesta:El sistema permite generar un documento CSV con los mensajes configurados. 

Paso7: El Personal de Soporte accede a la interfaz de selección de proveedor, carga el documento CSV generado y selecciona el tipo de gestión. Ingresa el nombre del proveedor, fecha de servicio, nombre del personal de soporte, número de servicio e indicaciones adicionales. 
Respuesta: El sistema envía el archivo CSV y las indicaciones al proveedor externo. 

Paso 8: El Personal de Soporte hace clic en "Monitoreo" y proporciona el número de servicio y fecha 
Respuesta: El sistema muestra los resultados del proveedor en tiempo real. 

Paso 9: Cuando el proveedor finaliza, el Personal de Soporte descarga los archivos de resultados haciendo clic en un botón correspondiente en la página de monitoreo. 
Respuesta: Se descarga correctamente el archivo csv con los resultados. 

Flujo Alternativo:

Paso 5: El Personal de Soporte carga un archivo CSV incorrecto o ingresa información incorrecta en la configuración de mensajes automáticos 
Respuesta: El sistema detecta que el archivo CSV subido no cumple con los requisitos o que la información ingresada es incorrecta 

Paso 6: Descargar Archivos de Resultados sin haber terminado el servicio.
Respuesta: El sistema notifica la falta de documento csv debido a que el proveedor aun no envia resultados.

* REQ-06: Gestión telefónica por deudor
  1. Caso de Uso	Gestionar la campaña por llamadas siguiendo los filtros que el supervisor generó en su análisis
2. Descripción del Caso de Uso
El sistema permitirá ingresar el usuario de ejecutor donde le mostrará solo las opciones que le permite su rol, por el que podrá movilizarse entre las campañas asignadas y colocarse en el filtro que por indicación del supervisor podrá gestionar llamada tras llamada por cada deudor, permitiéndole registrar el tipo de respuesta que le brindo su gestión, los compromisos y registrar pagos que indican los deudores.
3. Actor
Soporte
4. Flujo Regular	
Paso 1		
Acción del actor
El ejecutor ingresa con su usuario y contraseña al sistema.
Respuesta
El sistema muestra el menú de tareas que corresponde al usuario ejecutor.
Paso 2		
Acción del actor
El ejecutor ingresa al módulo de gestión de campañas.
Respuesta
El sistema muestra una lista desplegable con las campañas activas asignadas al ejecutor.
Paso 3		
Acción del actor
El ejecutor selecciona la campaña, coloca el filtro a posicionarse y da clic en el botón iniciar gestión
Respuesta
El sistema muestra los datos de la deuda con la información del deudor, permitiendo llenar datos de respuesta de la gestión. El sistema activa el botón registrar gestión.
Paso 4	
Acción del actor	
El ejecutor da clic en el botón de registrar gestión.
Respuesta
El sistema guarda la información registrada y notifica el registro exitoso y automáticamente avanza al siguiente deudor.
Acción del actor

5. Flujo Alternativo
Paso 3		
Acción del actor
El Ejecutor podrá registrar un compromiso, excepción o un pago.
Respuesta
El sistema muestra las casillas a rellenar dependiendo del tipo de registro.
Paso 4		
Acción del actor
El ejecutor realiza el registro y da en el botón aceptar.
Respuesta
El sistema notifica el registro con éxito y finaliza la gestión, automáticamente avanza al siguiente deudor.

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
* REQ-01: Creación de registros de información para la gestión
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966974/2afbcfc5-efba-4610-96d2-23fef66b8161)
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966974/3955199d-1d49-4d1e-b0b9-a73f62d1a841)

* REQ-02: Cargas masivas de información de la campaña y del deudor 
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/82728541/23de51aa-cca5-44b8-9cc1-d14b2c268fde)
* REQ-03: Generación de reportes
![Reportes](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966392/80c66e28-cfe5-4a34-8626-47ef589b8388)
* REQ-04: Asignación y generación de estrategias
![PROTOTIPO1](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/90528509/04225d18-c61c-4716-937c-d9aa012ece07)
![PROTOTIPO2](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/90528509/24b268fb-c2f5-433c-8179-3c93e98e6cb9)
* REQ-07: Validación de excepciones, pagos y finalización del proceso de cobranza
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/12478357-9dff-432c-9ed5-e5b2f6dcdf67)
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/719f3e85-8cc5-495d-a50c-62585c0ddb41)
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/022ea929-55aa-43cc-8d10-517eb3e0cce2)
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/9430fdb9-73b2-4b5c-994d-25b27326eb79)
* REQ-06: Gestión telefónica por deudor
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966974/9c6383fa-688f-469c-b782-6916b00029ab)

9. MODELAMIENTO CONCEPTUAL
10. DOCUMENTACIÓN DE RELACIONES Y REGLAS DE NEGOCIO
11. DICCIONARIO DE DATOS

