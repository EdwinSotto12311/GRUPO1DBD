## GESTOR DE BASE DE DATOS NoSQL
### Tipo de motor de búsqueda: Orientada a grafos
El concepto de base de datos orientada a grafos se remonta a la década de 1960, cuando las bases de datos de modelos de red comenzaron a soportar estructuras de grafos. En la década de 1980, el modelo de datos lógico introdujo grafos etiquetados. Desde entonces, las bases de datos orientadas a grafos han evolucionado y se han convertido en una plataforma especializada y de un solo propósito para crear y manipular grafos.
Una base de datos orientada a grafos es una plataforma especializada y de un solo propósito para crear y manipular grafos. Los grafos contienen nodos, bordes y propiedades que se utilizan para representar y almacenar datos de una forma que no permiten las bases de datos relacionales. La analítica de grafos es otro término de uso común y hace referencia específicamente al proceso de analizar datos en un formato de grafo utilizando los puntos de datos como nodos y las relaciones como bordes.
Hay dos modelos comunes de bases de datos orientadas a grafos: grafos de propiedades y grafos RDF. Los grafos de propiedades se centran en el análisis y las consultas, y los RDF se centran en la integración de datos.

#### Ventajas:
• Flexibilidad: Las bases de datos orientadas a grafos son muy flexibles y pueden manejar datos no estructurados y semiestructurados. Esto significa que pueden manejar datos que no encajan en una tabla relacional.
• Escalabilidad: Las bases de datos orientadas a grafos son altamente escalables y pueden manejar grandes cantidades de datos. Esto se debe a que los grafos son inherentemente escalables
• Rendimiento: Las bases de datos orientadas a grafos son muy rápidas para ciertas consultas, como las que involucran relaciones complejas entre los datos. Esto se debe a que los grafos son inherentemente eficientes para modelar y consultar datos relacionales.
• Análisis de grafos: Las bases de datos orientadas a grafos son ideales para el análisis de grafos, que es el proceso de analizar datos en un formato de grafo utilizando los puntos de datos como nodos y las relaciones como bordes. Esto permite a los usuarios descubrir patrones y relaciones en los datos que de otra manera serían difíciles de detectar.
• Integración de datos: Las bases de datos orientadas a grafos son ideales para la integración de datos, ya que pueden manejar datos de diferentes fuentes y formatos. Esto significa que pueden integrar datos de diferentes sistemas y aplicaciones sin problemas.
• Datos complejos: Las bases de datos orientadas a grafos son ideales para manejar datos complejos, como datos de redes sociales, datos de geolocalización y datos de sistemas de recomendación. Esto se debe a que los grafos son inherentemente buenos para modelar y consultar datos complejos.

### Motor de búsqueda: Neo4J
Es una plataforma de datos de grafos que ofrece una amplia gama de herramientas y aplicaciones para crear y administrar grafos, realizar análisis de grafos y escalar aplicaciones con búsqueda vectorial.
#### Ventajas:
• Rendimiento: Neo4j es muy rápido y escalable. Puede manejar grandes cantidades de datos de manera muy eficiente.
• Facilidad de uso: Neo4j es muy fácil de usar. Tiene una interfaz amigable que hace que sea fácil de aprender y usar.
• Flexibilidad: Neo4j es muy flexible y puede manejar datos no estructurados y semiestructurados. Esto significa que puede manejar datos que no encajan en una tabla relacional.
• Análisis de grafos: Neo4j es ideal para el análisis de grafos, que es el proceso de analizar datos en un formato de grafo utilizando los puntos de datos como nodos y las relaciones como bordes. Esto permite a los usuarios descubrir patrones y relaciones en los datos que de otra manera serían difíciles de detectar.
• Escalabilidad: Neo4j es altamente escalable y puede manejar grandes cantidades de datos. Esto se debe a que los grafos son inherentemente escalables.
• Comunidad de usuarios: La comunidad de usuarios de Neo4j es una de las más grandes y activas del mundo NoSQL. Los miembros de esta comunidad han contribuido a crear un ambiente de colaboración altamente productivo donde las dudas y problemas que se presenten con la estructuración de tus proyectos pueden ser resueltas de forma rápida.

### Descripción de escenario de uso
#### Escenario: Cobranzas

En el desarrollo de la app para escritorio de la empresa de cobranzas, se identificó al módulo de validacion y gestion unitaria como un escenario que puede beneficiarse significativamente de una base de datos NoSQL de tipo grafo en comparación con una relacional. A continuación, se exploran las tareas que se realizan en este módulo y las ventajas específicas en la eficiencia de tareas clave de cobranzas utilizando un motor de tipo grafo (Neo4j) en contraste con un motor relacional (PostgresSQL):

Tarea 1: Seguimiento de la evolución de pago y acuerdos

En esta tarea, se tiene que gestionar el seguimiento de la evolución de los pagos y acuerdos a lo largo del tiempo, principalmente para tener en cuenta la validacion de deuda y su interpretacion de resultados para los acuerdos. El enfoque de grafos muestra ventajas dado que las bases de datos de grafos permiten representar y analizar las relaciones entre los datos de una manera muy intuitiva y flexible. Neo4j puede manejar grandes volúmenes de datos y consultas complejas, lo que facilita el seguimiento rápido y eficiente de la evolución de las deudas

Rendimiento en consultas de grafos:

La estructura de grafos supera a los motores relacionales al realizar consultas de grafos complejas de manera eficiente. Esto es crucial para seguir la evolución de las deudas y detectar patrones en los datos.

Escalabilidad:

En comparación con los motores relacionales, se destaca en las bases de datos de grafos la escalabilidad, permitiendo manejar grandes volúmenes de datos de manera efectiva y sostenible a medida que crecerá la actividad de cobranzas de tu empresa.

Flexibilidad:

Las bases de datos de grafos no requieren un esquema predefinido, ofrecen una gran flexibilidad y te permiten adaptar la base de datos a tus necesidades específicas. Esto es especialmente útil en un entorno de cobranzas, donde las relaciones entre los datos pueden ser complejas y cambiar con el tiempo.
### Configuración
#### Instalación de Neo4J
1. Vamos al enlace y descargamos neo4j deskop de acuerdo al sistema operativo
https://neo4j.com/download/
![Imagen de WhatsApp 2023-12-06 a las 13 05 42_a0e4387a](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/080b3dfc-bf32-4da0-a2f9-995aba09c6c7)

2. Damos click a Download y nos pedira colocar nuestros datos para poder recibir la licencia gratuita
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/c485fe2a-5e32-4637-add5-3cd94bb118f0)


3. Copiamos y pegamos la licencia gratuita
![Imagen de WhatsApp 2023-12-06 a las 13 05 43_58a9292c](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/83815c14-b5ba-4607-ba0f-9dae65e7ecb0)

4. Ejecutamos el archivo setup para descargar neo4j desktop
![Imagen de WhatsApp 2023-12-06 a las 13 05 43_686fa30a](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/f232e4f5-40ee-4024-b487-c286460ff829)

5. Configuramos la ruta de descarga

![Imagen de WhatsApp 2023-12-06 a las 13 05 43_fc24a31d](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/43564d00-eb3d-44f4-a18d-7e6237e58fce)

6. Colocamos la licencia para poder obtener la app de escritorio con facilidad
![Imagen de WhatsApp 2023-12-06 a las 13 05 44_a7bff018](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/bcb91055-fd22-4d2b-b217-119fa2be58f2)

7. Creamos proyecto

![Imagen de WhatsApp 2023-12-06 a las 13 05 44_6095494a](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/8655d9e3-d84a-4bc5-931a-69c2db543573)

8. Configuramos nombre y contraseña
![Imagen de WhatsApp 2023-12-06 a las 13 05 45_117e3ffc](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/950a8f05-99ec-4e41-bdd3-abc9c90242bc)

9. Damos click a Start  
![Imagen de WhatsApp 2023-12-06 a las 13 06 18_65abfcf5](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/15389a5a-a2e0-4b41-9bc5-689ae8cd32d3)

10. Damos click a Open

![Imagen de WhatsApp 2023-12-06 a las 13 09 11_71a18183](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/50fcc036-550e-4833-8c2e-d13af3a60691)

### Implementación
1. Crear nodos para las tareas:
![Imagen de WhatsApp 2023-12-06 a las 13 21 03_3a3cb7dd](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/46d99991-22bf-45ae-a4ce-1eab99c0aec3)

|CREATE (e1:Empleado {Nombres: 'Juan', ApellMat: 'Pérez', ApellPat: 'García', rol: 'Agente de Cobranza', DNI: '12345678', usuario: 'jperez', contraseña: 'password1', id_empleado: 1}),|
|---|
|(e2:Empleado {Nombres: 'Ana', ApellMat: 'Martínez', ApellPat: 'López', rol: 'Supervisor', DNI: '87654321', usuario: 'amartinez', contraseña: 'password2', id_empleado: 2}), 
|(e3:Empleado {Nombres: 'Carlos', ApellMat: 'Rodríguez', ApellPat: 'Gómez', rol: 'Agente de Cobranza', DNI: '98765432', usuario: 'crodriguez', contraseña: 'password3', id_empleado: 3}),|
|(e4:Empleado {Nombres: 'María', ApellMat: 'Sánchez', ApellPat: 'Fernández', rol: 'Analista de Datos', DNI: '23456789', usuario: 'msanchez', contraseña: 'password4', id_empleado: 4}),|
|(e5:Empleado {Nombres: 'Pedro', ApellMat: 'Díaz', ApellPat: 'Ramírez', rol: 'Agente de Cobranza', DNI: '34567890', usuario: 'pdiaz', contraseña: 'password5', id_empleado: 5});|
![Imagen de WhatsApp 2023-12-06 a las 13 21 04_b9500ad0](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/6d67df7e-517c-4be1-bf7e-fc25e7c815f3)

|CREATE (d1:Deudor {Nombres: 'Eduardo', ApellPat: 'Gómez', ApellMat: 'Ramírez', fecha_nac: '1985-09-20', DNI: '76543210', id_deudor: 1001, calle: 'Calle A', distrito: 'San Isidro', num_puerta: 456, registro_salud: 'B987654'}),|
|---|
|(d2:Deudor {Nombres: 'Laura', ApellPat: 'Fernández', ApellMat: 'López', fecha_nac: '1992-03-15', DNI: '65432109', id_deudor: 1002, calle: 'Calle B', distrito: 'Miraflores', num_puerta: 789, registro_salud: 'C876543'}),|
|(d3:Deudor {Nombres: 'Roberto', ApellPat: 'Martínez', ApellMat: 'García', fecha_nac: '1978-07-10', DNI: '54321098', id_deudor: 1003, calle: 'Calle C', distrito: 'Barranco', num_puerta: 123, registro_salud: 'A765432'}),|
|(d4:Deudor {Nombres: 'Sofía', ApellPat: 'López', ApellMat: 'Díaz', fecha_nac: '1989-12-05', DNI: '43210987', id_deudor: 1004, calle: 'Calle D', distrito: 'Chorrillos', num_puerta: 567, registro_salud: 'D654321'}),|
|(d5:Deudor {Nombres: 'Alejandro', ApellPat: 'Ramírez', ApellMat: 'Sánchez', fecha_nac: '1980-01-25', DNI: '32109876', id_deudor: 1005, calle: 'Calle E', distrito: 'Surco', num_puerta: 890, registro_salud: 'E543210'});|

![Imagen de WhatsApp 2023-12-06 a las 13 21 04_bd5e99a5](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/bcb028d4-0e59-4949-b8b2-33efadb25dad)

|CREATE (r1:Respuesta {Descripcion_contacto: 'Llamada exitosa', tipo_contacto: 'Telefónico', Detalle: 'Acuerdo de pago', fecha_gestión: '2023-02-15', id_respuesta: 5001, id_empleado: 1, id_deudor: 1001}),|
|---|
|(r2:Respuesta {Descripcion_contacto: 'Correo enviado', tipo_contacto: 'Email', Detalle: 'Confirmación de pago', fecha_gestión: '2023-02-20', id_respuesta: 5002, id_empleado: 2, id_deudor: 1002}),|
|(r3:Respuesta {Descripcion_contacto: 'No disponible', tipo_contacto: 'Visita', Detalle: 'No se pudo contactar', fecha_gestión: '2023-02-25', id_respuesta: 5003, id_empleado: 3, id_deudor: 1003}),|
|(r4:Respuesta {Descripcion_contacto: 'Llamada sin respuesta', tipo_contacto: 'Telefónico', Detalle: 'Dejar mensaje en buzón', fecha_gestión: '2023-03-01', id_respuesta: 5004, id_empleado: 4, id_deudor: 1004}),|
|(r5:Respuesta {Descripcion_contacto: 'SMS enviado', tipo_contacto: 'Mensaje de texto', Detalle: 'Recordatorio de pago', fecha_gestión: '2023-03-05', id_respuesta: 5005, id_empleado: 5, id_deudor: 1005});|

![Imagen de WhatsApp 2023-12-06 a las 13 21 04_d4e86fdb](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/d78f325e-2e49-42fe-b9b7-e01a49243fce)

|CREATE (de1:Deuda {fecha_venc: '2023-04-30', monto_total: 2000.00, monto_capital: 1800.00, estado: 'Pendiente', origen: 'Tarjeta de crédito', id_deuda: 3001, id_deudor: 1001}),|
|---|
|(de2:Deuda {fecha_venc: '2023-03-15', monto_total: 1200.00, monto_capital: 1000.00, estado: 'Pendiente', origen: 'Préstamo Personal', id_deuda: 3002, id_deudor: 1002}),|
|(de3:Deuda {fecha_venc: '2023-05-20', monto_total: 2500.00, monto_capital: 2200.00, estado: 'Pendiente', origen: 'Tarjeta de crédito', id_deuda: 3003, id_deudor: 1003}),|
|(de4:Deuda {fecha_venc: '2023-03-01', monto_total: 1500.00, monto_capital: 1300.00, estado: 'Pendiente', origen: 'Préstamo Hipotecario', id_deuda: 3004, id_deudor: 1004}),|
|(de5:Deuda {fecha_venc: '2023-04-10', monto_total: 1800.00, monto_capital: 1600.00, estado: 'Pendiente', origen: 'Tarjeta de crédito', id_deuda: 3005, id_deudor: 1005});|

![Imagen de WhatsApp 2023-12-06 a las 13 21 04_df89b1e6](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/e244f80c-3240-42d6-9856-9bf152e8723e)

2.Ver nodos empleado para ver si se ejecutó correctamente:
![Imagen de WhatsApp 2023-12-06 a las 13 21 26_cc25ba25](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/0c5acc51-b173-4a74-afd6-867fb4655224)
MATCH (n:Empleado) RETURN n LIMIT 25

3. Crear relaciones para cuando empleados hallan realizado acuerdos. Asi se obtendrian ademas metricas de desempeño.
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/97325341/96bd88fc-546d-4f54-b376-5aab6063cdc0)
Relación entre Empleado y Acuerdo
MATCH (e:Empleado), (a:Acuerdo)
WHERE e.id_empleado = a.id_empleado
CREATE (e)-[:RealizaAcuerdo]->(a);

4. Crear relacion entre deudor y acuerdo
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/97325341/957e7f2e-4123-4922-b3bd-330325dbceaa)

MATCH (d:Deudor), (a:Acuerdo)
WHERE d.id_deudor = a.id_deudor
CREATE (d)-[:TieneAcuerdo]->(a);

6. Crear la asociacion entre pago y deudor
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/97325341/d3f5ec4c-f138-4440-b3d7-32b913d0752b)
 
Relación entre Pago y Deudor
MATCH (p:Pago), (d:Deudor)
WHERE p.id_deudor = d.id_deudor
CREATE (p)-[:REALIZADO_POR]->(d);
7. Relacion entre pago y deuda, siempre y cuando este en pagado.
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/97325341/4efc9cf5-8b97-4527-9688-20a190e59bf0)

Relación entre Pago y Deuda (cuando el pago está "pagado")
MATCH (p:Pago {estado: 'Pagado'}), (d:Deuda)
WHERE p.id_deudor = d.id_deudor
CREATE (p)-[:CORRESPONDE_A]->(d);

8. Ver los nodos finales
![image](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/97325341/0e24b607-e140-48e8-86ac-d5cf326441ef)
MATCH (n)
RETURN n;
10. CUANDO SE REALIZE EL POBLAMIENTO CORRECTO DE DATOS, SE DEBERIA VER ASI:
![orientada a grafos](https://github.com/EdwinSotto12311/GRUPO1DBD/assets/144966920/76ca31f1-6cd2-4031-828d-5bbc6cfed9e8)
