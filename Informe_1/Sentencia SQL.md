## 15. SENTENCIAS SQL PARA CADA PROTOTIPO
### Módulo registros nuevos
| Codigo Requerimiento | R-01                  |
|-------------|------------------------|
| Codigo Interfaz         | GUI-001_1       |
| Imagen Interfaz                                  |
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/82728541/28c6633d-1729-498e-ac6c-75c1130ac9de)|
| Sentencias SQL                                  |
| 1. Botón Agregar: Se agregará un nuevo registro a la tabla de empleado. |
|INSERT INTO Empleado (Nombres, ApellMat, ApellPat, rol, DNI, usuario, contraseña, id\_empleado) VALUES (<1>, <2>, <3>, <4>, <5>, <6>, <7>, <8>); |
|INSERT INTO Empleado\_email (email, id\_empleado) VALUES (<9>, <8>);|   
|INSERT INTO Empleado\_telefono (telefono, id\_empleado) VALUES (<10>, <8>);| 
|Donde los valores del 1 al 10 se capturarán de la interfaz del soporte según se muestran en la imagen. |


| Codigo Requerimiento | R-01                  |
|-------------|------------------------|
| Codigo Interfaz         | GUI-001_2        |
| Imagen Interfaz                                  |
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/82728541/f839db97-2300-442a-9e6b-c787f93d25ad)|
| Sentencias SQL                                  |
| 1. Botón Agregar: Se agregará un nuevo registro a la tabla de campaña. |
|INSERT INTO Campaña (nombre, fecha\_incio, fecha\_fin, estado, id\_campaña, id\_entfinan) VALUES (<1>, <2>, <3>, <4>, <5>, <6>); |
|Donde los valores del 1 al 6 se capturarán de la interfaz del soporte según se muestran en la imagen. |


| Codigo Requerimiento | R-01                  |
|-------------|------------------------|
| Codigo Interfaz         | GUI-001_3        |
| Imagen Interfaz                                  |
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/82728541/f75188b0-7326-4305-a2cf-e918faf1ef4a)|
| Sentencias SQL                                  |
| 1. Botón Agregar: Se agregará un nuevo registro a la tabla de entidad financiera. |
|INSERT INTO Entidad\_Financiera (nombre, RUC, tipo\_entidad, telefono\_contacto, id\_entfinan) VALUES (<1>, <2>, <3>, <4>, <5>); |
|Donde los valores del 1 al 5 se capturarán de la interfaz del soporte según se muestran en la imagen. |


### Módulo de Generación de Estrategias
|Código de requerimiento|R-04|
|------------------------|----|
|**Código de interfaz**|GUI-004_1|
|Imagen interfaz|
|![Generacion de Estrategias Pantalla1_con numeros](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/90528509/25e0d764-f172-418b-b30b-302ff165ed1b)|
|Sentencia SQL|
|Eventos:|
|1.Carga de Opciones de Tipos de Reporte: Se mostrara la lista de tipos de reportes a seleccionar:
SELECT CODIGO, DESCRIPCION FROM TIPOS_REPORTES;|
|2.Carga de Opciones de Tipos de Segmentacion: Se mostrara la lista de los tipos de segmentacion de Reporte de Estado a seleccionar
SELECT DESCRIPCION FROM TIPOS_SEGMENTACION_ESTADO;|
|3.Botón Buscar: Cuando el usuario presione el botón buscar se llenará la grilla de resultados utilizando la siguiente sentencia:
SELECT RC.descripcion AS Rango_de_Capital, COUNT(D.codigo) AS Cantidad_Deudas, SUM(D.monto_total) AS Monto_Total
FROM RANGO_CAPITALES RC
LEFT JOIN Deuda D ON D.monto_total BETWEEN RC.limite_inferior AND RC.limite_superior
GROUP BY RC.codigo, RC.descripcion
ORDER BY RC.codigo;|
|4.Botón Asignar: Se agregará un nueva estrategia a la tabla de estrategias.
INSERT INTO Estrategia(tipo_gestion,nombre_estrategia, id_estrategia, id_empleado) VALUES (<1>, <2>, <3>, <4>);
Donde los valores del 1 al 4 se capturarán de la interfaz de usuario según se muestran en la imagen.|


|Código de requerimiento|R-04|
|------------------------|----|
|**Código de interfaz**|GUI-004_2|
|Imagen interfaz|
|![Generacion de Estrategias Pantalla 2-con numeros](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/90528509/c3c5d2c2-7635-4a29-aac6-8289f2343197)|
|Sentencia SQL|
|Eventos:|
|1.Carga de Opciones de Tipos de Reporte: Se mostrara la lista de tipos de reportes a seleccionar
SELECT CODIGO, DESCRIPCION FROM TIPOS_REPORTES;|
|2.Carga de Opciones de Tipos de Segmentacion: Se mostrara la lista de los tipos de segmentacion del Reporte de Gestion a seleccionar
SELECT DESCRIPCION FROM TIPOS_SEGMENTACION_GESTION;|
|3.Carga de Opciones del Estado Historico: Se mostrara la lista de las opciones de tablas que se puede mostrar en la segmentacion por Estado Historico
SELECT DESCRIPCION FROM  OPCIONES_ESTADO_HISTORICO;|
|4.Botón Buscar: Cuando el usuario presione el botón buscar se llenará la grilla de resultados utilizando la siguiente sentencia:
SELECT OCI.DESCRIPCION AS Contacto_Indirecto, COUNT(D.codigo) AS Cantidad_Deudas
FROM OPCIONES_CONTACTO_INDIRECTO OCI
LEFT JOIN Deuda D ON D.descripcion = OCI.DESCRIPCION
GROUP BY OCI.codigo, OCI.DESCRIPCION
ORDER BY OCI.codigo;|
|5.Botón Asignar: Se agregará un nueva estrategia a la tabla de estrategias.
INSERT INTO Estrategia(tipo_gestion,nombre_estrategia, id_estrategia, id_empleado)
VALUES (<1>, <2>, <3>, <4>);
Donde los valores del 1 al 4 se capturarán de la interfaz de usuario según se muestran en la imagen|

### MODULO DE GESTION TECNOLOGICA
| Codigo Requerimiento | REQ-05                 |
|-------------|------------------------|
| Codigo Interfaz         | GUI-005-01       |
| Imagen Interfaz                                  |
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/97325341/9f3a3510-d6d9-4a7f-bf19-df563aa20062)|
| Sentencias SQL                                  |
| 1.	Botón Generar Agregar mensaje. |
|INSERT INTO Mensaje (id_mensaje, mensaje_predeterminado, id_empleado, id_estrategia, id_campaña, id_deudor)
VALUES (1, <6>, <5>, <2>, <1>, <4>); |
| 2.	Botón Generar  mensaje. |
|INSERT INTO Mensaje (id_mensaje, mensaje_predeterminado, id_empleado, id_estrategia, id_campaña, id_deudor)
SELECT
ROW_NUMBER() OVER () + (SELECT COALESCE(MAX(id_mensaje), 0) FROM Mensaje),
'<7>',
e.id_empleado,
ed.id_estrategia,
c.id_campaña,
d.id_deudor
FROM Empleado e
JOIN Empleado_telefono et ON e.id_empleado = et.id_empleado 
JOIN Respuesta r ON e.id_empleado = r.id_empleado
JOIN Deudor d ON r.id_deudor = d.id_deudor
JOIN estrategia_deudor ed ON d.id_deudor = ed.id_deudor
JOIN Estrategia es ON ed.id_estrategia = es.id_estrategia
JOIN Campaña c ON es.id_empleado = c.id_campaña
WHERE
es.tipo_gestion = <3>
AND c.id_campaña = <1>
AND ed.id_estrategia = <2>;|

| Codigo Requerimiento | REQ-05                 |
|-------------|------------------------|
| Codigo Interfaz         | GUI-005-02       |
| Imagen Interfaz                                  |
|![Gestion Tecnologica pantalla2](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/90528509/5b6d6ff6-82ad-4067-bb8c-7cf40ca882ae)|
| Sentencias SQL                                  |
| 1. Boton aplicar: 
SELECT 
(COUNT(CASE WHEN a.estado = 'Logrado' THEN 1 END)::FLOAT / COUNT(*)) * 100 AS porcentaje_logro, 
(c.fecha_fin - CURRENT_DATE) AS dias_restantes, 
COUNT(*) AS cantidad_mensajes_enviados 
FROM Acuerdo a 
JOIN Respuesta r ON a.id_respuesta = r.id_respuesta 
JOIN Mensajes m ON r.id_mensaje = m.id_mensaje 
JOIN Campaña c ON m.id_campaña = c.id_campaña 
WHERE m.id_campaña = '<1>'   
AND m.id_estrategia = '<2>';|





| Codigo Requerimiento | REQ-05                 |
|-------------|------------------------|
| Codigo Interfaz         | GUI-005-03       |
| Imagen Interfaz                                  |
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/97325341/261dbdca-c9fc-44ff-9998-dc38ba82f768) |
| Sentencias SQL                                  |
| 1. Cargar pagina:  |
|SELECT
d.Nombres || ' ' || d.ApellPat || ' ' || d.ApellMat AS Deudor,
d.distrito AS Ubigeo,
EXTRACT(YEAR FROM AGE(NOW(), d.fecha_nac)) AS Edad,
EXTRACT(YEAR FROM AGE(NOW(), deuda.fecha_venc)) AS Antiguedad_Deuda,
deuda.monto_total AS Monto_Total,
estrategia.tipo_gestion AS Tipo_Gestion
FROM Deudor d
JOIN estrategia_deudor ed ON d.id_deudor = ed.id_deudor
JOIN Estrategia estrategia ON ed.id_estrategia = estrategia.id_estrategia
JOIN Deuda deuda ON d.id_deudor = deuda.id_deudor
WHERE
EXTRACT(YEAR FROM AGE(NOW(), d.fecha_nac)) BETWEEN 25 AND 45
AND EXTRACT(YEAR FROM AGE(NOW(), deuda.fecha_venc)) <= 2
AND d.distrito IN ('Lima', 'Callao', 'Arequipa', 'Tumbes')
AND deuda.monto_total BETWEEN 2000 AND 12000;|

### Módulo de Gestion Unitaria

|Código de requerimiento|R-06|
|------------------------|----|
|**Código de interfaz**|GUI-006|
|Imagen interfaz|
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966974/8395b35a-8326-474e-b65f-e7ee9067ffb2)|
|Sentencia SQL|
|Eventos:|
|1.	Opción  “Gestión Unitaria”: Es una opción para visualizar y registrar la respuesta del deudor ante una gestión del ejecutor.|
|2.	Carga de página|
|Combo box Campaña:|
|select cd.id_campaña,c.nombre,count(ed.id_estrategia) as contar,c.estado  from campaña_deuda cd inner join campaña c on c.id_campaña = cd.id_campaña inner join deuda d on d.id_deuda= cd.id_deuda inner join deudor dr on dr.id_deudor=d.id_deudor inner join estrategia_deudor ed n ed.id_deudor=dr.id_deudor inner join estrategia e on e.id_estrategia=ed.id_estrategia WHERE c.estado and ed.estado and e.estado group by cd.id_campaña, c.nombre, c.estado order by count(ed.id_estrategia)|
|Combo box Filtro:|
|select e.id_estrategia,e.nombre_estrategia, count(ed.id_deudor) as contar, e.estado from estrategia e inner join estrategia_deudor ed on e.id_estrategia =ed.id_estrategia where e.estado and ed.id_deudor in ( 	select id_deudor from deuda where id_deuda in(	select cd.id_deuda from campaña_deuda cd inner join campaña c on c.id_campaña = cd.id_campaña WHERE c.estado and c.id_campaña= <1> )  group by e.id_estrategia,e.nombre_estrategia order by e.id_estrategia ;|
|3.	Carga de datos |
|SELECT  D.id_deudor,D.Nombres,D.ApellPat,D.ApellMat, De.monto_total, De.monto_capital, De.monto_total*(1-C.descuento/100) AS monto_descuento, De.origen, AGE(De.fecha_venc) as tiempo, C.descuento FROM Deudor D  inner join Deuda De on D.id_deudor = De.id_deudor inner join campaña_deuda C on De.id_deuda = C.id_deuda WHERE D.id_deudor in (Select   ed.id_deudor from estrategia_deudor ed where ed.id_estrategia = <2> and ed.estado) and C.id_campaña= <1>  ORDER BY C.descuento DESC LIMIT 1;																			|
|SELECT numero, mej_est_con, estado FROM Telefono WHERE id_deudor = <3> ;																		|
|4.	Botón “Registrar Gestión”: Registra la respuesta recibida del Deudor|
|INSERT INTO respuesta (id_respuesta, id_deudor, id_empleado, tipo_contacto, descripcion_contacto, detalle, fecha_gestión VALUES (nextval('seq_respuesta_id'), <3>, id_empleado , <4>, <5>, <6>, CURRENT_DATE)		|
|En caso de dar click En pago, se registrará un pago:|
|SELECT a.id_acuerdo FROM acuerdo  a INNER JOIN respuesta r ON a.id_respuesta = r.id_respuesta WHERE a.estado=1 AND a.tipo_acuerdo=’prom’ AND r.id_deudor=<3>								|
|INSERT INTO pago (id_deudor, id_empleado, id_acuerdo, fecha_pago, monto, num_cuota) VALUES (<3>, id_empleado, id_acuerdo, CURRENT_DATE, <9> , <10>);|
|Select id_respuesta from respuesta order by id_respuesta desc limit 1;|
|INSERT INTO acuerdo (id_respuesta, id_empleado, tipo_acuerdo, monto, fecha_generacion,fecha_pactada, descripcion) VALUES (id_respuesta, id_empleado,  <’prom’ o ‘excep’>, (<7> o <8>),  CURRENT_DATE, <11>, <6>);|
|UPDATE estrategia_deudor SET estado=0 WHERE id_estrategia = <2> AND id_deudor = <3>;|

### Módulo de validación

|Código de requerimiento|R-07|
|------------------------|----|
|**Código de interfaz**|GUI-007|
|Imagen interfaz|
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/7a1dfa32-ad27-4a7d-93cd-3bdb592317ea)|
|Sentencia SQL|
|Eventos:|
|1. Botón “Pagos”: Es una opción para visualizar en forma los pagos pendientes.|
|2. Carga de página: Se carga los datos de pago de los clientes.
SELECT p.id_pago AS N° solicitud, d.DNI AS DNI, p.monto AS Monto pagado, p.estado AS Estado
FROM Pago p, Deudor d
WHERE p.id_deudor = d.id_deudor|
|3. Botón “Detalle”: Se accede a una página para revisar los detalles del pago.|
|4. Botón “Generar cartas de no adeudo”: Se genera las cartas de no adeudo de todos los estados que cambiaron a “Completo”.|


|Código de requerimiento|R-07|
|------------------------|----|
|**Código de interfaz**|GUI-007_1|
|Imagen interfaz|
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/ad68bbc2-f193-42e2-b717-5da6817c9680)|
|Sentencia SQL|
|Eventos:|
|1. Carga de página: 
SELECT pa.id_pago AS Solicitud, dr.DNI, CONCAT(dr.apellpat, ' ',dr.apellmat) AS 
Apellidos, dr.nombres AS Nombres, da.estado AS Tipo_de_consumo, da.origen AS 
Entidad_de_origen_de_deuda, pa.monto AS Monto_pagado, da.monto_total AS 
Deuda_Total, pa.fecha_pago AS Fecha_de_pago 
FROM Deudor dr 
JOIN Deuda da ON da.id_deudor = dr.id_deudor 
LEFT JOIN Pago pa ON pa.id_deudor = dr.id_deudor 
WHERE id_pago= '<1>'|
|2. Botón “Modificar Monto pagado”: Se modifica al último monto que pagó el deudor. 
UPDATE Pago SET monto = <2> 
WHERE id_pago = '<1>'|
|3. Botón “Modificar Fecha de pago”: Se modifica a la última fecha en donde el deudor realizó un pago. 
UPDATE Pago SET fecha_pago = <3> 
WHERE id_pago = '<1>'|
|4. Botón de “Pendiente” o “Completo”: Se modifica el estado del pago. 
UPDATE Pago SET estado = '<4>' 
WHERE id_pago = '<1>'|
|5. Botón “Regresar a solicitudes”: Regresa a la página de validación ubicada en la opción de “pagos”.|

|Código de requerimiento|R-07|
|------------------------|----|
|**Código de interfaz**|GUI-007_2|
|Imagen interfaz|
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/da40d0b8-37dc-41d8-9415-0873599096f4)|
|Sentencia SQL|
|Eventos:|
|1.Botón “Excepciones”: Es una opción para visualizar en forma los excepciones que se realizarán a los deudores en el pago.|
|2. Carga de página:
SELECT A.id_acuerdo AS "N° Solicitud", D.DNI AS "DNI", DEU.monto_total AS "Monto de deuda", A.estado AS "Estado"
FROM Acuerdo A
JOIN Respuesta R ON A.id_respuesta = R.id_respuesta
JOIN Pago P ON A.id_acuerdo = P.id_acuerdo
JOIN Deudor D ON R.id_deudor = D.id_deudor
JOIN Deuda DEU ON D.id_deudor = DEU.id_deudor|
|3. Botón “Detalle”: Se accede a una página para revisar los detalles de la excepción.|


|Código de requerimiento|R-07|
|------------------------|----|
|**Código de interfaz**|GUI-007_3|
|Imagen interfaz|
|![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/3836e612-84ee-4276-abd8-a2db8e358938)|
|Sentencia SQL|
|Eventos:|
|1.	Carga de página:
SELECT A.id_acuerdo AS N°_solicitud, D.DNI AS DNI, CONCAT(D.apellpat,' ',D.apellmat) AS Apellidos, D.nombres AS Nombres, DEU.estado AS Tipo_de_Consumo, DEU.origen AS Entidad_de_origen_de_consumo, DEU.fecha_venc AS Fecha_de_deuda, DEU.monto_total AS Deuda_total, A.razón AS Justificación_del_deudor
FROM Acuerdo A
JOIN Respuesta R ON A.id_respuesta = R.id_respuesta
JOIN Pago P ON A.id_acuerdo = P.id_acuerdo
JOIN Deudor D ON R.id_deudor = D.id_deudor
JOIN Deuda DEU ON D.id_deudor = DEU.id_deudor
WHERE A.id_acuerdo = '<1>'|
|2. Botón de “Aceptar” o “Rechazar”: Se modifica el estado de excepción.
UPDATE Acuerdo SET estado = '<2>'
WHERE id_acuerdo = '<1>'|
|3. Botón “Regresar a solicitudes”: Regresa a la página de validación ubicada en la opción de “Excepciones”.|

